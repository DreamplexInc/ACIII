# ACIII
## Ссылка на скачивание : 
Новый метод шифрования для приложений на платформе .NET Framework 4.7.2

# Как пользоваться?
- Подключите библиотеку к своему проекту
- Подключите директиву библиотеки в коде вашей программы
```c#
using dwnclib;
```
- Создайте экземпляр класса Encryption
```c#
Encryption _Encryption = new Encryption();
```
- Для шифрования текста в ACIII, впишите след. код :
```c#
Encrypt.EncryptToACIII("TXT", Encryption.EncryptionModule.ACIIIModuleToHPI);
```
> Этот метод возвращает текстовые значения (string)
> Вместо "TXT" можете исполльзовать другие значения типа ```c# string ```

