---
title: Удаление рецензента accessReview
description: Удаление рецензента обзоров доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 83f136a3a9c131d5a05df92df2f3c3e3d3b6c75c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439317"
---
# <a name="remove-accessreview-reviewer"></a>Удаление рецензента accessReview

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) обновите существующий объект [accessReview,](../resources/accessreview.md) чтобы удалить пользователя в качестве рецензента.  Эта операция разрешена только для еще не завершенного обзора доступа и только для проверки доступа, в которой явно указаны рецензенты. Эта операция не разрешается для проверки доступа, в которой пользователи рассматривают собственный доступ, и не предназначена для проверки доступа, в которой владельцы групп назначены в качестве рецензентов. 


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение                            | AccessReview.ReadWrite.Membership |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}/reviewers/{userId}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Тело запроса
Не следует поставлять тело запроса.


## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа из 200 серий.

## <a name="example"></a>Пример

Это пример обновления разового (не повторяемого) обзора доступа, чтобы удалить ненужный рецензент.


##### <a name="request"></a>Запрос
В URL-адрес запроса поставляют id объекта accessReview, а затем id объекта пользователя.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


