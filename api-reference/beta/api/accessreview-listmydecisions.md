---
title: Список решений accessReview
description: В функции обзоров доступа Azure AD извлекаем решения объекта accessReview для вызываемого пользователя в качестве рецензента.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 31f065033d1980c8a1ab640294f52f893a1f02f0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048472"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="006b6-103">Список решений accessReview</span><span class="sxs-lookup"><span data-stu-id="006b6-103">List my accessReview decisions</span></span>

<span data-ttu-id="006b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="006b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="006b6-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) извлекаем решения объекта [accessReview](../resources/accessreview.md) для вызываемого пользователя в качестве рецензента.</span><span class="sxs-lookup"><span data-stu-id="006b6-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="006b6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="006b6-106">Permissions</span></span>
<span data-ttu-id="006b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="006b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="006b6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="006b6-109">Permission type</span></span>                        | <span data-ttu-id="006b6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="006b6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="006b6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="006b6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="006b6-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="006b6-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="006b6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="006b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="006b6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="006b6-114">Not supported.</span></span> |
|<span data-ttu-id="006b6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="006b6-115">Application</span></span>                            | <span data-ttu-id="006b6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="006b6-116">Not supported.</span></span> |

<span data-ttu-id="006b6-117">Подписанное в пользователе также должно быть разрешено прочитать данный обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="006b6-117">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="006b6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="006b6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="006b6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="006b6-119">Request headers</span></span>
| <span data-ttu-id="006b6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="006b6-120">Name</span></span>         | <span data-ttu-id="006b6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="006b6-121">Type</span></span>        | <span data-ttu-id="006b6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="006b6-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="006b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="006b6-123">Authorization</span></span> | <span data-ttu-id="006b6-124">string</span><span class="sxs-lookup"><span data-stu-id="006b6-124">string</span></span> | <span data-ttu-id="006b6-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="006b6-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="006b6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="006b6-127">Request body</span></span>
<span data-ttu-id="006b6-128">Не следует поставлять тело запроса.</span><span class="sxs-lookup"><span data-stu-id="006b6-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="006b6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="006b6-129">Response</span></span>
<span data-ttu-id="006b6-130">В случае успешной работы этот метод возвращает код отклика и массив объектов `200, OK` [accessReviewDecision](../resources/accessreviewdecision.md) в теле ответа, для которых вызываемая пользователь является назначенным рецензентом.</span><span class="sxs-lookup"><span data-stu-id="006b6-130">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="006b6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="006b6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="006b6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="006b6-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="006b6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="006b6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```
# <a name="c"></a>[<span data-ttu-id="006b6-134">C#</span><span class="sxs-lookup"><span data-stu-id="006b6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="006b6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="006b6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="006b6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="006b6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="006b6-137">Java</span><span class="sxs-lookup"><span data-stu-id="006b6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="006b6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="006b6-138">Response</span></span>
><span data-ttu-id="006b6-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="006b6-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="006b6-140">См. также</span><span class="sxs-lookup"><span data-stu-id="006b6-140">See also</span></span>

| <span data-ttu-id="006b6-141">Метод</span><span class="sxs-lookup"><span data-stu-id="006b6-141">Method</span></span>           | <span data-ttu-id="006b6-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="006b6-142">Return Type</span></span>    |<span data-ttu-id="006b6-143">Описание</span><span class="sxs-lookup"><span data-stu-id="006b6-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="006b6-144">Получить accessReview</span><span class="sxs-lookup"><span data-stu-id="006b6-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="006b6-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="006b6-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="006b6-146">Извлечение обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="006b6-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="006b6-147">Списки решений accessReview</span><span class="sxs-lookup"><span data-stu-id="006b6-147">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="006b6-148">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span><span class="sxs-lookup"><span data-stu-id="006b6-148">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="006b6-149">Извлечение всех решений accessReview.</span><span class="sxs-lookup"><span data-stu-id="006b6-149">Retrieve all the decisions of an accessReview.</span></span>|


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


