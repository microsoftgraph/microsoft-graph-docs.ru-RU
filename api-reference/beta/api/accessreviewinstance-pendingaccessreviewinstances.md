---
title: 'accessReviewInstance: pendingAccessReviewInstances'
description: Извлечение объектов accessReviewInstance до утверждения с помощью вызова пользователя.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c62f954ea7fe70d46ff4a46879b4d568d619226c
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030539"
---
# <a name="accessreviewinstance-pendingaccessreviewinstances-deprecated"></a><span data-ttu-id="cc273-103">accessReviewInstance: pendingAccessReviewInstances (deprecated)</span><span class="sxs-lookup"><span data-stu-id="cc273-103">accessReviewInstance: pendingAccessReviewInstances (deprecated)</span></span>

<span data-ttu-id="cc273-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc273-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="cc273-105">Этот метод будет обесценится и прекратит возвращать данные 19 мая 2023 г.</span><span class="sxs-lookup"><span data-stu-id="cc273-105">This method will be deprecated and will stop returning data on May 19, 2023.</span></span> <span data-ttu-id="cc273-106">Он был заменен [filterByCurrentUser](accessreviewinstance-filterbycurrentuser.md).</span><span class="sxs-lookup"><span data-stu-id="cc273-106">It has been replaced by [filterByCurrentUser](accessreviewinstance-filterbycurrentuser.md).</span></span>

>[!NOTE]
><span data-ttu-id="cc273-107">Размер страницы по умолчанию для этого API — 100 объектов accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="cc273-107">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="cc273-108">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="cc273-108">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="cc273-109">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="cc273-109">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="cc273-110">Извлечение [объектов accessReviewInstance](../resources/accessreviewinstance.md) до утверждения пользователем вызова.</span><span class="sxs-lookup"><span data-stu-id="cc273-110">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects pending approval by the calling user.</span></span> <span data-ttu-id="cc273-111">Возвращается список нулевых или более объектов accessReviewInstance, из которых пользователем вызова является назначен рецензент.</span><span class="sxs-lookup"><span data-stu-id="cc273-111">A list of zero or more accessReviewInstance objects are returned, of which the calling user is an assigned reviewer.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc273-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc273-112">Permissions</span></span>
<span data-ttu-id="cc273-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc273-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc273-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc273-115">Permission type</span></span>                        | <span data-ttu-id="cc273-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc273-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc273-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc273-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc273-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc273-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |

 <span data-ttu-id="cc273-119">При входе пользователь видит только экземпляры, которым им назначен рецензент в accessReviewScheduleDefinition экземпляра.</span><span class="sxs-lookup"><span data-stu-id="cc273-119">The signed-in user only sees instances of which they are assigned reviewer in the accessReviewScheduleDefinition of the instance.</span></span>

## <a name="http-request"></a><span data-ttu-id="cc273-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc273-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc273-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cc273-121">Optional query parameters</span></span>
<span data-ttu-id="cc273-122">Этот метод поддерживает `$skip` параметры `$top` запроса OData и помогает настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="cc273-122">This method supports `$skip` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="cc273-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cc273-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc273-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc273-124">Request headers</span></span>
<span data-ttu-id="cc273-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="cc273-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="cc273-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc273-126">Request body</span></span>
<span data-ttu-id="cc273-127">Не поставляем тело запроса.</span><span class="sxs-lookup"><span data-stu-id="cc273-127">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="cc273-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc273-128">Response</span></span>
<span data-ttu-id="cc273-129">В случае успешной работы этот метод возвращает код отклика и массив `200 OK` [объектов accessReviewInstance](../resources/accessreviewinstance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cc273-129">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc273-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc273-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="cc273-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc273-131">Request</span></span>
<span data-ttu-id="cc273-132">В следующем примере показан запрос на извлечение всех серий обзоров доступа в клиенте.</span><span class="sxs-lookup"><span data-stu-id="cc273-132">The following example shows a request to retrieve all the access review series in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc273-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc273-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances?$expand=definition&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="cc273-134">C#</span><span class="sxs-lookup"><span data-stu-id="cc273-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc273-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc273-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc273-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc273-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc273-137">Java</span><span class="sxs-lookup"><span data-stu-id="cc273-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cc273-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc273-138">Response</span></span>
><span data-ttu-id="cc273-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cc273-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="cc273-140">См. также</span><span class="sxs-lookup"><span data-stu-id="cc273-140">See also</span></span>

- [<span data-ttu-id="cc273-141">Получить accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="cc273-141">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)
- [<span data-ttu-id="cc273-142">Получите accessReviewInstanceDecisionItems до утверждения</span><span class="sxs-lookup"><span data-stu-id="cc273-142">Get accessReviewInstanceDecisionItems pending approval</span></span>](accessreviewinstancedecisionitem-listpendingapproval.md)


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
