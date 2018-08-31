---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Создание списка пользователей, имеющих доступ к файлу
ms.openlocfilehash: d7090939fb2b950ed92fd9574cf9dd5b80ec8a6c
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266634"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a>Создание списка разрешений на общий доступ в элементе DriveItem

Создание списка действующих разрешений на общий доступ в элементе [DriveItem](../resources/driveitem.md).

## <a name="access-to-sharing-permissions"></a>Доступ к разрешениями на общий доступ

Коллекция разрешений включает потенциально конфиденциальные сведения и может быть доступна не для всех вызывающих объектов.

* Для владельца элемента возвращаются все разрешения на общий доступ. К владельцам элемента также относятся его совладельцы.
* Вызывающему объекту, который не является владельцем, возвращаются только применяемые к нему разрешения.
* Свойства разрешений на общий доступ, содержащие секреты (например, `shareId` и `webUrl`), возвращаются только для вызывающих объектов, которые могут создать разрешение на общий доступ.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Для приложений | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](../../../concepts/query_parameters.md) `$select` для настройки отклика.

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя          | Тип   | Описание                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | строковый | Если указан этот заголовок запроса, а предоставленный тег etag совпадает с текущим тегом etag элемента, будет возвращен отклик `HTTP 304 Not Modified`. |

## <a name="response"></a>Ответ

При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию ресурсов [Permission](../resources/permission.md) в теле отклика.

Действующие разрешения на общий доступ для элемента DriveItem могут быть получены двумя путями:

* разрешения на общий доступ, примененные непосредственно к самому элементу DriveItem;
* разрешения на общий доступ, унаследованные от предков элемента DriveItem.

Абоненты могут распознать унаследованное разрешение, проверив свойство **inheritedFrom**. Это свойство — ресурс [**itemReference**](../resources/itemreference.md), отсылающий к предшествующему элементу, от которого унаследовано разрешение.

Уровни разрешений SharePoint, заданные для элемента, возвращаются с префиксом SP. Примеры: SP.View Only, SP.Limited Access, SP.View Web Analytics Data. См. [полный список ролей SharePoint](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).

## <a name="example"></a>Пример

В этом примере показано, как получить набор разрешений для элемента в объекте drive пользователя, выполнившего вход в систему.

<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/permissions
```

### <a name="response"></a>Ответ

Этот пример отклика включает три разрешения. Первое разрешение представляет собой ссылку для общего доступа с разрешениями на изменение, второе — явное разрешение для пользователя с именем John, которое унаследовано от родительской папки, а третье разрешение — это ссылка для общего доступа с правами на чтение и запись, созданная приложением.

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "Contoso Time Manager"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a>Замечания

Связи между **разрешениями** ресурса DriveItem невозможно развернуть как часть запроса на [получение DriveItem](driveitem_get.md) или коллекции DriveItems. Необходимо открыть доступ непосредственно к свойству разрешений.

## <a name="error-responses"></a>Ответы с ошибками

Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions"
} -->
