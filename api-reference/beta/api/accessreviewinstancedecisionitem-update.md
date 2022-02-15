---
title: Обновление accessReviewInstanceDecisionItem
description: Обновите существующий объект accessReviewInstanceDecisionItem, для которого вызываемая пользователь является рецензентом.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9b3e75d9817b2e41a332d0138dc409301d58f4e1
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "62815856"
---
# <a name="update-accessreviewinstancedecisionitem"></a>Обновление accessReviewInstanceDecisionItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите решения о доступе, известные как [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), для которых пользователь является рецензентом.

>[!NOTE]
>Любые обновления, сделанные в **accessReviewInstanceDecisionItem** , могут быть сделаны только путем вызова пользователей, перечисленных в качестве рецензента для родительского [accessReviewInstance](../resources/accessreviewinstance.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из следующих разрешений. Делегирование разрешений личным учетным записям Майкрософт не поддерживается. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

Чтобы обновить решение о accessReviewInstance:
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

Обновление решения на этапе accessReviewInstance с несколькими этапами:
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
| Авторизация|Bearer {token}. Обязательный.|
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В следующей таблице показаны свойства, принятые для обновления `accessReviewInstanceDecisionItem`.

| Свойство     | Тип       | Описание |
|:-------------|:------------|:------------|
| решение  | Строка | Решение о доступе для проверяемого объекта. Возможные значения: `Approve` `NotReviewed` `Deny` `DontKnow`. Обязательный элемент.  |
|  обоснование | String | Контекст обзора, предоставленного администраторам. Обязательно, если оправданиеRequiredOnApproval является true на accessReviewScheduleDefinition.  |

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код `204 No Content` ответа и не возвращает текст ответа.


## <a name="examples"></a>Примеры

### <a name="example-1-update-a-decision-on-an-accessreviewinstance"></a>Пример 1. Обновление решения о accessReviewInstance

#### <a name="request"></a>Запрос

Ниже приводится пример решения об утверждении доступа для пользователя.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-accessreviewinstancedecisionitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 Accepted
```


### <a name="example-2-update-a-decision-on-an-stage-in-a-multi-stage-access-review"></a>Пример 2. Обновление решения на этапе в многоэтансовом обзоре доступа

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
Content-Type: application/json

{
  "decision": "Approve",
  "justification": "This person is still on my team",
}
```

#### <a name="response"></a>Отклик

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
