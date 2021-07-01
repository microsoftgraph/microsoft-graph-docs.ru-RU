---
title: 'accessReviewScheduleDefinition: filterByCurrentUser'
description: Возвращает объекты accessReviewScheduleDefinition, в которых вызываемая пользователь является рецензентом.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2185e064dcd39049e90063dbcbe1100f9da36344
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209605"
---
# <a name="accessreviewscheduledefinition-filterbycurrentuser"></a>accessReviewScheduleDefinition: filterByCurrentUser
Пространство имен: microsoft.graph

Возвращает [объекты accessReviewScheduleDefinition,](../resources/accessreviewscheduledefinition.md) в которых вызываемая пользователь является рецензентом на одном или более [объектах accessReviewInstance.](../resources/accessreviewinstance.md)

>[!NOTE]
>Размер страницы по умолчанию для этого API — 100 объектов accessReviewScheduleDefinition. Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов. Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)

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
GET /identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')
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

В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте ответа.

## <a name="examples"></a>Примеры
Возвращает все определения обзора, в которых вызываемая пользователь является рецензентом.

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewscheduledefinition_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewscheduledefinition-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewscheduledefinition-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewscheduledefinition-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewscheduledefinition-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewScheduleDefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(accessReviewScheduleDefinition)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
            "id": "66666337-b075-4a92-9d71-255cc4b5d12a",
            "displayName": "All groups review",
            "createdDateTime": "2021-03-09T00:45:51.6272836Z",
            "lastModifiedDateTime": "2021-03-09T00:46:11.2041753Z",
            "status": "InProgress",
            "descriptionForAdmins": "All groups review",
            "descriptionForReviewers": "",
            "createdBy": {
                "id": "cae33dff-88e8-4e02-8a52-de021295997e",
                "displayName": "Example user",
                "userPrincipalName": "exampleuser@contoso.com"
            },
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            "instanceEnumerationScope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            "reviewers": [
                {
                    "query": "./owners",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": null
                }
            ],
            "fallbackReviewers": [],
            "settings": {
                "mailNotificationsEnabled": true,
                "reminderNotificationsEnabled": true,
                "justificationRequiredOnApproval": true,
                "defaultDecisionEnabled": false,
                "defaultDecision": "None",
                "instanceDurationInDays": 3,
                "autoApplyDecisionsEnabled": true,
                "recommendationsEnabled": true,
                "recurrence": {
                    "pattern": {
                        "type": "weekly",
                        "interval": 1,
                        "month": 0,
                        "dayOfMonth": 0,
                        "daysOfWeek": [],
                        "firstDayOfWeek": "sunday",
                        "index": "first"
                    },
                    "range": {
                        "type": "numbered",
                        "numberOfOccurrences": 0,
                        "recurrenceTimeZone": null,
                        "startDate": "2021-03-09",
                        "endDate": "9999-12-31"
                    }
                },
                "applyActions": [
                    {
                        "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                    }
                ]
            },
            "instances": []
        }
    ]
}
```
