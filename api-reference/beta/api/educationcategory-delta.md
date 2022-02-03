---
title: 'educationCategory: delta'
description: Получите список вновь созданных или обновленных объектов educationCategory без выполнения полного чтения коллекции.
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6c669a40301df123b3f4c706cb2089eaf3eb3a67
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347717"
---
# <a name="educationcategory-delta"></a>educationCategory: delta
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список вновь созданных или обновленных [объектов educationCategory](../resources/educationcategory.md) без выполнения полного чтения коллекции.

> Этот метод не возвращает удаленные категории.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                                                                         |
| Приложение                            | EduAssignments.ReadBasic.All, EduAssignments.ReadWriteBasic.All, EduAssignments.Read.All, EduAssignments.ReadWrite.All |

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод не поддерживает `$expand`параметры запроса , `$orderby`и `$filter` `$search`OData.

Этот метод поддерживает только параметр `$top` запроса OData.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{educationClassId}/assignmentCategories/delta
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/categories/delta
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы эта функция возвращает код `200 OK` отклика и [коллекцию educationCategory](../resources/educationcategory.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-assignment-categories"></a>Пример 1. Получить категории назначений

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. 

Используйте параметр `$top` , чтобы указать количество возвращаемой категории. Параметр необязательный, но использовать его желательно, если у вас есть длинный список категорий, в противном случае вы получите все категории в классе.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classcategories_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$top=3
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classcategories-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classcategories-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classcategories-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classcategories-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-classcategories-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-classcategories-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

#### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

>**Примечание:** Возьмите ответ `@odata.nextLink` , чтобы сделать еще один вызов и получить следующий набор категорий.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(educationCategory)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$skiptoken=U43TyYWKlRvJ6wWxZOfJvkp22nMqShRw9f-GxBtG2FDy9b1hMDaAJGdLb7n2fh1IVSFtBcXz0jxjIEihcR91dS3R7i8Z2IMtxIn9rKbK9Jvurj6jCH-lDbSNatdesrK0PJ5zpZ_-i8HyqkdtLhWD9tewXVArIqQWJA7gJz8z4paG2q0MU9rixrQOTe7WIXikPiBTUPilHuUW-o1k7cvqke3K7llJbU3G7z_O7WGoVGE.l8-2OcBi9ZWAhwhPnXvJ-kyyk8GNb6-H4o6qofP5YBY",
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "Fall 21",
            "id": "f0fd3e18-87a7-4060-b348-bd2d7a178a9d"
        },
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "reading",
            "id": "10aa7bb1-7f5b-4c12-b1d4-0bf1429a12de"
        },
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "expand",
            "id": "02f60051-806d-4729-a251-4156f7d8e8a5"
        }
    ]
}
```

### <a name="example-2-get-next-set-of-categories"></a>Пример 2. Получить следующий набор категорий 

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

Используйте значение `@odata.nextLink` из предыдущего вызова для этого запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classcategories_delta"
}-->

```msgraph-interactive
GET /education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$skiptoken=U43TyYWKlRvJ6wWxZOfJvkp22nMqShRw9f-GxBtG2FDy9b1hMDaAJGdLb7n2fh1IVSFtBcXz0jxjIEihcR91dS3R7i8Z2IMtxIn9rKbK9Jvurj6jCH-lDbSNatdesrK0PJ5zpZ_-i8HyqkdtLhWD9tewXVArIqQWJA7gJz8z4paG2q0MU9rixrQOTe7WIXikPiBTUPilHuUW-o1k7cvqke3K7llJbU3G7z_O7WGoVGE.l8-2OcBi9ZWAhwhPnXvJ-kyyk8GNb6-H4o6qofP5YBY
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classcategories-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classcategories-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classcategories-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classcategories-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-classcategories-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-classcategories-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание:** Вы должны продолжать использовать значение для `@odata.nextLink` последующих вызовов, пока не получите `@odata.deltaLink` свойство в ответе.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(educationCategory)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$deltatoken=7ORzTfzlUEGDy6BRE3OC-3ePBbvLHCRe4aJ_hjaBKJxUHmn_ODgoM4xreLS7YRaxc-iACeqCQsT5Tb0u9vn6QXYflO6j0sRgRQlhcfR7DApZYl6uZqiXcR7H0G14btPqR761sKWNc0jgiczrHGF6dGfSQwsLzPT46og-84ArhOU.Jnxvkr08FE-QBvEYstYel3JZUrgwgTauo-GmpbdWeSA",
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "apps",
            "id": "62cee656-f3e7-45c9-958f-5dc3ff47dd97"
        },
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "homework",
            "id": "440c56ea-6c2a-4566-a8ab-56fcda3bc1e3"
        }
    ]
}
```

### <a name="example-3-get-the-created-and-modified-categories-using-delta-token"></a>Пример 3. Получить созданные и измененные категории с помощью маркера delta

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

Используйте значение `@odata.deltaLink` из предыдущего вызова для этого запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classcategories_delta"
}-->

```msgraph-interactive
GET /education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$deltatoken=7ORzTfzlUEGDy6BRE3OC-3ePBbvLHCRe4aJ_hjaBKJxUHmn_ODgoM4xreLS7YRaxc-iACeqCQsT5Tb0u9vn6QXYflO6j0sRgRQlhcfR7DApZYl6uZqiXcR7H0G14btPqR761sKWNc0jgiczrHGF6dGfSQwsLzPT46og-84ArhOU.Jnxvkr08FE-QBvEYstYel3JZUrgwgTauo-GmpbdWeSA
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classcategories-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classcategories-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classcategories-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classcategories-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-classcategories-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-classcategories-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание:** Вы должны продолжать использовать, `@odata.deltaLink` чтобы получить недавно созданные или измененные категории с момента первоначального вызова Delta.

>Иногда ответ дельты будет `@odata.nextLink` очень большим, и в этом случае будет возвращено, чтобы продолжить извлечение изменений до тех пор, пока вы не нажметесь снова `@odata.deltaLink` .

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(educationCategory)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$deltatoken=7ORzTfzlUEGDy6BRE3OC-3ePBbvLHCRe4aJ_hjaBKJxUHmn_ODgoM4xreLS7YRaxc-iACeqCQsT5Tb0u9vn6QXYflO6j0sRgRQlhcfR7DApVu5vuUKP3uuUhFpYW8Ku3RtYbkmxRlHbDAkK-NyvPczuDOJqONtesUhKgaoXQGmM.4Rw7IYlmUFBcaDmEbJoGDLMbchYNgoLiPNyp4e7z2po",
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "arts",
            "id": "d9fa9b82-04d5-4411-ae4d-848e6fd75575"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-11-18 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
