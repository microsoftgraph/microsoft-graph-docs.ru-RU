# <a name="accessing-shared-driveitems"></a>Доступ к общим элементам DriveItem

Вы можете получить доступ к общим элементам [DriveItem](../resources/driveitem.md) или коллекции общих элементов, используя параметр **shareId** или URL-адрес для совместного доступа.

Чтобы использовать URL-адрес для совместного доступа с этим API, вашему приложению необходимо [ преобразовать URL-адрес в токен общего доступа](#transform-a-sharing-url).

## <a name="prerequisites"></a>Необходимые компоненты

Для применения этого API требуется одна из указанных **областей**:

  * Files.ReadWrite

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /shares/{sharingIdOrUrl}
```

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `200 OK` и ресурс [sharedDriveItem](../resources/shareddriveitem.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Вот пример запроса для получения общего элемента:

<!-- {
  "blockType": "request",
  "name": "get_shares_by_url"
}-->
```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}
```
##### <a name="response"></a>Отклик

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedDriveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```

## <a name="access-the-shared-item-directly"></a>Прямой доступ к общему элементу

Так как элемент [**SharedDriveItem**](../resources/shareddriveitem.md) содержит полезную информацию, большинство приложений будут стремиться получить прямой доступ к общему элементу [DriveItem](../resources/driveitem.md). Ресурс **SharedDriveItem** включает связи **корня** и **элементов**, которые могут получать доступ к содержимому в области общего элемента.

### <a name="exmaple-single-file"></a>Пример (один файл)

##### <a name="request"></a>Запрос

При запросе связи **корня** будет возвращен элемент **DriveItem**, к которому был предоставлен доступ.

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root
```

##### <a name="response"></a>Отклик

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

### <a name="exmaple-shared-folder"></a>Пример (общая папка)

##### <a name="request"></a>Запрос

При запросе связи **корня** и расширении **дочерней** коллекции будет возвращен элемент **DriveItem**, к которому был предоставлен доступ, а также файлы в общей папке.

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root?$expand=children
```

##### <a name="response"></a>Отклик

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {}
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="transform-a-sharing-url"></a>Преобразование URL-адреса для совместного доступа

Чтобы получить доступ к URL-адресу для совместного доступа с помощью API **общих ресурсов**, необходимо преобразовать URL-адрес в токен для совместного доступа.

Чтобы преобразовать URL-адрес в токен для совместного доступа, выполните указанные ниже действия.

1. Закодируйте URL-адрес для общего доступа с использованием кодировки Base64.
2. Преобразуйте данные в кодировке Base64 в [формат URL-адреса с недополненной кодировкой Base64](https://en.wikipedia.org/wiki/Base64), выполнив указанные ниже действия.
  1. Усеките конечные символы `=` в строке.
  2. Замените небезопасные символы URL-адреса эквивалентными символами; замените `/` на `_`, а `+` — на `-`.
3. Добавьте `u!` в начало строки.

Например, указанный ниже метод C# преобразует входную строку в токен общего доступа.

```csharp
string UrlToSharingToken(string inputUrl) {
  var base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(inputUrl));
  return "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
