---
title: Список решений Акцессревиев
description: В функции проверок доступа Azure AD извлекаются решения объекта Акцессревиев.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b0b2844ecdfbe7663c6832ae0a72c018c6ed9ea4
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655476"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="70e8d-103">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="70e8d-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70e8d-104">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD извлекаются решения объекта [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="70e8d-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="70e8d-105">Обратите внимание, что для повторяющейся проверки доступа `decisions` связь не будет.</span><span class="sxs-lookup"><span data-stu-id="70e8d-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="70e8d-106">Вместо этого вызывающий объект должен перейти `instance` по связи, чтобы `accessReview` найти объект для текущего или последнего экземпляра проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="70e8d-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="70e8d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70e8d-107">Permissions</span></span>
<span data-ttu-id="70e8d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70e8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70e8d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70e8d-110">Permission type</span></span>                        | <span data-ttu-id="70e8d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70e8d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="70e8d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70e8d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="70e8d-113">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="70e8d-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="70e8d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70e8d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70e8d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70e8d-115">Not supported.</span></span> |
|<span data-ttu-id="70e8d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70e8d-116">Application</span></span>                            | <span data-ttu-id="70e8d-117">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="70e8d-117">AccessReview.Read.All</span></span> |

 <span data-ttu-id="70e8d-118">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="70e8d-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="70e8d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70e8d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="70e8d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70e8d-120">Request headers</span></span>
| <span data-ttu-id="70e8d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="70e8d-121">Name</span></span>         | <span data-ttu-id="70e8d-122">Тип</span><span class="sxs-lookup"><span data-stu-id="70e8d-122">Type</span></span>        | <span data-ttu-id="70e8d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="70e8d-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="70e8d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="70e8d-124">Authorization</span></span> | <span data-ttu-id="70e8d-125">string</span><span class="sxs-lookup"><span data-stu-id="70e8d-125">string</span></span> | <span data-ttu-id="70e8d-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70e8d-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70e8d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70e8d-128">Request body</span></span>
<span data-ttu-id="70e8d-129">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="70e8d-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="70e8d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="70e8d-130">Response</span></span>
<span data-ttu-id="70e8d-131">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиевдеЦисион](../resources/accessreviewdecision.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70e8d-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70e8d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="70e8d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70e8d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="70e8d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```

##### <a name="response"></a><span data-ttu-id="70e8d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="70e8d-134">Response</span></span>
><span data-ttu-id="70e8d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70e8d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="70e8d-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="70e8d-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="70e8d-138">C#</span><span class="sxs-lookup"><span data-stu-id="70e8d-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70e8d-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="70e8d-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="70e8d-140">См. также</span><span class="sxs-lookup"><span data-stu-id="70e8d-140">See also</span></span>

| <span data-ttu-id="70e8d-141">Метод</span><span class="sxs-lookup"><span data-stu-id="70e8d-141">Method</span></span>           | <span data-ttu-id="70e8d-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="70e8d-142">Return Type</span></span>    |<span data-ttu-id="70e8d-143">Описание</span><span class="sxs-lookup"><span data-stu-id="70e8d-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70e8d-144">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="70e8d-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="70e8d-145">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="70e8d-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="70e8d-146">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="70e8d-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="70e8d-147">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="70e8d-147">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="70e8d-148">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="70e8d-148">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="70e8d-149">В качестве проверяющего получите мое решение Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="70e8d-149">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="70e8d-150">Отправка напоминания о Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="70e8d-150">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="70e8d-151">Нет.</span><span class="sxs-lookup"><span data-stu-id="70e8d-151">None.</span></span>   |   <span data-ttu-id="70e8d-152">Отправьте напоминание рецензентам Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="70e8d-152">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="70e8d-153">Остановить Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="70e8d-153">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="70e8d-154">Нет.</span><span class="sxs-lookup"><span data-stu-id="70e8d-154">None.</span></span>   |   <span data-ttu-id="70e8d-155">Остановка Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="70e8d-155">Stop an accessReview.</span></span> |
|[<span data-ttu-id="70e8d-156">Сброс решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="70e8d-156">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="70e8d-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="70e8d-157">None.</span></span>   |   <span data-ttu-id="70e8d-158">Сброс решений во время выполнения Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="70e8d-158">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="70e8d-159">Применение решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="70e8d-159">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="70e8d-160">Нет.</span><span class="sxs-lookup"><span data-stu-id="70e8d-160">None.</span></span>   |   <span data-ttu-id="70e8d-161">Применение решений из завершенной Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="70e8d-161">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
