---
title: List accessReviewInstanceDecisionItem
description: Извлечение объектов accessReviewInstanceDecisionItem.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1d2ec913e3ef942f76c26c86df74493819c2d790
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439137"
---
# <a name="list-accessreviewinstancedecisionitem"></a><span data-ttu-id="08b1b-103">List accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="08b1b-103">List accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="08b1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08b1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08b1b-105">[Извлечение объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) для определенного [accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="08b1b-105">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects for a specific [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="08b1b-106">Возвращается список объектов zero или more accessReviewInstanceDecisionItem, включая все вложенные свойства.</span><span class="sxs-lookup"><span data-stu-id="08b1b-106">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="08b1b-107">Если возвращается много **accessReviewInstanceDecisionItems,** чтобы повысить эффективность и избежать периодов времени, извлеките результат, заданный на страницах, включив в запрос как параметр $top запроса с размером страницы не более 100, так и параметр запроса $skip=0 в запросе.</span><span class="sxs-lookup"><span data-stu-id="08b1b-107">If many **accessReviewInstanceDecisionItems** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="08b1b-108">Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу с свойством @odata.nextLink в ответ, содержащий URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="08b1b-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="08b1b-109">Если это свойство присутствует, продолжайте делать дополнительные запросы с URL-адресом @odata.nextLink в каждом ответе, пока не будут возвращены все результаты, как описано в проверке данных Microsoft Graph в вашем приложении.</span><span class="sxs-lookup"><span data-stu-id="08b1b-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="08b1b-110">Если параметры запроса не предоставлены и результатов более 100, Microsoft Graph автоматически будет предоставлять результаты по 100 результатов на страницу.</span><span class="sxs-lookup"><span data-stu-id="08b1b-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="08b1b-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08b1b-111">Permissions</span></span>
<span data-ttu-id="08b1b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08b1b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08b1b-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08b1b-114">Permission type</span></span>                        | <span data-ttu-id="08b1b-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08b1b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="08b1b-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08b1b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="08b1b-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08b1b-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="08b1b-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08b1b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08b1b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08b1b-119">Not supported.</span></span>|
|<span data-ttu-id="08b1b-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="08b1b-120">Application</span></span>                            | <span data-ttu-id="08b1b-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08b1b-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="08b1b-122">В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="08b1b-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="08b1b-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08b1b-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="08b1b-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08b1b-124">Request headers</span></span>
<span data-ttu-id="08b1b-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="08b1b-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="08b1b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08b1b-126">Request body</span></span>
<span data-ttu-id="08b1b-127">Не поставляем тело запроса.</span><span class="sxs-lookup"><span data-stu-id="08b1b-127">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="08b1b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="08b1b-128">Response</span></span>
<span data-ttu-id="08b1b-129">В случае успешной работы этот метод возвращает код ответа и массив `200 OK` [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="08b1b-129">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08b1b-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="08b1b-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="08b1b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="08b1b-131">Request</span></span>
<span data-ttu-id="08b1b-132">В следующем примере показан запрос на извлечение всех решений в экземпляре обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="08b1b-132">The following example shows a request to retrieve all the decisions on an instance of an access review.</span></span>


# <a name="http"></a>[<span data-ttu-id="08b1b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="08b1b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/14444cdb-6a18-4c08-ba2c-48c02f0a0138/decisions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="08b1b-134">C#</span><span class="sxs-lookup"><span data-stu-id="08b1b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08b1b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08b1b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08b1b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08b1b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08b1b-137">Java</span><span class="sxs-lookup"><span data-stu-id="08b1b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="08b1b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="08b1b-138">Response</span></span>
><span data-ttu-id="08b1b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08b1b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.count": 4,
    "value": [
        {
            "id": "77a61af9-3bef-4bbf-b00b-04734d6d5eae",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
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
                "userId": "3736c87b-dc21-4290-8802-d6fef5fa3a08",
                "userDisplayName": "Irvin Sayers",
                "userPrincipalName": "IrvinS@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "f30b68ef-b843-4479-86b8-0a3a2f4bb209",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:08.377Z",
            "decision": "Approve",
            "justification": "This employee needs access for reason X",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "ecd78419-3f1e-4f07-9bd9-7c77137af4f1",
                "userDisplayName": "Bianca Pisani",
                "userPrincipalName": "BiancaP@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "037b737f-e8ca-4507-b126-5a0620ba2c18",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:28.473Z",
            "decision": "Deny",
            "justification": "This employee changed roles and no longer needs access",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "5f16b75b-031c-4944-9691-070f03273079",
                "userDisplayName": "Delia Dennis",
                "userPrincipalName": "DeliaD@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "7032f455-10a3-4d04-bf02-66fb65d26d10",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:44.38Z",
            "decision": "DontKnow",
            "justification": "I do not know what this employee needs",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "4169762e-895f-4350-a13d-e5b09b1efcfa",
                "userDisplayName": "Isaiah Langer",
                "userPrincipalName": "IsaiahL@M365x471116.OnMicrosoft.com"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="08b1b-141">См. также</span><span class="sxs-lookup"><span data-stu-id="08b1b-141">See also</span></span>

- [<span data-ttu-id="08b1b-142">Получить accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="08b1b-142">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="08b1b-143">Получить accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="08b1b-143">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
