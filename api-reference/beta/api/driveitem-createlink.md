---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Предоставление доступа к файлу посредством ссылки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4b4b86621579b945af01eb1dc517b7525220aae8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526223"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a>Создание ссылки совместного доступа для ресурса DriveItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используя действие **createLink**, вы можете поделиться ресурсом [DriveItem](../resources/driveitem.md) с помощью ссылки для совместного доступа.

Действие **createLink** создает ссылку для совместного доступа, если ссылка указанного типа еще не существует для приложения, совершающего вызов. Если для приложения уже создана такая ссылка указанного типа, возвращается она.

Ресурсы DriveItem наследуют разрешения совместного доступа от своих предков.

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
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a>Тело запроса

В теле запроса определяются свойства ссылки для совместного доступа, запрашиваемой приложением.
Запрос должен быть объектом JSON с указанными ниже свойствами.

|   Имя    |  Тип  |                                 Описание                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| **type**  | строка | Тип создаваемой ссылки для совместного доступа. Возможные значения: `view`, `edit` или `embed`.       |
| **scope** | string | Необязательный параметр. Область создаваемой ссылки. Возможные значения: `anonymous` или `organization`. |


### <a name="link-types"></a>Типы ссылок

Параметр **type** может принимать указанные ниже значения.

| Значение типа | Описание                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | Создает ссылку на объект DriveItem, предполагающую доступ только для чтения.                                                        |
| `edit`     | Создает ссылку на объект DriveItem, предполагающую доступ для чтения и записи.                                                       |
| `embed`    | Создает встраиваемую ссылку на объект DriveItem. Этот вариант доступен только для файлов в личных учетных записях OneDrive. |

### <a name="scope-types"></a>Типы областей

Параметр **scope** может принимать указанные ниже значения.
Если параметр **scope** не задан, создается ссылка того типа, который используется в организации по умолчанию.

| Значение типа     | Описание                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | Создает ссылку на объект DriveItem, доступный всем, кому она предоставлена. Администратор может отключить ссылки, не требующие проверки подлинности.                 |
| `organization` | Создает ссылку на объект DriveItem, доступный всем в организации пользователя. Область организации для ссылок недоступна в личных учетных записях OneDrive. |

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает в тексте ответа один ресурс [Permission](../resources/permission.md), представляющий запрашиваемые разрешения для совместного доступа.

Если для элемента создается новая ссылка совместного доступа, возвращается код ответа `201 Created`, а если возвращается существующая ссылка — код `200 OK`.

## <a name="example"></a>Пример

В приведенном ниже примере запрашивается создание ссылки для совместного доступа к объекту DriveItem, указанному по {itemId}, в хранилище OneDrive пользователя.
Ссылка для совместного доступа подразумевает доступ только для чтения, и ее может использовать каждый, кому она предоставлена.

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

### <a name="response"></a>Ответ

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a>Создание ссылок с возможностью общего доступа в компании

OneDrive для бизнеса и SharePoint поддерживают ссылки с возможностью общего доступа в компании.
Они аналогичны ссылкам, не требующим проверки подлинности, но работают только для элементов соответствующей организации.
Чтобы создать такую ссылку, задайте для параметра **scope** значение `organization`.

### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a>Ответ

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-embeddable-links"></a>Создание встраиваемых ссылок

При использовании типа ссылки `embed` возвращаемое значение webUrl можно внедрять в элемент HTML `<iframe>`. При создании встроенной ссылки свойство `webHtml` содержит HTML-код для объекта `<iframe>`, в котором размещается содержимое.

**Примечание.** Внедрение ссылок поддерживается только в личных учетных записях OneDrive.

### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a>Ответ

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a>Замечания

* Срок действия ссылок, созданных с помощью этого действия, не истекает при условии, что в организации не включена политика срока действия.
* Ссылки отображаются в разрешениях на совместное использование для элемента и могут быть удалены владельцем элемента.
* Они всегда указывают на текущую версию элемента, если он не был извлечен (только в SharePoint).

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
