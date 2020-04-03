---
title: Список моих решений Акцессревиев
description: В функции рецензирования Access в Azure AD извлекаются решения объекта Акцессревиев для вызывающего пользователя как проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7722d6084399fc00b0f99932ac7173b2d83dfa08
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123575"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="1e589-103">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="1e589-103">List my accessReview decisions</span></span>

<span data-ttu-id="1e589-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e589-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e589-105">В функции [рецензирования Access](../resources/accessreviews-root.md) в Azure AD извлекаются решения объекта [акцессревиев](../resources/accessreview.md) для вызывающего пользователя как проверяющего.</span><span class="sxs-lookup"><span data-stu-id="1e589-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e589-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e589-106">Permissions</span></span>
<span data-ttu-id="1e589-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e589-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e589-109">Permission type</span></span>                        | <span data-ttu-id="1e589-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e589-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e589-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e589-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e589-112">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1e589-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="1e589-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e589-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e589-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e589-114">Not supported.</span></span> |
|<span data-ttu-id="1e589-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e589-115">Application</span></span>                            | <span data-ttu-id="1e589-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e589-116">Not supported.</span></span> |

<span data-ttu-id="1e589-117">Кроме того, вошедшего в систему пользователь должен иметь разрешение на чтение этой конкретной проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="1e589-117">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="1e589-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e589-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="1e589-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e589-119">Request headers</span></span>
| <span data-ttu-id="1e589-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1e589-120">Name</span></span>         | <span data-ttu-id="1e589-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1e589-121">Type</span></span>        | <span data-ttu-id="1e589-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1e589-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1e589-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e589-123">Authorization</span></span> | <span data-ttu-id="1e589-124">string</span><span class="sxs-lookup"><span data-stu-id="1e589-124">string</span></span> | <span data-ttu-id="1e589-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e589-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e589-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e589-127">Request body</span></span>
<span data-ttu-id="1e589-128">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="1e589-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="1e589-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e589-129">Response</span></span>
<span data-ttu-id="1e589-130">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиевдеЦисион](../resources/accessreviewdecision.md) в теле отклика, для которого вызывающий пользователь является назначенным рецензентом.</span><span class="sxs-lookup"><span data-stu-id="1e589-130">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="1e589-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1e589-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e589-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e589-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1e589-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e589-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```
# <a name="c"></a>[<span data-ttu-id="1e589-134">C#</span><span class="sxs-lookup"><span data-stu-id="1e589-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e589-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e589-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e589-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e589-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1e589-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e589-137">Response</span></span>
><span data-ttu-id="1e589-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e589-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="1e589-140">См. также</span><span class="sxs-lookup"><span data-stu-id="1e589-140">See also</span></span>

| <span data-ttu-id="1e589-141">Метод</span><span class="sxs-lookup"><span data-stu-id="1e589-141">Method</span></span>           | <span data-ttu-id="1e589-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1e589-142">Return Type</span></span>    |<span data-ttu-id="1e589-143">Описание</span><span class="sxs-lookup"><span data-stu-id="1e589-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1e589-144">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="1e589-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="1e589-145">акцессревиев</span><span class="sxs-lookup"><span data-stu-id="1e589-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="1e589-146">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="1e589-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="1e589-147">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="1e589-147">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="1e589-148">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="1e589-148">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="1e589-149">Получение всех решений Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="1e589-149">Retrieve all the decisions of an accessReview.</span></span>|


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
