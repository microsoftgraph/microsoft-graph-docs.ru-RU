---
title: 'listItem: createLink'
description: Создание ссылки для обмена listItem
author: learafa
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b0d490139763e619a151e3152868f98c1f1b96e4
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941583"
---
# <a name="listitem-createlink"></a>listItem: createLink

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте ссылку общего доступа для [listItem.](../resources/listitem.md)

Действие **createLink** создает новую ссылку общего доступа, если указанный тип ссылки еще не существует для вызываемого приложения.
Если для приложения уже существует ссылка общего доступа указанного типа, это действие возвращает существующую ссылку общего доступа.

**ресурсы listItem** наследуют разрешения на совместное использование [из списка,](../resources/list.md) в который находится элемент.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из следующих разрешений. Дополнительные дополнительные информации, в том числе о выборе разрешений, см. [в см. в .](/graph/permissions-reference)

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All    |
|Для приложений | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Основной текст запроса
В теле запроса укажи JSON представление параметров.

В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.

|   Свойство             |  Тип  |           Описание                        |
| :----------------------| :----- | :--------------------------------------------|
|type|Строка|Тип создаваемой ссылки для совместного доступа. Необязательно. |
|scope|String|Область создаваемой ссылки. Либо `anonymous` , `organization` или `users` . Необязательно. |
|expirationDateTime|DateTimeOffset|Строка с форматом yyyy-MM-ddTHH:mm:ssZ dateTime указывает срок действия разрешения. Необязательно. |
|password|Строка|Пароль ссылки общего доступа, за устанавливаемой создателем. Необязательно. |
|recipients|[коллекция driveRecipient](../resources/driverecipient.md)|Коллекция получателей, которые получат доступ к ссылке общего доступа. Необязательно. |

### <a name="link-types"></a>Типы ссылок

Параметр **type** может принимать указанные ниже значения.

| Значение типа | Описание                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| представление           | Создает ссылку на элемент, предполагающую доступ только для чтения.                                                                        |
| обзор         | Создает ссылку на обзор элемента. Этот параметр доступен только для файлов в OneDrive для бизнеса и SharePoint.                   |
| edit           | Создает ссылку на элемент для чтения.                                                                       |
| Внедрить          | Создает встроенную ссылку на элемент.                                                                      |
| blocksDownload | Создает ссылку только для чтения, которая блокирует загрузку элемента. Этот параметр доступен только для файлов в OneDrive для бизнеса и SharePoint.  |
| createOnly     | Создает ссылку на элемент только для загрузки. Этот параметр доступен только для папок в OneDrive для бизнеса и SharePoint.             |
| addressBar     | Создает ссылку по умолчанию, которая отображается в барах адресов браузера для вновь созданных файлов. Доступно только в OneDrive для бизнеса и SharePoint. Администратор организации настраивает, поддерживается ли этот тип ссылок и какие функции поддерживаются этим типом ссылок. |
| adminDefault   | Создает ссылку по умолчанию на элемент, определяемую администратором организации. Доступно только в OneDrive для бизнеса и SharePoint. Политика для организации выполняется администратором. |

### <a name="scope-types"></a>Типы областей

Параметр **scope** может принимать указанные ниже значения.

| Значение          | Описание
|:---------------|:------------------------------------------------------------
| анонимный    | Любой пользователь со ссылкой обладает правом доступа без необходимости входа в систему. Это также относится к людям вне вашей организации. Администратор может отключить поддержку ссылок, не требующих проверки подлинности.
| organization; | Любой пользователь, вошедший в вашу организацию (клиент), может использовать ссылку для получения доступа. Доступно только в OneDrive для бизнеса и SharePoint.
| users        | Конкретные люди из коллекции получателей могут использовать ссылку для получения доступа. Доступно только в OneDrive для бизнеса и SharePoint.

## <a name="response"></a>Отклик

В случае успешного использования [](../resources/permission.md) этот метод возвращает один ресурс разрешений в органе отклика, который представляет запрашиваемую для обмена разрешениями.

Ответ будет, если для listItem создается новая ссылка общего доступа или возвращается `201 Created` `200 OK` существующая ссылка.

## <a name="examples"></a>Примеры

### <a name="example-1-create-an-anonymous-sharing-link"></a>Пример 1. Создание анонимной ссылки на общий доступ
В следующем примере запрашивается ссылка общего доступа, которая будет создана для listItem, указанного {itemId} в указанном списке {listId}.
Ссылка для совместного доступа подразумевает доступ только для чтения, и ее может использовать каждый, кому она предоставлена.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json
Content-length: 212

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

#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
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
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

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
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

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

* Чтобы создать ссылку на основе политики по умолчанию организации и разрешений вызываемого в listItem, ограничьте параметры области и типа
* Срок действия ссылок, созданных с помощью этого действия, не истекает при условии, что в организации не включена политика срока действия.
* Ссылки видны в разрешениях общего доступа для listItem и могут быть удалены владельцем listItem.
* Ссылки всегда указывают на текущую версию listItem, если только listItem не будет SharePoint).

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an listItem.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->