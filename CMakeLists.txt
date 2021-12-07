# cmake_minimum_required(VERSION <specify CMake version here>)
project(servoByBoard)

set(CMAKE_CXX_STANDARD 14)

add_executable(servoByBoard main.cpp Emakefun_MotorShield.cpp Emakefun_MotorShield.h Emakefun_MotorDriver.cpp Emakefun_MotorDriver.h Raspi_i2c.cpp Raspi_i2c.h)

target_link_libraries(servoByBoard wiringPi)