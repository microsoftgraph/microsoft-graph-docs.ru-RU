---
title: Список accessReviewScheduleDefinitions
description: Извлечение объектов accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 71eaf61e43a145b809da34854fc33975eb459c81
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981006"
---
# <a name="list-accessreviewscheduledefinition"></a>Список accessReviewScheduleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Извлечение объектов accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md) Для каждого созданного ряда проверки доступа возвращается список объектов accessReviewScheduleDefinition, включая все их вложенные свойства. Это не включает связанные accessReviewInstances.

>[!NOTE]
>Если возвращается большое количество **accessReviewScheduleDefinitions,** для повышения эффективности и предотвращения времени выполнения, извлекать набор результатов на страницах, включив в запрос как параметр запроса $top с размером страницы не более 100, так и параметр $skip=0 запроса. Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу со свойством @odata.nextLink в отклике, содержа содержам URL-адрес следующей страницы результатов. Если это свойство присутствует, продолжайте делать дополнительные запросы с URL-адресом @odata.nextLink в каждом ответе, пока не будут возвращены все результаты, как описано в разгонах данных Microsoft Graph в приложении.
>
>Если параметры запроса не заданы и имеется более 100 результатов, Microsoft Graph автоматически размещает результаты по 100 результатов на страницу.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись)     | AccessReview.Read.All, AccessReview.ReadWrite.All  |
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение                            | AccessReview.Read.All, AccessReview.ReadWrite.All |

 Во входе пользователя также должна быть роль каталога, которая позволяет им прочитать проверку доступа.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a>Заголовки запросов
Нет.

## <a name="request-body"></a>Текст запроса
Не укажив тело запроса.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и массив объектов `200 OK` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте отклика.

## <a name="examples"></a>Примеры
### <a name="request"></a>Запрос
В следующем примере показан запрос на извлечение всех серии отзывов о доступе в клиенте.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "id": "98dcebed-c7f6-46f4-bcf3-4a3fccdb3e2a",
            "displayName": "Access Review",
            "createdDateTime": "2020-09-09T14:27:59Z",
            "lastModifiedDateTime": "2020-09-11T12:02:50Z",
            "status": "InProgress",
            "descriptionForAdmins": "",
            "descriptionForReviewers": "",
            "createdBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "admin@contoso.com"
            },
            "scope": {
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b",
                "queryType": "MicrosoftGraph"
            },
            "reviewers": [
                {
                    "query": "./manager",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": "decisions"
                }
            ],
            "settings": {
                "mailNotificationsEnabled": true,
                "reminderNotificationsEnabled": true,
                "justificationRequiredOnApproval": true,
                "defaultDecisionEnabled": false,
                "defaultDecision": "None",
                "instanceDurationInDays": 0,
                "autoApplyDecisionsEnabled": false,
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
                        "startDate": "2020-09-11",
                        "endDate": "9999-12-31"
                    }
                }
            }
        }
    ]
}
```

## <a name="see-also"></a>См. также

- [Get accessReviewScheduleDefinition](accessreviewscheduledefinition-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
