# rtc_functionality

## Description
A simple kernel module with a user-space application.

## Project Structure
```
rtc_functionality/
├── kernel_module/
│   ├── src/
│   │   └── rtc_functionality.c
│   ├── include/
│   │   └── rtc_functionality.h
│   └── Makefile
└── application/
    ├── main.c
    └── CMakeLists.txt
```

## Build

### Kernel Module
```bash
cd rtc_functionality/kernel_module
make
```

### Application
```bash
cd rtc_functionality/application
cmake .
make
```

## Usage

### Kernel Module
```bash
sudo insmod rtc_functionality/kernel_module/rtc_functionality.ko
# Do something with the module
sudo rmmod rtc_functionality
```

### Application
```bash
cd rtc_functionality/application
./test_app
```

## License
GPL
