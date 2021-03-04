---
title: Список accessReviewScheduleDefinitions
description: Извлечение объектов accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 983ecadb7bf60258ee531ad252c4c67325e97802
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439056"
---
# <a name="list-accessreviewscheduledefinition"></a><span data-ttu-id="d22d7-103">Список accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="d22d7-103">List accessReviewScheduleDefinition</span></span>

<span data-ttu-id="d22d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d22d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d22d7-105">Извлечение [объектов accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d22d7-105">Retrieve the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects.</span></span> <span data-ttu-id="d22d7-106">Возвращается список объектов accessReviewScheduleDefinition, включая все вложенные свойства, для каждой созданной серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="d22d7-106">A list of zero or more accessReviewScheduleDefinition objects are returned, including all of their nested properties, for each access review series created.</span></span> <span data-ttu-id="d22d7-107">Это не включает связанные accessReviewInstances.</span><span class="sxs-lookup"><span data-stu-id="d22d7-107">This does not include associated accessReviewInstances.</span></span>

>[!NOTE]
><span data-ttu-id="d22d7-108">Если возвращается большое количество **accessReviewScheduleDefinitions,** чтобы повысить эффективность и избежать периодов времени, извлекайте результат, заданный на страницах, включив в запрос как параметр $top запроса с размером страницы не более 100, так и параметр запроса $skip=0 в запросе.</span><span class="sxs-lookup"><span data-stu-id="d22d7-108">If many **accessReviewScheduleDefinitions** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="d22d7-109">Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу с свойством @odata.nextLink в ответ, содержащий URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="d22d7-109">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="d22d7-110">Если это свойство присутствует, продолжайте делать дополнительные запросы с URL-адресом @odata.nextLink в каждом ответе, пока не будут возвращены все результаты, как описано в проверке данных Microsoft Graph в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="d22d7-110">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="d22d7-111">Если параметры запроса не предоставлены и результатов более 100, Microsoft Graph автоматически будет предоставлять результаты по 100 результатов на страницу.</span><span class="sxs-lookup"><span data-stu-id="d22d7-111">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>


## <a name="permissions"></a><span data-ttu-id="d22d7-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d22d7-112">Permissions</span></span>
<span data-ttu-id="d22d7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d22d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d22d7-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d22d7-115">Permission type</span></span>                        | <span data-ttu-id="d22d7-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d22d7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d22d7-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d22d7-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="d22d7-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d22d7-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="d22d7-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d22d7-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d22d7-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d22d7-120">Not supported.</span></span>|
|<span data-ttu-id="d22d7-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="d22d7-121">Application</span></span>                            | <span data-ttu-id="d22d7-122">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d22d7-122">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="d22d7-123">В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="d22d7-123">The signed-in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="d22d7-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d22d7-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="d22d7-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d22d7-125">Request headers</span></span>
<span data-ttu-id="d22d7-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="d22d7-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="d22d7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d22d7-127">Request body</span></span>
<span data-ttu-id="d22d7-128">Не поставляем тело запроса.</span><span class="sxs-lookup"><span data-stu-id="d22d7-128">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="d22d7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d22d7-129">Response</span></span>
<span data-ttu-id="d22d7-130">В случае успешной работы этот метод возвращает код отклика и массив `200 OK` [объектов accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d22d7-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d22d7-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d22d7-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="d22d7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d22d7-132">Request</span></span>
<span data-ttu-id="d22d7-133">В следующем примере показан запрос на извлечение всех серий обзоров доступа в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d22d7-133">The following example shows a request to retrieve all the access review series in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="d22d7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d22d7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="d22d7-135">C#</span><span class="sxs-lookup"><span data-stu-id="d22d7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d22d7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d22d7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d22d7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d22d7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d22d7-138">Java</span><span class="sxs-lookup"><span data-stu-id="d22d7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="d22d7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d22d7-139">Response</span></span>
><span data-ttu-id="d22d7-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d22d7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d22d7-142">См. также</span><span class="sxs-lookup"><span data-stu-id="d22d7-142">See also</span></span>

- [<span data-ttu-id="d22d7-143">Получить accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="d22d7-143">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)


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
