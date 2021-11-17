---
title: Get administrativeUnit
description: Извлечение простого **административного каталогаUnit,** соответствующего этому **educationSchool.**
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9ec9e392e106a503916188cc2b7a08c292e15cef
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975173"
---
# <a name="get-administrativeunit"></a>Get administrativeUnit

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение простого **административного каталогаUnit,** соответствующего этому **educationSchool.**

>**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях. В данном случае используйте ресурс `...beta/education/me/schools`.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется сочетание разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All|
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All| 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/administrativeUnit
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [administrativeUnit](../resources/administrativeunit.md) в тексте ответа.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_administrativeUnit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-get-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/educationschool-get-administrativeunit-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

<!-- uuid: A681726F-B4A7-4BCF-9407-F87CB9A4771D
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


