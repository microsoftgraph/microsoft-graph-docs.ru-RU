---
author: swapnil1993
title: Получить columnDefinition
description: Получите сайт, список или столбец типа контента.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6c592c378d035cf3f16eef9e2cfe7769cb257649
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730139"
---
# <a name="get-columndefinition"></a>Получить columnDefinition
Пространство имен: microsoft.graph


Извлечение метаданных для [сайта,][] [списка][]или [столбца contentType.][] [][columnDefinition]

  

## <a name="permissions"></a>Разрешения

  

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

  

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All  |

  

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /sites/{site-id}/columns/{column-id}
GET /sites/{site-id}/lists/{list-id}/columns/{column-id}
GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|  

## <a name="request-body"></a>Тело запроса

  

Не указывайте текст запроса для этого метода.

  

## <a name="example"></a>Пример

  

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get_column_from_contenttype" } -->

  

```msgraph-interactive
GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-column-from-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-column-from-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-column-from-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-column-from-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

  

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
  "readOnly": false,
  "required": false,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md

[list]: ../resources/list.md

[site]: ../resources/site.md

[contentType]: ../resources/contentType.md
  
