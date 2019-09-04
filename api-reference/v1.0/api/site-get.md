---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение сайта SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Получение свойств и отношений ресурса site.
doc_type: apiPageType
ms.openlocfilehash: 102295c12ca5278b40c9540049282db360f7701b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727721"
---
# <a name="get-a-site-resource"></a>Получение ресурса site

Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.

[сайта]: ../resources/site.md

Для обращения к ресурсу **site** используется уникальный идентификатор, при создании которого используются указанные ниже значения.

* имя узла семейства веб-сайтов (contoso.sharepoint.com);
* уникальный идентификатор семейства веб-сайтов (GUID);
* уникальный идентификатор сайта (GUID).

Кроме того, существует зарезервированный идентификатор сайта `root`, который всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.

* `/sites/root`. Корневой сайт клиента.
* `/groups/{group-id}/sites/root`. Сайт группы для ресурса group.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Sites.Read.All, Sites.ReadWrite.All |

## <a name="get-the-tenants-root-site"></a>Получение корневого сайта клиента

Чтобы получить доступ к корневому сайту SharePoint внутри клиента, создайте следующие запросы:

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a>Использование относительного URL-адреса сервера для доступа к сайту

Если у вас есть относительный URL-адрес сервера для ресурса **site**, можно создать следующий запрос:

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a>Доступ к сайту группы для группы

Чтобы получить доступ к сайту группы для группы, создайте следующий запрос:

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID",
  "suppressions": [
  ]
} -->
