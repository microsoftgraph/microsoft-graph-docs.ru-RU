---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Доступ к общим элементам
localization_priority: Normal
ms.openlocfilehash: 46779e40862c7056cc60ef4be55595da5615e9f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864241"
---
# <a name="accessing-shared-driveitems"></a>Доступ к общим элементам DriveItem

Вы можете получить доступ к общим элементам [DriveItem](../resources/driveitem.md) или коллекции общих элементов, используя параметр **shareId** или URL-адрес для совместного доступа.

Чтобы использовать URL-адрес для совместного доступа с этим API, вашему приложению необходимо [преобразовать URL-адрес в токен общего доступа](#encoding-sharing-urls).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All    |
|Для приложений | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a>Параметры пути

| Имя параметра        | Значение    | Описание                                                                         |
|:----------------------|:---------|:------------------------------------------------------------------------------------|
| **sharingTokenOrUrl** | `string` | Обязательный. Маркер общего доступа, возвращенный API, или правильно закодированный URL-адрес для общего доступа. |

### <a name="encoding-sharing-urls"></a>Кодирование URL-адресов для общего доступа

Чтобы закодировать URL-адрес для общего доступа, используйте следующую логику:

1. Для начала примените к URL-адресу кодировку base64.
2. Преобразуйте результат из кодировки base64 в [недополненный формат base64url](https://en.wikipedia.org/wiki/Base64), удалив символы `=` в конце значения и заменив `/` символом `_`, а `+` — символом `-`.)
3. Добавьте `u!` в начало строки.

Ниже показан пример кодирования URL-адреса в языке C#:

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="response"></a>Ответ

При успешном выполнении этот метод возвращает код отклика `200 OK` и ресурс [sharedDriveItem](../resources/shareddriveitem.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Вот пример запроса для получения общего элемента:

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET https://graph.microsoft.com/beta/shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.sharedDriveItem" } -->

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
  },
  "remoteItem": { 
    "driveId": "",
    "id": ""
  }
}
```

## <a name="access-the-shared-item-directly"></a>Прямой доступ к общему элементу

Так как элемент [**SharedDriveItem**](../resources/shareddriveitem.md) содержит полезную информацию, большинство приложений будут стремиться получить прямой доступ к общему элементу [DriveItem](../resources/driveitem.md). Ресурс **SharedDriveItem** включает связи **корня** и **элементов**, которые могут получать доступ к содержимому в области общего элемента.

## <a name="example-single-file"></a>Пример (один файл)

### <a name="request"></a>Запрос

При запросе связи **driveItem** будет возвращен элемент **DriveItem**, к которому предоставлен общий доступ.

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a>Ответ

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

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

## <a name="example-shared-folder"></a>Пример (общая папка)

### <a name="request"></a>Запрос

При запросе связи **driveItem** и расширении коллекции **children** будет возвращен элемент **DriveItem**, к которому предоставлен общий доступ, а также файлы, содержащиеся в общей папке.

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET https://graph.microsoft.com/beta/shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a>Ответ

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {},
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

## <a name="remarks"></a>Замечания

* В случае OneDrive для бизнеса и SharePoint API общих ресурсов всегда требует аутентификации. С его помощью невозможно обращаться к содержимому, доступ к которому предоставлен анонимно, без контекста пользователя.

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link"
} -->
