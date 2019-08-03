---
title: Список решений Акцессревиев
description: В функции проверок доступа Azure AD извлекаются решения объекта Акцессревиев.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b82b3fc19320d1a4a1f4f77c18f5ad866f0a8cab
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172739"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="d344a-103">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="d344a-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d344a-104">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD извлекаются решения объекта [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="d344a-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="d344a-105">Обратите внимание, что для повторяющейся проверки доступа `decisions` связь не будет.</span><span class="sxs-lookup"><span data-stu-id="d344a-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="d344a-106">Вместо этого вызывающий объект должен перейти `instance` по связи, чтобы `accessReview` найти объект для текущего или последнего экземпляра проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="d344a-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="d344a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d344a-107">Permissions</span></span>
<span data-ttu-id="d344a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d344a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d344a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d344a-110">Permission type</span></span>                        | <span data-ttu-id="d344a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d344a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d344a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d344a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d344a-113">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d344a-113">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="d344a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d344a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d344a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d344a-115">Not supported.</span></span> |
|<span data-ttu-id="d344a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d344a-116">Application</span></span>                            | <span data-ttu-id="d344a-117">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="d344a-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="d344a-118">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="d344a-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="d344a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d344a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="d344a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d344a-120">Request headers</span></span>
| <span data-ttu-id="d344a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d344a-121">Name</span></span>         | <span data-ttu-id="d344a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d344a-122">Type</span></span>        | <span data-ttu-id="d344a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d344a-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d344a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d344a-124">Authorization</span></span> | <span data-ttu-id="d344a-125">string</span><span class="sxs-lookup"><span data-stu-id="d344a-125">string</span></span> | <span data-ttu-id="d344a-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d344a-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d344a-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d344a-128">Request body</span></span>
<span data-ttu-id="d344a-129">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="d344a-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d344a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d344a-130">Response</span></span>
<span data-ttu-id="d344a-131">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиевдеЦисион](../resources/accessreviewdecision.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d344a-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d344a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d344a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d344a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d344a-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d344a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d344a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d344a-135">C#</span><span class="sxs-lookup"><span data-stu-id="d344a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d344a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="d344a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d344a-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d344a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d344a-138">Java</span><span class="sxs-lookup"><span data-stu-id="d344a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d344a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d344a-139">Response</span></span>
><span data-ttu-id="d344a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d344a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d344a-142">См. также</span><span class="sxs-lookup"><span data-stu-id="d344a-142">See also</span></span>

| <span data-ttu-id="d344a-143">Метод</span><span class="sxs-lookup"><span data-stu-id="d344a-143">Method</span></span>           | <span data-ttu-id="d344a-144">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d344a-144">Return Type</span></span>    |<span data-ttu-id="d344a-145">Описание</span><span class="sxs-lookup"><span data-stu-id="d344a-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d344a-146">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="d344a-146">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="d344a-147">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="d344a-147">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="d344a-148">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="d344a-148">Retrieve an access review.</span></span> |
|[<span data-ttu-id="d344a-149">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="d344a-149">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="d344a-150">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="d344a-150">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="d344a-151">В качестве проверяющего получите мое решение Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="d344a-151">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="d344a-152">Отправка напоминания о Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="d344a-152">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="d344a-153">Нет.</span><span class="sxs-lookup"><span data-stu-id="d344a-153">None.</span></span>   |   <span data-ttu-id="d344a-154">Отправьте напоминание рецензентам Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="d344a-154">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="d344a-155">Остановить Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="d344a-155">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="d344a-156">Нет.</span><span class="sxs-lookup"><span data-stu-id="d344a-156">None.</span></span>   |   <span data-ttu-id="d344a-157">Остановка Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="d344a-157">Stop an accessReview.</span></span> |
|[<span data-ttu-id="d344a-158">Сброс решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="d344a-158">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="d344a-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="d344a-159">None.</span></span>   |   <span data-ttu-id="d344a-160">Сброс решений во время выполнения Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="d344a-160">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="d344a-161">Применение решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="d344a-161">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="d344a-162">Нет.</span><span class="sxs-lookup"><span data-stu-id="d344a-162">None.</span></span>   |   <span data-ttu-id="d344a-163">Применение решений из завершенной Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="d344a-163">Apply the decisions from a completed accessReview.</span></span>|


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
