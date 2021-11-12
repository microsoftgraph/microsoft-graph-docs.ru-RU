---
author: JeremyKelley
description: Используя действие createLink, вы можете поделиться ресурсом DriveItem с помощью ссылки для совместного доступа.
title: 'driveItem: createLink'
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bfa70cc4deb1062c2efc4d354b8787e9f607a8e9
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944147"
---
# <a name="driveitem-createlink"></a>driveItem: createLink

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете использовать **действие createLink** для общего доступа [к driveItem](../resources/driveitem.md) по ссылке общего доступа.

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
## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса определяются свойства ссылки для совместного доступа, запрашиваемой приложением.
Запрос должен быть объектом JSON с указанными ниже свойствами.

|   Свойство                 |  Тип  |                                 Описание                                                               |
| :----------------------| :----- | :---------------------------------------------------------------------------------------------------------|
|type|String|Optional.The type of sharing link to create.   |
|scope|String|Необязательный параметр. Область создаваемой ссылки. Анонимные, организации или пользователи.|
|expirationDateTime|DateTimeOffset|Необязательный параметр. Строка с форматом yyyy-MM-ddTHH:mm:ssZ dateTime указывает срок действия разрешения.|
|password|Строка|Optional.The password of the sharing link that is set by the creator.|
|recipients|[коллекция driveRecipient](../resources/driverecipient.md)|Необязательный параметр. Коллекция получателей, которые получат доступ к ссылке общего доступа.|

### <a name="link-types"></a>Типы ссылок

Параметр **type** может принимать указанные ниже значения.

| Значение типа | Описание                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| представление           | Создает ссылку только для чтения на **driveItem.**                                                                        |
| обзор         | Создает ссылку на обзор **на driveItem**. Этот параметр доступен только для файлов в OneDrive для бизнеса и SharePoint.                   |
| edit           | Создает ссылку для чтения на **driveItem.**                                                                       |
| Внедрить          | Создает встраивную ссылку на **driveItem.**                                                                      |
| blocksDownload | Создает ссылку только для чтения, которая блокирует загрузку **на driveItem.** Этот параметр доступен только для файлов в OneDrive для бизнеса и SharePoint.  |
| createOnly     | Создает ссылку только для загрузки на **driveItem.** Этот параметр доступен только для папок в OneDrive для бизнеса и SharePoint.             |
| addressBar     | Создает ссылку по умолчанию, которая отображается в барах адресов браузера для вновь созданных файлов. Доступно только в OneDrive для бизнеса и SharePoint. Администратор организации настраивает, поддерживается ли этот тип ссылок и какие функции поддерживаются этим типом ссылок. |
| adminDefault   | Создает по умолчанию ссылку на **driveItem,** определяемую администратором организации. Доступно только в OneDrive для бизнеса и SharePoint. Политика для организации выполняется администратором. |

### <a name="scope-types"></a>Типы областей

Параметр **scope** может принимать указанные ниже значения.

| Значение          | Описание
|:---------------|:------------------------------------------------------------
| анонимный    | Любой пользователь со ссылкой обладает правом доступа без необходимости входа в систему. Это также относится к людям вне вашей организации. Администратор может отключить поддержку ссылок, не требующих проверки подлинности.
| organization | Любой пользователь, вошедший в вашу организацию (клиент), может использовать ссылку для получения доступа. Доступно только в OneDrive для бизнеса и SharePoint.
| users        | Конкретные люди из коллекции получателей могут использовать ссылку для получения доступа. Доступно только в OneDrive для бизнеса и SharePoint.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает в тексте ответа один ресурс [Permission](../resources/permission.md), представляющий запрашиваемые разрешения для совместного доступа.

Ответ будет в том случае, если для driveItem создается новая ссылка общего доступа или возвращается `201 Created`  `200 OK` существующая ссылка.

## <a name="examples"></a>Примеры

### <a name="example-1-create-an-anonymous-sharing-link"></a>Пример 1. Создание анонимной ссылки на общий доступ
В следующем примере запрашивается ссылка общего доступа, которая будет создана для **driveItem,** указанной {itemId} в OneDrive.
Ссылка для совместного доступа подразумевает доступ только для чтения, и ее может использовать каждый, кому она предоставлена.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "driveItem_createlink",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "view",
  "scope": "anonymous",
  "password": "String",
  "recipients": [
    {
      "@odata.type": "microsoft.graph.driveRecipient"
    }
  ]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/driveitem-createlink-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/driveitem-createlink-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/driveitem-createlink-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/driveitem-createlink-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->

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
  },
  "hasPassword": true
}
```

### <a name="example-2-creating-company-sharable-links"></a>Пример 2. Создание sharable ссылок компании

OneDrive для бизнеса и SharePoint поддерживают ссылки с возможностью общего доступа в компании.
Они аналогичны ссылкам, не требующим проверки подлинности, но работают только для элементов соответствующей организации.
Чтобы создать такую ссылку, задайте для параметра **scope** значение `organization`.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create-link-scoped",
  "scopes": "files.readwrite service.sharepoint",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
 } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-scoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

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

### <a name="example-3-creating-embeddable-links"></a>Пример 3. Создание встраивемых ссылок

При использовании типа ссылки `embed` возвращаемое значение webUrl можно внедрять в элемент HTML `<iframe>`. При создании встроенной ссылки свойство `webHtml` содержит HTML-код для объекта `<iframe>`, в котором размещается содержимое.

>**Примечание.** Внедрение ссылок поддерживается только в личных учетных записях OneDrive.

#### <a name="request"></a>Запросить

<!-- {
  "blockType": "request",
  "name": "create-embedded-link",
  "scopes": "files.readwrite service.onedrive",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
} -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-embedded-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

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

## <a name="remarks"></a>Примечания

* Чтобы создать ссылку на основе политики по умолчанию организации и разрешений вызываемого на **driveItem,** ограничьте параметры области и типа
* Срок действия ссылок, созданных с помощью этого действия, не истекает при условии, что в организации не включена политика срока действия.
* Ссылки видны в разрешениях общего доступа для **driveItem** и могут быть удалены владельцем **driveItem.**
* Ссылки всегда указывают на текущую версию **driveItem,** если только **driveItem** не будет проверен (только SharePoint).

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for a driveItem.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->
