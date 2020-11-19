---
title: 'Акцессревиевинстанце: Пендингакцессревиевинстанцес'
description: Получение объектов Акцессревиевинстанце, ожидающих утверждения, вызывающим пользователем.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 793192a647865d524754f20be7d1deb664821d44
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222052"
---
# <a name="accessreviewinstance-pendingaccessreviewinstances"></a><span data-ttu-id="8050e-103">Акцессревиевинстанце: Пендингакцессревиевинстанцес</span><span class="sxs-lookup"><span data-stu-id="8050e-103">accessReviewInstance: pendingAccessReviewInstances</span></span>

<span data-ttu-id="8050e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8050e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8050e-105">Получение объектов [акцессревиевинстанце](../resources/accessreviewinstance.md) , ожидающих утверждения вызывающим пользователем.</span><span class="sxs-lookup"><span data-stu-id="8050e-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects pending approval by the calling user.</span></span> <span data-ttu-id="8050e-106">Возвращается список, содержащий ноль или более объектов Акцессревиевинстанце, для которых вызывающий пользователь является назначенным рецензентом.</span><span class="sxs-lookup"><span data-stu-id="8050e-106">A list of zero or more accessReviewInstance objects are returned, of which the calling user is an assigned reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="8050e-107">Если возвращается множество **акцессревиевинстанцес** , чтобы повысить эффективность и избежать истечения времени ожидания, извлеките набор результатов на страницы, включив в него как параметр запроса $Top, который содержит не более 100, и параметр запроса $Skip = 0 в запросе.</span><span class="sxs-lookup"><span data-stu-id="8050e-107">If many **accessReviewInstances** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="8050e-108">Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу с помощью свойства @odata. nextLink в ответе, который содержит URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="8050e-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="8050e-109">При наличии этого свойства Продолжайте делать дополнительные запросы с URL-адресом @odata. nextLink в каждом ответе до тех пор, пока не будут возвращены все результаты, как описано в разделе разбиение данных Microsoft Graph в приложении.</span><span class="sxs-lookup"><span data-stu-id="8050e-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="8050e-110">Если не указано ни одного параметра запроса и число результатов превышает 100, Microsoft Graph автоматически разбивать результаты на страницы 100 на каждой странице.</span><span class="sxs-lookup"><span data-stu-id="8050e-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="8050e-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8050e-111">Permissions</span></span>
<span data-ttu-id="8050e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8050e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8050e-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8050e-114">Permission type</span></span>                        | <span data-ttu-id="8050e-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8050e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8050e-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8050e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="8050e-117">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8050e-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |

 <span data-ttu-id="8050e-118">Вошедшего в систему пользователь видит только те экземпляры, которым назначен проверяющий в Акцессревиевсчедуледефинитион экземпляра.</span><span class="sxs-lookup"><span data-stu-id="8050e-118">The signed-in user only sees instances of which they are assigned reviewer in the accessReviewScheduleDefinition of the instance.</span></span>

## <a name="http-request"></a><span data-ttu-id="8050e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8050e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances
```
## <a name="request-headers"></a><span data-ttu-id="8050e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8050e-120">Request headers</span></span>
<span data-ttu-id="8050e-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="8050e-121">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="8050e-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8050e-122">Request body</span></span>
<span data-ttu-id="8050e-123">Не указывайте текст запроса.</span><span class="sxs-lookup"><span data-stu-id="8050e-123">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="8050e-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="8050e-124">Response</span></span>
<span data-ttu-id="8050e-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и массив объектов [акцессревиевинстанце](../resources/accessreviewinstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8050e-125">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8050e-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="8050e-126">Examples</span></span>
### <a name="request"></a><span data-ttu-id="8050e-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="8050e-127">Request</span></span>
<span data-ttu-id="8050e-128">В приведенном ниже примере показан запрос на получение всех рядов проверки доступа в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8050e-128">The following example shows a request to retrieve all the access review series in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="8050e-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="8050e-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances?$expand=definition&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="8050e-130">C#</span><span class="sxs-lookup"><span data-stu-id="8050e-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8050e-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8050e-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8050e-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8050e-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8050e-133">Java</span><span class="sxs-lookup"><span data-stu-id="8050e-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8050e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8050e-134">Response</span></span>
><span data-ttu-id="8050e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8050e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="8050e-137">См. также</span><span class="sxs-lookup"><span data-stu-id="8050e-137">See also</span></span>

- [<span data-ttu-id="8050e-138">Получение Акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="8050e-138">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)
- [<span data-ttu-id="8050e-139">Получение АкцессревиевинстанцедеЦисионитемс, ожидающих утверждения</span><span class="sxs-lookup"><span data-stu-id="8050e-139">Get accessReviewInstanceDecisionItems pending approval</span></span>](accessreviewinstancedecisionitem-listpendingapproval.md)


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
