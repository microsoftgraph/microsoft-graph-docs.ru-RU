---
title: Решения по списку (из многоступенчатого обзора доступа)
description: Получите решения на этапе в многоступенчатом обзоре доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a188aa60896a31cdde5cdbb6ca7edcf8929cce9d
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63721859"
---
# <a name="list-decisions-from-a-multi-stage-access-review"></a>Решения по списку (из многоступенчатого обзора доступа)
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите решения на этапе в многоступенчатом обзоре доступа. Решения в [объекте accessReviewStage](../resources/accessReviewStage.md) представлены accessReviewInstanceDecisionItem].. объект /resources/accessreviewinstancedecisionitem.md.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.Read.All, AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|AccessReview.Read.All, AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}/decisions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры `$select`запроса , `$filter`, `$orderBy`, и `$skip``$top` OData, чтобы помочь настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

Размер страницы по умолчанию для этого API — 100 **объектов accessReviewStage** . Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов. Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)


## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот `200 OK` метод возвращает код отклика и коллекцию [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_stage_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/16d424f6-0100-4bf1-9ebc-fe009c5e5006/instances/bb14c722-51b8-4962-9bd2-1d96ba773d80/stages/8f0a8999-205b-4c29-a68c-2bee353fd4c5/decisions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-stage-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-stage-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-stage-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-stage-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-stage-accessreviewinstancedecisionitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstanceDecisionItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/16d424f6-0100-4bf1-9ebc-fe009c5e5006/instances/bb14c722-51b8-4962-9bd2-1d96ba773d80/stages/8f0a8999-205b-4c29-a68c-2bee353fd4c5/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "bfbd4d74-275c-4368-aaa1-06c93838d0d5",
            "accessReviewId": "bb14c722-51b8-4962-9bd2-1d96ba773d80",
            "reviewedDateTime": "2021-05-05T16:48:28.79Z",
            "decision": "Deny",
            "justification": "bye alexxxxx",
            "appliedDateTime": "2021-05-05T16:50:30.9Z",
            "applyResult": "AppliedSuccessfully",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/540da31b-4d25-4934-b7f7-98bc230eb15a",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "ff15bedb-22de-49ad-b2d7-59656607484d",
                "displayName": "group owner",
                "userPrincipalName": "group owner"
            },
            "appliedBy": {
                "id": "8798d204-fa3c-4d7b-977d-bc939b8a0848",
                "displayName": "Access Reviews",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "540da31b-4d25-4934-b7f7-98bc230eb15a",
                "userDisplayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "540da31b-4d25-4934-b7f7-98bc230eb15a",
                "displayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            }
        }
    ]
}
```

