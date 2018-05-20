# CheckReceiptSDK
Библиотека для получения информации по чекам от ФНС

Пример вызова методов:

Регистрации:
```csharp
var result = FNS.RegistrationAsync("some@mail.com", "Name", "+79991234567");
```
Восстановления пароля:
```csharp
var result = FNS.RestorePasswordAsync("+79991234567");
```
Проверки существования чека:
```csharp
var date = DateTime.Parse("2018-05-18T22:05:00");
var result = FNS.CheckAsync("8710000101337659", "94248", "815426975", date, 235.61);
```
Получения детальной информации по чеку:
```csharp
var result = FNS.ReceiveAsync("8710000101337659", "94248", "815426975", "+79991234567", "123456");
```
