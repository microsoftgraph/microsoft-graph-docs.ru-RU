---
author: swapnil1993
title: Get contentType
description: Получите тип контента на сайте или в списке.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 4f0886b63061a6996dda7559b3c53ce6187d0486
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101361"
---
# <a name="get-contenttype"></a>Get contentType
Пространство имен: microsoft.graph



Извлечение метаданных для типа [контента][contentType] на [сайте][] или в [списке.][]

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes/{contentType-id}

GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект contentType](../resources/contenttype.md) в тексте ответа.


## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contenttype"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/{contentType-id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-contenttype-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-contenttype-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id":"0x0120D520",
  "description":"Create a document set when you want to manage multiple documents as a single work product.",
  "group":"Document Set Content Types",
  "hidden":false,
  "name":"Document Set",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```

[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
[list]: ../resources/list.md
