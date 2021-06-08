---
title: 'Filter: clear'
description: Сброс фильтра для определенного столбца.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 6ac9fac0f389efefadeaec3a30eba0b58d851aca
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786993"
---
# <a name="filter-clear"></a>Filter: clear

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сброс фильтра для определенного столбца.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


