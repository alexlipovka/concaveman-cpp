# Порядок построения библиотеки

1. Скачать и установить проект [TDM-GCC](https://jmeubank.github.io/tdm-gcc/)
2. Открыть терминал Windows (обычный CMD)
3. Перейти с папку `cpp`
4. Выполнить команду `g++ -c -o concaveman.o concaveman.cpp -std=c++11`
5. Выполнить команду `g++ -o .\concaveman.dll -s -shared concaveman.o -Wl,--subsystem,windows`
6. Изменить путь к скомпилированной библиотеке в файле concaveman.py
   `_lib = _ffi.dlopen('Диск:/полный/путь/к/concaveman.dll`