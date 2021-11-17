---
title: Обновление accessReviewInstanceDecisionItem
description: Обновление существующего объекта accessReviewInstanceDecisionItem, вызываемого пользователем, является рецензентом.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c83ebbe6b79f987e8c7d523114dd31e570f155df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987726"
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
|Авторизация|Bearer {token}. Обязательный.|
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В следующей таблице показаны свойства, принятые для обновления `accessReviewInstanceDecisionItem` .

| Свойство     | Тип       | Описание |
|:-------------|:------------|:------------|
| решение  | String | Решение о доступе для проверяемого объекта. Возможные значения: `Approve` `Deny` `NotReviewed` `DontKnow` . Обязательный.  |
|  обоснование | Строка | Контекст обзора, предоставленного администраторам. Обязательно, если оправданиеRequiredOnApproval является true на accessReviewScheduleDefinition.  |

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
``` http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/12348410-67f3-4d4c-b946-6989e050be19
Content-Type: application/json

{
  "decision": "Approve",
  "justification": "This person is still on my team",
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

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-accessreviewinstancedecisionitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response"
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
