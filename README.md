# ACIII
Новый метод шифрования для приложений на платформе .NET Framework 4.7.2
## Ссылка на скачивание : 


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
- Пример использования класса Encryption :
```c#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using dwnclib;

namespace ACIII
{
    class Program
    {
        static Encryption _Enc = new Encryption();
        static void Main(string[] args)
        {
            string t;
            t = _Enc.EncryptToACIII("Hello, World!", Encryption.EncryptionModule.ACIIIModuleToHPI);
            Console.WriteLine($"Оригинал : Hello, World!\nЗашифрованный в ACIII : {t}");
        }
    }
}
```
> Этот метод возвращает текстовые значения (string)
> Вместо "TXT" можете исполльзовать другие значения типа ```c# string ```

