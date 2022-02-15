---
title: Get accessReviewInstanceDecisionItem
description: Ознакомьтесь с свойствами и отношениями объекта accessReviewInstanceDecisionItem.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 5884841a3e169f0640fe09adb8237bf64816e497
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "62815890"
---
# <a name="get-accessreviewinstancedecisionitem"></a>Get accessReviewInstanceDecisionItem
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.Read.All, AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|AccessReview.Read.All, AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

Чтобы получить решение по accessReviewInstance:
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

Чтобы получить решение на этапе accessReviewInstance:

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметр `$select` запроса OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной `200 OK` работы этот метод возвращает код ответа и [объект accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-retrieve-a-decision-on-an-accessreviewinstance"></a>Пример 1. Извлечение решения по accessReviewInstance

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accessreviewinstancedecisionitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0')/instances('6444d4fd-ab55-4608-8cf9-c6702d172bcc')/decisions/$entity",
    "id": "e6cafba0-cbf0-4748-8868-0810c7f4cc06",
    "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
    "reviewedDateTime": null,
    "decision": "NotReviewed",
    "justification": "",
    "appliedDateTime": null,
    "applyResult": "New",
    "recommendation": "Approve",
    "principalLink": "https://graph.microsoft.com/v1.0/users/04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
    "resourceLink": null,
    "resource": null,
    "reviewedBy": {
        "id": "00000000-0000-0000-0000-000000000000",
        "displayName": "",
        "userPrincipalName": ""
    },
    "appliedBy": {
        "id": "00000000-0000-0000-0000-000000000000",
        "displayName": "",
        "userPrincipalName": ""
    },
    "target": {
        "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
        "userId": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
        "userDisplayName": "Diego Siciliani",
        "userPrincipalName": "DiegoS@contoso.com"
    },
    "principal": {
        "@odata.type": "#microsoft.graph.userIdentity",
        "id": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
        "displayName": "Diego Siciliani",
        "userPrincipalName": "DiegoS@contoso.com"
    }
}
```

### <a name="example-2-retrieve-a-decision-from-a-stage-of-a-multi-stage-access-review"></a>Пример 2. Извлечение решения на этапе многоэтансного обзора доступа

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_accessreviewstage_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
```

#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/$entity",
    "id": "e6cafba0-cbf0-4748-8868-0810c7f4cc06",
    "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
    "reviewedDateTime": null,
    "decision": "NotReviewed",
    "justification": "",
    "appliedDateTime": null,
    "applyResult": "New",
    "recommendation": "Approve",
    "principalLink": "https://graph.microsoft.com/v1.0/users/04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
    "resourceLink": null,
    "resource": null,
    "reviewedBy": {
        "id": "00000000-0000-0000-0000-000000000000",
        "displayName": "",
        "userPrincipalName": ""
    },
    "appliedBy": {
        "id": "00000000-0000-0000-0000-000000000000",
        "displayName": "",
        "userPrincipalName": ""
    },
    "target": {
        "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
        "userId": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
        "userDisplayName": "Diego Siciliani",
        "userPrincipalName": "DiegoS@contoso.com"
    },
    "principal": {
        "@odata.type": "#microsoft.graph.userIdentity",
        "id": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
        "displayName": "Diego Siciliani",
        "userPrincipalName": "DiegoS@contoso.com"
    }
}
```
