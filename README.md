# ACIII
## Ссылка на скачивание : 
Новый метод шифрования для приложений на платформе .NET Framework 4.7.2

# Как пользоваться?
- Подключите библиотеку к своему проекту
- Подключите директиву библиотеки в коде вашей программы
<csharp>using dwnclib;<csharp>
- Создайте экземпляр класса Encryption
- Для шифрования текста в ACIII, впишите след. код :
> Encrypt.EncryptToACIII(encBox.Text, Encryption.EncryptionModule.ACIIIModuleToHPI);
>> Этот метод возвращает текстовые значения (string)
