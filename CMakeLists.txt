cmake_minimum_required(VERSION 3.26)
project(TP)

set(CMAKE_CXX_STANDARD 20)

add_executable(TP src/main.cpp
        lib/Terminal.cpp
        lib/Terminal.h
        src/Aparelhos/Aparelho.h
        src/Aparelhos/Aparelho.cpp
        src/Processadores/ProcessadorRegras.cpp
        src/Processadores/Regra.h
        src/Processadores/Regra.cpp
        src/Propriedades/Propriedade.cpp
        src/Sensores/FumoSensor.h
        src/Sensores/FumoSensor.cpp
        src/Sensores/HumidadeSensor.h
        src/Sensores/HumidadeSensor.cpp
        src/Sensores/LuminosidadeSensor.cpp
        src/Sensores/MovimentoSensor.cpp
        src/Sensores/RadiacaoSensor.h
        src/Sensores/RadiacaoSensor.cpp
        src/Sensores/Sensor.cpp
        src/Sensores/SomSensor.h
        src/Sensores/SomSensor.cpp
        src/Sensores/TemperaturaSensor.h
        src/Sensores/TemperaturaSensor.cpp
        src/Zonas/Zona.cpp
        src/Interface/Interface.cpp
        src/Interface/Interface.h
        src/Terreno/Terreno.cpp
        src/Habitacao/Habitacao.cpp)

target_link_libraries(${PROJECT_NAME} C:/PDCurses-3.9/wincon/pdcurses.a)