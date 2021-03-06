---
title: Обновление accessReviewInstanceDecisionItem
description: Обновление существующего объекта accessReviewInstanceDecisionItem, вызываемого пользователем, является рецензентом.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4322009b4f574e9a32958c25bf65320d4e535435
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439116"
---
# <a name="update-accessreviewinstancedecisionitem"></a>Обновление accessReviewInstanceDecisionItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите решения о доступе, известные как [accessReviewInstanceDecisionItems,](../resources/accessreviewinstancedecisionitem.md)для которых пользователь является рецензентом.

>[!NOTE]
>Любые обновления, сделанные в **accessReviewInstanceDecisionItem,** могут быть сделаны только путем вызова пользователей, которые указаны в качестве рецензента для родительского [accessReviewInstance](../resources/accessreviewinstance.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из следующих разрешений. Делегирование разрешений личным учетным записям Майкрософт не поддерживается. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
|Авторизация|Bearer {токен}. Обязательный.|
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В следующей таблице показаны свойства, принятые для обновления `accessReviewInstanceDecisionItem` .

| Свойство     | Тип       | Описание |
|:-------------|:------------|:------------|
| решение  | String | Решение о доступе для проверяемого объекта. Возможные значения: `Approve` `Deny` `NotReviewed` `DontKnow` . Обязательный.  |
|  обоснование | String | Контекст обзора, предоставленного администраторам. Обязательно, если оправданиеRequiredOnApproval является true на accessReviewScheduleDefinition.  |

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код `204, NoContent` ответа и не возвращает текст ответа.

### <a name="request"></a>Запрос
## <a name="examples"></a>Примеры

Это пример утверждения доступа для пользователя, представленного пользователем `accessReviewInstanceDecisionItem` .


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/654b34e7-b48f-4772-a2d4-08f1d0dd014c

{
  "decision": "Approve",
  "justification": "I trust this person"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
