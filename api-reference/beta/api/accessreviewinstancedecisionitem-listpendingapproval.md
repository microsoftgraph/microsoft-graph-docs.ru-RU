---
title: Список accessReviewInstanceDecisionItem до утверждения
description: Извлечение объектов accessReviewInstanceDecisionItem до утверждения пользователем вызова.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d1ce0293510f2f9a6ca526216b3fc2ad024b6285
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030480"
---
# <a name="list-accessreviewinstancedecisionitems-pending-approval-deprecated"></a><span data-ttu-id="abf89-103">List accessReviewInstanceDecisionItems pending approval (deprecated)</span><span class="sxs-lookup"><span data-stu-id="abf89-103">List accessReviewInstanceDecisionItems pending approval (deprecated)</span></span>

<span data-ttu-id="abf89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abf89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="abf89-105">Этот метод будет обесценится и прекратит возвращать данные 19 мая 2023 г.</span><span class="sxs-lookup"><span data-stu-id="abf89-105">This method will be deprecated and will stop returning data on May 19, 2023.</span></span> <span data-ttu-id="abf89-106">Он был заменен [filterByCurrentUser](accessreviewinstancedecisionitem-filterbycurrentuser.md).</span><span class="sxs-lookup"><span data-stu-id="abf89-106">It has been replaced by [filterByCurrentUser](accessreviewinstancedecisionitem-filterbycurrentuser.md).</span></span>

<span data-ttu-id="abf89-107">Извлечение [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) для определенного [accessReviewInstance](../resources/accessreviewscheduledefinition.md) до утверждения пользователем вызова.</span><span class="sxs-lookup"><span data-stu-id="abf89-107">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects for a specific [accessReviewInstance](../resources/accessreviewscheduledefinition.md) pending approval by the calling user.</span></span> <span data-ttu-id="abf89-108">Возвращается список объектов zero или more accessReviewInstanceDecisionItem, включая все вложенные свойства.</span><span class="sxs-lookup"><span data-stu-id="abf89-108">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="abf89-109">Размер страницы по умолчанию для этого API — 100 объектов accessReviewInstanceDecisionItem.</span><span class="sxs-lookup"><span data-stu-id="abf89-109">The default page size for this API is 100 accessReviewInstanceDecisionItem objects.</span></span> <span data-ttu-id="abf89-110">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="abf89-110">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="abf89-111">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="abf89-111">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="abf89-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abf89-112">Permissions</span></span>
<span data-ttu-id="abf89-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abf89-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abf89-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abf89-115">Permission type</span></span>                        | <span data-ttu-id="abf89-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="abf89-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="abf89-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abf89-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="abf89-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abf89-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="abf89-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abf89-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abf89-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abf89-120">Not supported.</span></span>|

<span data-ttu-id="abf89-121">При входе пользователь также увидит решения, которым им назначен рецензент в доступе экземпляра этого решенияReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="abf89-121">The signed-in user will also only see decisions of which they are assigned reviewer in that decision's instance's accessReviewScheduleDefinition.</span></span>

## <a name="http-request"></a><span data-ttu-id="abf89-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abf89-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances/{instance-id}/decisions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abf89-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="abf89-123">Optional query parameters</span></span>
<span data-ttu-id="abf89-124">Этот метод поддерживает `$skip` параметры `$top` запроса OData и помогает настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="abf89-124">This method supports `$skip` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="abf89-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="abf89-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="abf89-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abf89-126">Request headers</span></span>
<span data-ttu-id="abf89-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="abf89-127">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="abf89-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abf89-128">Request body</span></span>
<span data-ttu-id="abf89-129">Не поставляем тело запроса.</span><span class="sxs-lookup"><span data-stu-id="abf89-129">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="abf89-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="abf89-130">Response</span></span>
<span data-ttu-id="abf89-131">В случае успешной работы этот метод возвращает код ответа и массив `200 OK` [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="abf89-131">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="abf89-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="abf89-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="abf89-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="abf89-133">Request</span></span>
<span data-ttu-id="abf89-134">В следующем примере показан запрос на извлечение всех решений в экземпляре обзора доступа до утверждения вызываемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="abf89-134">The following example shows a request to retrieve all the decisions on an instance of an access review pending the calling user's approval.</span></span>


# <a name="http"></a>[<span data-ttu-id="abf89-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="abf89-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="abf89-136">C#</span><span class="sxs-lookup"><span data-stu-id="abf89-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abf89-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abf89-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abf89-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abf89-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="abf89-139">Java</span><span class="sxs-lookup"><span data-stu-id="abf89-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="abf89-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="abf89-140">Response</span></span>
><span data-ttu-id="abf89-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="abf89-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="abf89-142">См. также</span><span class="sxs-lookup"><span data-stu-id="abf89-142">See also</span></span>

- [<span data-ttu-id="abf89-143">Получить accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="abf89-143">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="abf89-144">Получить accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="abf89-144">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


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
