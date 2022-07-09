---
title: Обновление accessReviewInstanceDecisionItem
description: Обновите существующий объект accessReviewInstanceDecisionItem, для которого вызывающий пользователь является рецензентом.
ms.localizationpriority: medium
author: zhusijia26
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e0cf1034cbf8e1a8fbfcfd5d73568431a2ca75de
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697122"
---
# <a name="update-accessreviewinstancedecisionitem"></a>Обновление accessReviewInstanceDecisionItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите решения о доступе, известные как [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), для которых пользователь является рецензентом.

>[!NOTE]
>Любые обновления **accessReviewInstanceDecisionItem** могут быть внесены только путем вызова пользователей, перечисленных в качестве рецензента для родительского [объекта accessReviewInstance](../resources/accessreviewinstance.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из следующих разрешений. Делегированные разрешения для личных учетных записей Майкрософт не поддерживаются. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

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

Чтобы обновить решение на этапе accessReviewInstance с несколькими этапами:
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
| Авторизация|Bearer {token}. Обязательный.|
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Основной текст запроса
В следующей таблице показаны свойства, принятые для обновления `accessReviewInstanceDecisionItem`.

| Свойство     | Тип       | Описание |
|:-------------|:------------|:------------|
| Решение  | Строка | Решение о доступе для проверяемой сущности. Возможные значения: `Approve` `NotReviewed` `Deny` `DontKnow`. Обязательный элемент.  |
|  Обоснование | String | Контекст проверки, предоставленной администраторам. Требуется, если для свойства accessReviewScheduleDefinition свойство justificationRequiredOnApproval имеет значение True.  |

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `204 No Content` отклика без текста ответа.


## <a name="examples"></a>Примеры

### <a name="example-1-update-a-decision-on-an-accessreviewinstance"></a>Пример 1. Обновление решения о accessReviewInstance

#### <a name="request"></a>Запрос

Ниже приведен пример решения об утверждении доступа для пользователя.



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


### <a name="example-2-update-a-decision-on-an-stage-in-a-multi-stage-access-review"></a>Пример 2. Обновление решения на этапе многоэтабной проверки доступа

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
