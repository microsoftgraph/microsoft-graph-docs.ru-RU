---
title: Список решений
description: Получите ресурсы accessReviewInstanceDecisionItem из свойства навигации решений.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 74de88c1e14e9983580a80c1c1698842eaddc8f9
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031504"
---
# <a name="list-decisions"></a>Список решений
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите [объекты accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) из решений [по accessReviewInstance.](../resources/accessreviewinstance.md)

>[!NOTE]
>Размер страницы по умолчанию для этого API — 100 объектов accessReviewInstance. Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов. Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.Read.All, AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|AccessReview.Read.All, AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает `$select` `$filter` параметры запроса `$orderBy` `$skip` `$top` OData и OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/16d424f6-0100-4bf1-9ebc-fe009c5e5006/instances/bb14c722-51b8-4962-9bd2-1d96ba773d80/decisions
```


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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('16d424f6-0100-4bf1-9ebc-fe009c5e5006')/instances('bb14c722-51b8-4962-9bd2-1d96ba773d80')/decisions",
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
