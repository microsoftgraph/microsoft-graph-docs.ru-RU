---
title: Список решений accessReview
description: В функции обзоров доступа Azure AD извлекаем решения объекта accessReview для вызываемого пользователя в качестве рецензента.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ca028cb7605f90037ec41b8c1e6d994766bf10d1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439358"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="d83b0-103">Список решений accessReview</span><span class="sxs-lookup"><span data-stu-id="d83b0-103">List my accessReview decisions</span></span>

<span data-ttu-id="d83b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d83b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d83b0-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) извлекаем решения объекта [accessReview](../resources/accessreview.md) для вызываемого пользователя в качестве рецензента.</span><span class="sxs-lookup"><span data-stu-id="d83b0-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="d83b0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d83b0-106">Permissions</span></span>
<span data-ttu-id="d83b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d83b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d83b0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d83b0-109">Permission type</span></span>                        | <span data-ttu-id="d83b0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d83b0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d83b0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d83b0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d83b0-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d83b0-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="d83b0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d83b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d83b0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d83b0-114">Not supported.</span></span> |
|<span data-ttu-id="d83b0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d83b0-115">Application</span></span>                            | <span data-ttu-id="d83b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d83b0-116">Not supported.</span></span> |

<span data-ttu-id="d83b0-117">Подписанное в пользователе также должно быть разрешено прочитать данный обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="d83b0-117">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="d83b0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d83b0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="d83b0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d83b0-119">Request headers</span></span>
| <span data-ttu-id="d83b0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d83b0-120">Name</span></span>         | <span data-ttu-id="d83b0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d83b0-121">Type</span></span>        | <span data-ttu-id="d83b0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d83b0-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d83b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d83b0-123">Authorization</span></span> | <span data-ttu-id="d83b0-124">string</span><span class="sxs-lookup"><span data-stu-id="d83b0-124">string</span></span> | <span data-ttu-id="d83b0-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d83b0-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d83b0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d83b0-127">Request body</span></span>
<span data-ttu-id="d83b0-128">Не следует поставлять тело запроса.</span><span class="sxs-lookup"><span data-stu-id="d83b0-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d83b0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d83b0-129">Response</span></span>
<span data-ttu-id="d83b0-130">В случае успешной работы этот метод возвращает код отклика и массив объектов `200, OK` [accessReviewDecision](../resources/accessreviewdecision.md) в теле ответа, для которых вызываемая пользователь является назначенным рецензентом.</span><span class="sxs-lookup"><span data-stu-id="d83b0-130">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="d83b0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d83b0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d83b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d83b0-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d83b0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d83b0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```
# <a name="c"></a>[<span data-ttu-id="d83b0-134">C#</span><span class="sxs-lookup"><span data-stu-id="d83b0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d83b0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d83b0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d83b0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d83b0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d83b0-137">Java</span><span class="sxs-lookup"><span data-stu-id="d83b0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d83b0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d83b0-138">Response</span></span>
><span data-ttu-id="d83b0-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d83b0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="d83b0-141">См. также</span><span class="sxs-lookup"><span data-stu-id="d83b0-141">See also</span></span>

| <span data-ttu-id="d83b0-142">Метод</span><span class="sxs-lookup"><span data-stu-id="d83b0-142">Method</span></span>           | <span data-ttu-id="d83b0-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d83b0-143">Return Type</span></span>    |<span data-ttu-id="d83b0-144">Описание</span><span class="sxs-lookup"><span data-stu-id="d83b0-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d83b0-145">Получить accessReview</span><span class="sxs-lookup"><span data-stu-id="d83b0-145">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="d83b0-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="d83b0-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="d83b0-147">Извлечение обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="d83b0-147">Retrieve an access review.</span></span> |
|[<span data-ttu-id="d83b0-148">Списки решений accessReview</span><span class="sxs-lookup"><span data-stu-id="d83b0-148">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="d83b0-149">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span><span class="sxs-lookup"><span data-stu-id="d83b0-149">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="d83b0-150">Извлечение всех решений accessReview.</span><span class="sxs-lookup"><span data-stu-id="d83b0-150">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


