---
title: Список моих решений Акцессревиев
description: В функции рецензирования Access в Azure AD извлекаются решения объекта Акцессревиев для вызывающего пользователя как проверяющего.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 51eeafd316433678643978b187888e4044d4fbf8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586075"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="651a8-103">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="651a8-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="651a8-104">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD извлекаются решения объекта [акцессревиев](../resources/accessreview.md) для вызывающего пользователя как проверяющего.</span><span class="sxs-lookup"><span data-stu-id="651a8-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="651a8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="651a8-105">Permissions</span></span>
<span data-ttu-id="651a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="651a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="651a8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="651a8-108">Permission type</span></span>                        | <span data-ttu-id="651a8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="651a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="651a8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="651a8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="651a8-111">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="651a8-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="651a8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="651a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="651a8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="651a8-113">Not supported.</span></span> |
|<span data-ttu-id="651a8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="651a8-114">Application</span></span>                            | <span data-ttu-id="651a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="651a8-115">Not supported.</span></span> |

<span data-ttu-id="651a8-116">Кроме того, вошедшего в систему пользователь должен иметь разрешение на чтение этой конкретной проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="651a8-116">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="651a8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="651a8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="651a8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="651a8-118">Request headers</span></span>
| <span data-ttu-id="651a8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="651a8-119">Name</span></span>         | <span data-ttu-id="651a8-120">Тип</span><span class="sxs-lookup"><span data-stu-id="651a8-120">Type</span></span>        | <span data-ttu-id="651a8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="651a8-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="651a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="651a8-122">Authorization</span></span> | <span data-ttu-id="651a8-123">string</span><span class="sxs-lookup"><span data-stu-id="651a8-123">string</span></span> | <span data-ttu-id="651a8-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="651a8-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="651a8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="651a8-126">Request body</span></span>
<span data-ttu-id="651a8-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="651a8-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="651a8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="651a8-128">Response</span></span>
<span data-ttu-id="651a8-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиевдеЦисион](../resources/accessreviewdecision.md) в теле отклика, для которого вызывающий пользователь является назначенным рецензентом.</span><span class="sxs-lookup"><span data-stu-id="651a8-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="651a8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="651a8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="651a8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="651a8-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```

##### <a name="response"></a><span data-ttu-id="651a8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="651a8-132">Response</span></span>
><span data-ttu-id="651a8-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="651a8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="651a8-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="651a8-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="651a8-136">Языках</span><span class="sxs-lookup"><span data-stu-id="651a8-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="651a8-137">Язык</span><span class="sxs-lookup"><span data-stu-id="651a8-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="651a8-138">См. также</span><span class="sxs-lookup"><span data-stu-id="651a8-138">See also</span></span>

| <span data-ttu-id="651a8-139">Метод</span><span class="sxs-lookup"><span data-stu-id="651a8-139">Method</span></span>           | <span data-ttu-id="651a8-140">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="651a8-140">Return Type</span></span>    |<span data-ttu-id="651a8-141">Описание</span><span class="sxs-lookup"><span data-stu-id="651a8-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="651a8-142">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="651a8-142">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="651a8-143">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="651a8-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="651a8-144">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="651a8-144">Retrieve an access review.</span></span> |
|[<span data-ttu-id="651a8-145">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="651a8-145">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="651a8-146">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="651a8-146">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="651a8-147">Получение всех решений Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="651a8-147">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
