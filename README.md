# ACIII
Новый метод шифрования текста в **С# 7.2**
#### Тип проекта : Библиотека .NET Framework
#### Версия проекта : v1.2
## :point_right: Ссылка на скачивание : **<...Идет тест новой библиотеки...>**
##### > На данный момент не доступно расшифровывание кодировки ACIII(Эйси-3)

# Внимание!!! Новая версия библиотеки
Скоро в новой версии, мы выпустим несколько новых методов, которые помогут вам защитить ваши данные, а именно данные предоставленные в форме текста (не зашифрованные и уязвимые)

# Таблица ACIII
#### С нижним регистром
- a -> SfZLMK
- b -> IVPHnK
- c -> VlGKNH
- d -> jHgSjN
- e -> kbmVTs
- f -> GrIoLMS
- g -> ufhmBs
- h -> DdDpyO
- i -> JhhCvh
- j -> bFrcOV
- k -> DCRzpA
- l -> VlGKNH
- m -> avYCLP
- n -> USbKzo
- o -> YeiaHn
- p -> zXNiKI
- q -> GkDeNP
- r -> SDOimz
- s -> VgxpvT
- t -> oMNSuS
- u -> YxzKfT
- v -> yRJChS
- w -> ycoEVP
- x -> GeLmnn
- y -> gnUpXt
- z -> jsIkTa
#### С верхним регистром
- A -> UaHNFp
- B -> vIDQYx
- C -> wIbDCT
- D -> Bueqip
- E -> VipNYa
- F -> OkndYR
- G -> LxayGP
- H -> KXQNBk
- I -> aRkDRx
- J -> CImfax
- K -> eeUEib
- L -> ubssBi
- M -> JhggYK
- N -> yjRtse
- O -> IzQvua
- P -> xtntPU
- Q -> zxFnIx
- R -> OpKHbl
- S -> cJPtMW
- T -> tFenYY
- U -> ZIiOds
- V -> LzfLCR
- W -> jDqgzN
- X -> EVkuwr
- Y -> sSkidu
- Z -> lzibOu

# Как пользоваться?
- Подключите библиотеку к своему проекту
- Подключите директиву библиотеки в коде вашей программы
```c#
using Dreamplex.ACIII;
```
- Создайте экземпляр класса Encryption
```c#
ACIIIEncryption _ACIIIEnc = new ACIIIEncryption();
```
- Пример использования класса ACIIIEncryption :
```c#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
//Компоненты от Dreamplex
using Dreamplex.ACIII; //Подключаем библиотеку для использования ACIII шифрования

namespace ACIIIApp
{
    class Program
    {
        static void Main(string[] args)
        {
            //Создаем переменную, откуда и будем брать написанный нами текст
            string _Input = "";
            //Создаем экземпляр класса ACIIIEncryption
            ACIIIEncryption _ACIIIEncryption = new ACIIIEncryption();
            //Выводим сообщение приветствия и т.д.
            Console.Write("Добро пожаловать в среду ACIII App!");
            Console.Write("\nВведите ваш шифруемый текст : ");
            _Input = Console.ReadLine();
            //Показываем зашифрованный текст (результат)
            Console.Write($"\nРезультат шифрования : {_ACIIIEncryption.EncryptTextToACIII(_Input, ACIIIEncryption.EncryptionModule.ACIIIModule)}" );

            //Конечное сообщение в консоли
            Console.Write("\nДля продолжения нажмите любую клавишу...");
            Console.ReadLine();
        }
    }
}

```
В результате работы программы(в этом примере) вы получите такие сообщения в консоле : 
![ACIIIExample1](https://downloader.disk.yandex.ru/preview/763b776d78efc125d2d7790482af7aefbf6e9d6dce99daa85c1f8275014289dc/5cf317cd/zIvvq_bS8cgR_88wdRL7Z-KmKAsagD6NXWjENJMociY4zYOqkyY8EAv9LFTsbpeDBbgDs7JOlQY1EmrvsPIC6A%3D%3D?uid=0&filename=ACIIIExample1.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&tknv=v2&size=2048x2048 "Пример работы шифрования ACIII")
> ##### Метод `EncryptTextToACIII(string _EncryptableText, EncryptionMethod _EncryptionMethod);` возвращает только значения типа `string`
> ##### Метод `EncryptFileToACIII(string _FileName, EncryptionMethod _EncryptionMethod);` не возвращает значения, т.к. этот метод является типом `void`. Этот метод шифрует данные в ACIII, которые находятся в файле

#Справочник функций
>
- Шифрование текста
```c#
EncryptTextToACIII(string _EncryptableText, EncryptionMethod _EncryptionMethod);
```
- Шифрование текста в файле
```c#
EncryptFileToACIII(string _FileName, EncryptionMethod _EncryptionMethod);
```
- Получить текст из файла
```c#
ReadTextFromFile(string _FileName);
```
- Сохранить зашифрованные данные в отдельный файл
```c#
SaveEncryptedTextToFile(string _FileName, string _WritableText);
```

> Шифрует текстовое значение предоставленное в типе **string**, в **ACIII** кодировку с типом **string**

# Социальная сеть
#### ВКонтакте : **https://vk.com/the_dreamplex**
#### ACIII Вконтакте : **https://vk.com/aciii_code**
#### Разработчик Вконтакте : **https://vk.com/dragonree**
