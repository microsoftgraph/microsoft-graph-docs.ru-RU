---
title: List accessReviewInstance
description: Извлечение объектов accessReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 155c77e5a7b7fc8c81c5595dd2d504febd14673f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439198"
---
# <a name="list-accessreviewinstance"></a><span data-ttu-id="64d04-103">List accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="64d04-103">List accessReviewInstance</span></span>

<span data-ttu-id="64d04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64d04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64d04-105">[Извлечение объектов accessReviewInstance](../resources/accessreviewinstance.md) для определенного [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="64d04-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects for a specific [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="64d04-106">Возвращается список объектов zero или more **accessReviewInstance,** включая все вложенные свойства.</span><span class="sxs-lookup"><span data-stu-id="64d04-106">A list of zero or more **accessReviewInstance** objects are returned, including all of their nested properties.</span></span> <span data-ttu-id="64d04-107">Возвращенные объекты не включают связанный accessReviewInstanceDecisionItems.</span><span class="sxs-lookup"><span data-stu-id="64d04-107">Returned objects do not include associated accessReviewInstanceDecisionItems.</span></span> <span data-ttu-id="64d04-108">Чтобы получить решения в экземпляре, используйте [list accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span><span class="sxs-lookup"><span data-stu-id="64d04-108">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

>[!NOTE]
><span data-ttu-id="64d04-109">Если возвращается большое количество **accessReviewInstances,** чтобы повысить эффективность и избежать периодов времени, извлекайте результат, заданный на страницах, включив в запрос как параметр $top запроса с размером страницы не более 100, так и параметр запроса $skip=0 в запросе.</span><span class="sxs-lookup"><span data-stu-id="64d04-109">If many **accessReviewInstances** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="64d04-110">Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу с свойством @odata.nextLink в ответ, содержащий URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="64d04-110">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="64d04-111">Если это свойство присутствует, продолжайте делать дополнительные запросы с URL-адресом @odata.nextLink в каждом ответе, пока не будут возвращены все результаты, как описано в проверке данных Microsoft Graph в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="64d04-111">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="64d04-112">Если параметры запроса не предоставлены и результатов более 100, Microsoft Graph автоматически будет предоставлять результаты по 100 результатов на страницу.</span><span class="sxs-lookup"><span data-stu-id="64d04-112">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="64d04-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64d04-113">Permissions</span></span>
<span data-ttu-id="64d04-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64d04-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64d04-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64d04-116">Permission type</span></span>                        | <span data-ttu-id="64d04-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64d04-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="64d04-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64d04-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="64d04-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64d04-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="64d04-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="64d04-120">Application</span></span>                            | <span data-ttu-id="64d04-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64d04-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="64d04-122">В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="64d04-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="64d04-123">Чтобы просмотреть только те экземпляры, в которые назначен рецензент, см. в примере [List pending access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span><span class="sxs-lookup"><span data-stu-id="64d04-123">To view just the instances that the signed-in user is assigned the reviewer on, see [List pending access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span></span>

## <a name="http-request"></a><span data-ttu-id="64d04-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64d04-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```
## <a name="request-headers"></a><span data-ttu-id="64d04-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64d04-125">Request headers</span></span>
<span data-ttu-id="64d04-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="64d04-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="64d04-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64d04-127">Request body</span></span>
<span data-ttu-id="64d04-128">Не поставляем тело запроса.</span><span class="sxs-lookup"><span data-stu-id="64d04-128">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="64d04-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="64d04-129">Response</span></span>
<span data-ttu-id="64d04-130">В случае успешной работы этот метод возвращает код отклика и массив `200 OK` [объектов accessReviewInstance](../resources/accessreviewinstance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="64d04-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64d04-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="64d04-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="64d04-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="64d04-132">Request</span></span>
<span data-ttu-id="64d04-133">В следующем примере показан запрос на извлечение всех экземпляров обзора доступа для определения.</span><span class="sxs-lookup"><span data-stu-id="64d04-133">The following example shows a request to retrieve all the access review instances for a definition.</span></span>


# <a name="http"></a>[<span data-ttu-id="64d04-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="64d04-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04f34444/instances?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="64d04-135">C#</span><span class="sxs-lookup"><span data-stu-id="64d04-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64d04-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64d04-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64d04-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64d04-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64d04-138">Java</span><span class="sxs-lookup"><span data-stu-id="64d04-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64d04-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="64d04-139">Response</span></span>
><span data-ttu-id="64d04-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64d04-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "value": [
        {
            "id": "12490cdb-6a18-4c08-ba2c-44442f0a0138",
            "startDateTime": "2020-09-21T20:03:36Z",
            "endDateTime": "2020-09-23T20:03:36Z",
            "status": "NotStarted",
            "scope": {
                "query": "/groups/b7a04444-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        },
        {
            "id": "64444761-b89f-4d9c-afb9-fcfc8bb9cf45",
            "startDateTime": "2020-09-14T20:03:36.74Z",
            "endDateTime": "2020-09-16T20:03:36.74Z",
            "status": "Completed",
            "scope": {
                "query": "/groups/b7a04444-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="64d04-142">См. также</span><span class="sxs-lookup"><span data-stu-id="64d04-142">See also</span></span>

- [<span data-ttu-id="64d04-143">Список accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="64d04-143">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="64d04-144">Получить accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="64d04-144">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
