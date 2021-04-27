---
title: 'accessReviewInstance: pendingAccessReviewInstances'
description: Извлечение объектов accessReviewInstance до утверждения с помощью вызова пользователя.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 581ade7ffd620a105dfbb2e6f5c8e9854aab76dc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048416"
---
# <a name="accessreviewinstance-pendingaccessreviewinstances"></a><span data-ttu-id="39ba9-103">accessReviewInstance: pendingAccessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="39ba9-103">accessReviewInstance: pendingAccessReviewInstances</span></span>

<span data-ttu-id="39ba9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39ba9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39ba9-105">Извлечение [объектов accessReviewInstance](../resources/accessreviewinstance.md) до утверждения пользователем вызова.</span><span class="sxs-lookup"><span data-stu-id="39ba9-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects pending approval by the calling user.</span></span> <span data-ttu-id="39ba9-106">Возвращается список нулевых или более объектов accessReviewInstance, из которых пользователем вызова является назначен рецензент.</span><span class="sxs-lookup"><span data-stu-id="39ba9-106">A list of zero or more accessReviewInstance objects are returned, of which the calling user is an assigned reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="39ba9-107">Если возвращается большое количество **accessReviewInstances,** чтобы повысить эффективность и избежать периодов времени, извлекайте результат, заданный на страницах, включив в запрос как параметр $top запроса с размером страницы не более 100, так и параметр запроса $skip=0 в запросе.</span><span class="sxs-lookup"><span data-stu-id="39ba9-107">If many **accessReviewInstances** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="39ba9-108">Если набор результатов охватывает несколько страниц, корпорация Майкрософт Graph возвращает эту страницу с свойством @odata.nextLink в ответе, который содержит URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="39ba9-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="39ba9-109">Если это свойство присутствует, продолжайте делать дополнительные запросы с URL-адресом @odata.nextLink в каждом ответе, пока не будут возвращены все результаты, как описано в Graph данных Microsoft в приложении.</span><span class="sxs-lookup"><span data-stu-id="39ba9-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="39ba9-110">Если параметры запроса не предоставлены и результатов более 100, microsoft Graph автоматически будет предоставлять результаты по 100 результатов на странице.</span><span class="sxs-lookup"><span data-stu-id="39ba9-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="39ba9-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39ba9-111">Permissions</span></span>
<span data-ttu-id="39ba9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39ba9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39ba9-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39ba9-114">Permission type</span></span>                        | <span data-ttu-id="39ba9-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39ba9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="39ba9-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39ba9-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="39ba9-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39ba9-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |

 <span data-ttu-id="39ba9-118">При входе пользователь видит только экземпляры, которым им назначен рецензент в accessReviewScheduleDefinition экземпляра.</span><span class="sxs-lookup"><span data-stu-id="39ba9-118">The signed-in user only sees instances of which they are assigned reviewer in the accessReviewScheduleDefinition of the instance.</span></span>

## <a name="http-request"></a><span data-ttu-id="39ba9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39ba9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances
```
## <a name="request-headers"></a><span data-ttu-id="39ba9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39ba9-120">Request headers</span></span>
<span data-ttu-id="39ba9-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="39ba9-121">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="39ba9-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39ba9-122">Request body</span></span>
<span data-ttu-id="39ba9-123">Не поставляем тело запроса.</span><span class="sxs-lookup"><span data-stu-id="39ba9-123">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="39ba9-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="39ba9-124">Response</span></span>
<span data-ttu-id="39ba9-125">В случае успешной работы этот метод возвращает код отклика и массив `200 OK` [объектов accessReviewInstance](../resources/accessreviewinstance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="39ba9-125">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39ba9-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="39ba9-126">Examples</span></span>
### <a name="request"></a><span data-ttu-id="39ba9-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="39ba9-127">Request</span></span>
<span data-ttu-id="39ba9-128">В следующем примере показан запрос на извлечение всех серий обзоров доступа в клиенте.</span><span class="sxs-lookup"><span data-stu-id="39ba9-128">The following example shows a request to retrieve all the access review series in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="39ba9-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="39ba9-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances?$expand=definition&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="39ba9-130">C#</span><span class="sxs-lookup"><span data-stu-id="39ba9-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39ba9-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39ba9-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39ba9-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39ba9-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39ba9-133">Java</span><span class="sxs-lookup"><span data-stu-id="39ba9-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="39ba9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="39ba9-134">Response</span></span>
><span data-ttu-id="39ba9-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="39ba9-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "id": "70a68410-67f3-4d4c-b946-6989e050be19",
            "startDateTime": "2020-09-09T15:57:56Z",
            "endDateTime": "2020-10-08T15:57:56Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "definition": {
                "id": "70a68410-67f3-4d4c-b946-6989e050be19",
                "displayName": "review of leadership",
                "createdDateTime": "2020-09-08T15:59:06Z",
                "lastModifiedDateTime": "2020-09-09T15:58:24Z",
                "status": "InProgress",
                "descriptionForAdmins": "review of leadership",
                "descriptionForReviewers": "",
                "createdBy": {
                    "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@msft.com"
                },
                "scope": {
                    "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff/transitiveMembers",
                    "queryType": "MicrosoftGraph"
                },
                "instanceEnumerationScope": {
                    "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff",
                    "queryType": "MicrosoftGraph"
                },
                "reviewers": [
                    {
                        "query": "/users/957f1027-c0ee-460d-9269-b8828e59e0fe",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
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
                        "pattern": null,
                        "range": {
                            "type": "numbered",
                            "numberOfOccurrences": 0,
                            "recurrenceTimeZone": null,
                            "startDate": "2020-09-09",
                            "endDate": "2020-10-08"
                        }
                    },
                    "applyActions": [
                        {
                            "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                        }
                    ]
                }
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="39ba9-136">См. также</span><span class="sxs-lookup"><span data-stu-id="39ba9-136">See also</span></span>

- [<span data-ttu-id="39ba9-137">Получить accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="39ba9-137">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)
- [<span data-ttu-id="39ba9-138">Получите accessReviewInstanceDecisionItems до утверждения</span><span class="sxs-lookup"><span data-stu-id="39ba9-138">Get accessReviewInstanceDecisionItems pending approval</span></span>](accessreviewinstancedecisionitem-listpendingapproval.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstance pendingApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
