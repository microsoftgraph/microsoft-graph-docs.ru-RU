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
# <a name="list-accessreviewscheduledefinition"></a><span data-ttu-id="5afa5-103">Список accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="5afa5-103">List accessReviewScheduleDefinition</span></span>

<span data-ttu-id="5afa5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5afa5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5afa5-105">[Извлечение объектов accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5afa5-105">Retrieve the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects.</span></span> <span data-ttu-id="5afa5-106">Для каждого созданного ряда проверки доступа возвращается список объектов accessReviewScheduleDefinition, включая все их вложенные свойства.</span><span class="sxs-lookup"><span data-stu-id="5afa5-106">A list of zero or more accessReviewScheduleDefinition objects are returned, including all of their nested properties, for each access review series created.</span></span> <span data-ttu-id="5afa5-107">Это не включает связанные accessReviewInstances.</span><span class="sxs-lookup"><span data-stu-id="5afa5-107">This does not include associated accessReviewInstances.</span></span>

>[!NOTE]
><span data-ttu-id="5afa5-108">Если возвращается большое количество **accessReviewScheduleDefinitions,** для повышения эффективности и предотвращения времени выполнения, извлекать набор результатов на страницах, включив в запрос как параметр запроса $top с размером страницы не более 100, так и параметр $skip=0 запроса.</span><span class="sxs-lookup"><span data-stu-id="5afa5-108">If many **accessReviewScheduleDefinitions** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="5afa5-109">Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу со свойством @odata.nextLink в отклике, содержа содержам URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="5afa5-109">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="5afa5-110">Если это свойство присутствует, продолжайте делать дополнительные запросы с URL-адресом @odata.nextLink в каждом ответе, пока не будут возвращены все результаты, как описано в разгонах данных Microsoft Graph в приложении.</span><span class="sxs-lookup"><span data-stu-id="5afa5-110">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="5afa5-111">Если параметры запроса не заданы и имеется более 100 результатов, Microsoft Graph автоматически размещает результаты по 100 результатов на страницу.</span><span class="sxs-lookup"><span data-stu-id="5afa5-111">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>


## <a name="permissions"></a><span data-ttu-id="5afa5-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5afa5-112">Permissions</span></span>
<span data-ttu-id="5afa5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5afa5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5afa5-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5afa5-115">Permission type</span></span>                        | <span data-ttu-id="5afa5-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5afa5-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5afa5-117">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5afa5-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="5afa5-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5afa5-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="5afa5-119">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5afa5-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5afa5-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5afa5-120">Not supported.</span></span>|
|<span data-ttu-id="5afa5-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="5afa5-121">Application</span></span>                            | <span data-ttu-id="5afa5-122">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5afa5-122">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="5afa5-123">Во входе пользователя также должна быть роль каталога, которая позволяет им прочитать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="5afa5-123">The signed-in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="5afa5-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5afa5-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="5afa5-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5afa5-125">Request headers</span></span>
<span data-ttu-id="5afa5-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="5afa5-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="5afa5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5afa5-127">Request body</span></span>
<span data-ttu-id="5afa5-128">Не укажив тело запроса.</span><span class="sxs-lookup"><span data-stu-id="5afa5-128">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="5afa5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5afa5-129">Response</span></span>
<span data-ttu-id="5afa5-130">В случае успеха этот метод возвращает код отклика и массив объектов `200 OK` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5afa5-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5afa5-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5afa5-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="5afa5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5afa5-132">Request</span></span>
<span data-ttu-id="5afa5-133">В следующем примере показан запрос на извлечение всех серии отзывов о доступе в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5afa5-133">The following example shows a request to retrieve all the access review series in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="5afa5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5afa5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="5afa5-135">C#</span><span class="sxs-lookup"><span data-stu-id="5afa5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5afa5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5afa5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5afa5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5afa5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5afa5-138">Java</span><span class="sxs-lookup"><span data-stu-id="5afa5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="5afa5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5afa5-139">Response</span></span>
><span data-ttu-id="5afa5-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5afa5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5afa5-142">См. также</span><span class="sxs-lookup"><span data-stu-id="5afa5-142">See also</span></span>

- [<span data-ttu-id="5afa5-143">Get accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="5afa5-143">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)


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
