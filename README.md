# ACIII
Новый метод шифрования для приложений на платформе .NET Framework 4.7.2
## :point_right: Ссылка на скачивание : **https://yadi.sk/d/KREzjdpWcWjN6g**


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
            Console.ReadLine();
        }
    }
}
```
В результате работы программы(в этом примере) вы получите такие сообщения в консоле : 
![ACIIIExample1](https://downloader.disk.yandex.ru/preview/763b776d78efc125d2d7790482af7aefbf6e9d6dce99daa85c1f8275014289dc/5cf317cd/zIvvq_bS8cgR_88wdRL7Z-KmKAsagD6NXWjENJMociY4zYOqkyY8EAv9LFTsbpeDBbgDs7JOlQY1EmrvsPIC6A%3D%3D?uid=0&filename=ACIIIExample1.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&tknv=v2&size=2048x2048 "Пример работы шифрования ACIII")
> Метод `EncryptToACIII();` возвращает только значения типа `string`

