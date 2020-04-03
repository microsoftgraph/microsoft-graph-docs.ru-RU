---
title: Список решений Акцессревиев
description: В функции проверок доступа Azure AD извлекаются решения объекта Акцессревиев.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7042210e9a3e3b6686e5c1bc4529a06d210a34d8
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123526"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="04195-103">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="04195-103">List accessReview decisions</span></span>

<span data-ttu-id="04195-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04195-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04195-105">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD извлекаются решения объекта [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="04195-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="04195-106">Обратите внимание, что для повторяющейся проверки доступа `decisions` связь не будет.</span><span class="sxs-lookup"><span data-stu-id="04195-106">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="04195-107">Вместо этого вызывающий объект должен перейти `instance` по связи, чтобы `accessReview` найти объект для текущего или последнего экземпляра проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="04195-107">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="04195-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04195-108">Permissions</span></span>
<span data-ttu-id="04195-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04195-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04195-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04195-111">Permission type</span></span>                        | <span data-ttu-id="04195-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04195-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="04195-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04195-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="04195-114">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="04195-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="04195-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04195-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04195-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04195-116">Not supported.</span></span> |
|<span data-ttu-id="04195-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04195-117">Application</span></span>                            | <span data-ttu-id="04195-118">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="04195-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="04195-119">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="04195-119">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="04195-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04195-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="04195-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04195-121">Request headers</span></span>
| <span data-ttu-id="04195-122">Имя</span><span class="sxs-lookup"><span data-stu-id="04195-122">Name</span></span>         | <span data-ttu-id="04195-123">Тип</span><span class="sxs-lookup"><span data-stu-id="04195-123">Type</span></span>        | <span data-ttu-id="04195-124">Описание</span><span class="sxs-lookup"><span data-stu-id="04195-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="04195-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="04195-125">Authorization</span></span> | <span data-ttu-id="04195-126">string</span><span class="sxs-lookup"><span data-stu-id="04195-126">string</span></span> | <span data-ttu-id="04195-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04195-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04195-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04195-129">Request body</span></span>
<span data-ttu-id="04195-130">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="04195-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="04195-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="04195-131">Response</span></span>
<span data-ttu-id="04195-132">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиевдеЦисион](../resources/accessreviewdecision.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04195-132">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04195-133">Пример</span><span class="sxs-lookup"><span data-stu-id="04195-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04195-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="04195-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="04195-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="04195-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="c"></a>[<span data-ttu-id="04195-136">C#</span><span class="sxs-lookup"><span data-stu-id="04195-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04195-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04195-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04195-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04195-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04195-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="04195-139">Response</span></span>
><span data-ttu-id="04195-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04195-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="04195-142">См. также</span><span class="sxs-lookup"><span data-stu-id="04195-142">See also</span></span>

| <span data-ttu-id="04195-143">Метод</span><span class="sxs-lookup"><span data-stu-id="04195-143">Method</span></span>           | <span data-ttu-id="04195-144">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="04195-144">Return Type</span></span>    |<span data-ttu-id="04195-145">Описание</span><span class="sxs-lookup"><span data-stu-id="04195-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="04195-146">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="04195-146">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="04195-147">акцессревиев</span><span class="sxs-lookup"><span data-stu-id="04195-147">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="04195-148">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="04195-148">Retrieve an access review.</span></span> |
|[<span data-ttu-id="04195-149">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="04195-149">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="04195-150">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="04195-150">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="04195-151">В качестве проверяющего получите мое решение Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="04195-151">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="04195-152">Отправка напоминания о Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="04195-152">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="04195-153">Нет.</span><span class="sxs-lookup"><span data-stu-id="04195-153">None.</span></span>   |   <span data-ttu-id="04195-154">Отправьте напоминание рецензентам Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="04195-154">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="04195-155">Остановить Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="04195-155">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="04195-156">Нет.</span><span class="sxs-lookup"><span data-stu-id="04195-156">None.</span></span>   |   <span data-ttu-id="04195-157">Остановка Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="04195-157">Stop an accessReview.</span></span> |
|[<span data-ttu-id="04195-158">Сброс решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="04195-158">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="04195-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="04195-159">None.</span></span>   |   <span data-ttu-id="04195-160">Сброс решений во время выполнения Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="04195-160">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="04195-161">Применение решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="04195-161">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="04195-162">Нет.</span><span class="sxs-lookup"><span data-stu-id="04195-162">None.</span></span>   |   <span data-ttu-id="04195-163">Применение решений из завершенной Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="04195-163">Apply the decisions from a completed accessReview.</span></span>|


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
