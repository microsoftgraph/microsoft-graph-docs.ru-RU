---
title: 'accessReviewInstanceDecisionItem: filterByCurrentUser'
description: Извлечение всех элементов решений в экземпляре обзора доступа или стадии экземпляра многоступенчатого обзора доступа, для которого вызываемого пользователя является рецензентом.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d75c344b21d04fb9d6af130e0387f374861a611d
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722085"
---
# <a name="accessreviewinstancedecisionitem-filterbycurrentuser"></a>accessReviewInstanceDecisionItem: filterByCurrentUser
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение всех элементов решений в экземпляре обзора доступа или стадии экземпляра многоступенчатого обзора доступа, для которого вызываемого пользователя является рецензентом. Элементы решений представляются [объектами accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) на заданном [accessReviewInstance](../resources/accessreviewinstance.md) или [accessReviewStage](../resources/accessReviewStage.md) , для которых вызываемая пользователь является рецензентом.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.Read.All, AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|AccessReview.Read.All, AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

Для получения решений для экземпляра обзора доступа, для которого вызываемая пользователь является рецензентом:
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/filterByCurrentUser(on='reviewer')
```

Извлечение решений для этапа в экземпляре обзора доступа, для которого вызываемая пользователь является рецензентом:
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}/decisions/filterByCurrentUser(on='reviewer')
```

>[!NOTE]
>Рецензенты многоэтапных обзоров могут извлекать решения на предыдущих этапах, если свойство **decisionHistoriesForReviewersEnabled** включено [](../resources/accessreviewschedulesettings.md) в параметрах [объекта accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).

## <a name="function-parameters"></a>Параметры функции
В следующей таблице показаны параметры запроса, которые можно использовать с помощью этого метода.

|Параметр|Тип|Описание|
|:---|:---|:---|
|on|accessReviewInstanceDecisionItemFilterByCurrentUserOptions|Фильтр для запроса объектов принятия решений для текущего пользователя. Возможные значения : `reviewer`. `unknownFutureValue` Использование `reviewer`. Обязательно.|


## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры `$select`запроса , `$filter`, `$orderBy`, и `$skip``$top` OData, чтобы помочь настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

Размер страницы по умолчанию для этого API — 100 **объектов accessReviewInstanceDecisionItem** . Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов. Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной `200 OK` работы эта функция возвращает код ответа и [коллекцию accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-retrieve-all-decisions-on-an-accessreviewinstance-for-which-the-calling-user-is-the-reviewer"></a>Пример 1. Извлечение всех решений по accessReviewInstance, для которого вызываемая пользователь является рецензентом

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstancedecisionitem_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-5678-ae36-41b923c3bf87/decisions/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstancedecisionitem-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstancedecisionitem-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstancedecisionitem-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstancedecisionitem-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accessreviewinstancedecisionitem-filterbycurrentuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstanceDecisionItem)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
            "id": "139166ec-d214-4835-95aa-3c1d89581e51",
            "accessReviewId": "8d035c9d-798d-47fa-beb4-f986a4b8126f",
            "reviewedDateTime": "2021-05-03T19:28:25.02Z",
            "decision": "Approve",
            "justification": "Christie still needs access to the Marketing group as she works in the Marketing organization.",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "36c4c56e-fce3-4e2d-b28e-4ac0c7d2fa10",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "userDisplayName": "Christie Cline",
                "userPrincipalName": "ChristieC@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "displayName": "Christie Cline",
                "userPrincipalName": "ChristieC@contoso.com"
            }
        }
    ]
}
```

### <a name="example-2-retrieve-all-decisions-on-an-accessreviewstage-of-a-multi-stage-access-review-for-which-the-calling-user-is-the-reviewer"></a>Пример 2. Извлечение всех решений по accessReviewStage многоэтапного обзора доступа, для которого вызываемого пользователя является рецензентом

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstancedecisionitem_filterbycurrentuser_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-5678-ae36-41b923c3bf87/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstancedecisionitem-filterbycurrentuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstancedecisionitem-filterbycurrentuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstancedecisionitem-filterbycurrentuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstancedecisionitem-filterbycurrentuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accessreviewinstancedecisionitem-filterbycurrentuser-2-go-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstanceDecisionItem)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
            "id": "139166ec-d214-4835-95aa-3c1d89581e51",
            "accessReviewId": "8d035c9d-798d-47fa-beb4-f986a4b8126f",
            "reviewedDateTime": "2021-05-03T19:28:25.02Z",
            "decision": "Approve",
            "justification": "Christie still needs access to the Marketing group as she works in the Marketing organization.",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "36c4c56e-fce3-4e2d-b28e-4ac0c7d2fa10",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "userDisplayName": "Christie Cline",
                "userPrincipalName": "ChristieC@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "displayName": "Christie Cline",
                "userPrincipalName": "ChristieC@contoso.com"
            }
        }
    ]
}
```
