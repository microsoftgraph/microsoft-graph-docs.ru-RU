---
title: Список accessReviewInstanceDecisionItem до утверждения
description: Извлечение объектов accessReviewInstanceDecisionItem до утверждения пользователем вызова.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2eabb7f646806d501dfacad8aa2b22e8cb5e95ee
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048388"
---
# <a name="list-accessreviewinstancedecisionitems-pending-approval"></a><span data-ttu-id="74f24-103">Список accessReviewInstanceDecisionItems до утверждения</span><span class="sxs-lookup"><span data-stu-id="74f24-103">List accessReviewInstanceDecisionItems pending approval</span></span>

<span data-ttu-id="74f24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74f24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74f24-105">Извлечение [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) для определенного [accessReviewInstance](../resources/accessreviewscheduledefinition.md) до утверждения пользователем вызова.</span><span class="sxs-lookup"><span data-stu-id="74f24-105">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects for a specific [accessReviewInstance](../resources/accessreviewscheduledefinition.md) pending approval by the calling user.</span></span> <span data-ttu-id="74f24-106">Возвращается список объектов zero или more accessReviewInstanceDecisionItem, включая все вложенные свойства.</span><span class="sxs-lookup"><span data-stu-id="74f24-106">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="74f24-107">Если возвращается много **accessReviewInstanceDecisionItems,** чтобы повысить эффективность и избежать периодов времени, извлеките результат, заданный на страницах, включив в запрос как параметр $top запроса с размером страницы не более 100, так и параметр запроса $skip=0 в запросе.</span><span class="sxs-lookup"><span data-stu-id="74f24-107">If many **accessReviewInstanceDecisionItems** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="74f24-108">Если набор результатов охватывает несколько страниц, корпорация Майкрософт Graph возвращает эту страницу с свойством @odata.nextLink в ответе, который содержит URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="74f24-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="74f24-109">Если это свойство присутствует, продолжайте делать дополнительные запросы с URL-адресом @odata.nextLink в каждом ответе, пока не будут возвращены все результаты, как описано в Graph данных Microsoft в приложении.</span><span class="sxs-lookup"><span data-stu-id="74f24-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="74f24-110">Если параметры запроса не предоставлены и результатов более 100, microsoft Graph автоматически будет предоставлять результаты по 100 результатов на странице.</span><span class="sxs-lookup"><span data-stu-id="74f24-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="74f24-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74f24-111">Permissions</span></span>
<span data-ttu-id="74f24-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74f24-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74f24-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74f24-114">Permission type</span></span>                        | <span data-ttu-id="74f24-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74f24-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="74f24-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74f24-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="74f24-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f24-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="74f24-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74f24-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74f24-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74f24-119">Not supported.</span></span>|

<span data-ttu-id="74f24-120">При входе пользователь также увидит решения, которым им назначен рецензент в доступе экземпляра этого решенияReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="74f24-120">The signed-in user will also only see decisions of which they are assigned reviewer in that decision's instance's accessReviewScheduleDefinition.</span></span>

## <a name="http-request"></a><span data-ttu-id="74f24-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74f24-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances/{instance-id}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="74f24-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74f24-122">Request headers</span></span>
<span data-ttu-id="74f24-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="74f24-123">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="74f24-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74f24-124">Request body</span></span>
<span data-ttu-id="74f24-125">Не поставляем тело запроса.</span><span class="sxs-lookup"><span data-stu-id="74f24-125">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="74f24-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="74f24-126">Response</span></span>
<span data-ttu-id="74f24-127">В случае успешной работы этот метод возвращает код ответа и массив `200 OK` [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="74f24-127">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74f24-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="74f24-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="74f24-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="74f24-129">Request</span></span>
<span data-ttu-id="74f24-130">В следующем примере показан запрос на извлечение всех решений в экземпляре обзора доступа до утверждения вызываемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="74f24-130">The following example shows a request to retrieve all the decisions on an instance of an access review pending the calling user's approval.</span></span>


# <a name="http"></a>[<span data-ttu-id="74f24-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="74f24-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="74f24-132">C#</span><span class="sxs-lookup"><span data-stu-id="74f24-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74f24-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74f24-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74f24-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74f24-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74f24-135">Java</span><span class="sxs-lookup"><span data-stu-id="74f24-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="74f24-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="74f24-136">Response</span></span>
><span data-ttu-id="74f24-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="74f24-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 2,
    "value": [
        {
            "id": "654b34e7-b48f-4772-a2d4-08f1d0dd014c",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "7eae986b-d425-48b2-adf2-3c777f6256f3",
                "userDisplayName": "Adele Vance",
                "userPrincipalName": "AdeleV@contoso.com"
            }
        },
        {
            "id": "0311dba4-c60c-412e-ac77-14e1da23daf1",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "userDisplayName": "MOD Administrator",
                "userPrincipalName": "admin@contoso.com"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="74f24-138">См. также</span><span class="sxs-lookup"><span data-stu-id="74f24-138">See also</span></span>

- [<span data-ttu-id="74f24-139">Получить accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="74f24-139">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="74f24-140">Получить accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="74f24-140">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstanceDecisionItem pendingApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
