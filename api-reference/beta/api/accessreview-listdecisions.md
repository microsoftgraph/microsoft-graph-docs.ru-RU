---
title: Списки решений accessReview
description: В функции обзоров доступа Azure AD извлекаем решения объекта accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a3566889236934a2b0668cecd50c8b5b860e61cb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048486"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="f41e2-103">Списки решений accessReview</span><span class="sxs-lookup"><span data-stu-id="f41e2-103">List accessReview decisions</span></span>

<span data-ttu-id="f41e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f41e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f41e2-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) извлекаем решения объекта [accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="f41e2-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="f41e2-106">Обратите внимание, что повторяющиеся проверки доступа не будут иметь `decisions` отношения.</span><span class="sxs-lookup"><span data-stu-id="f41e2-106">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="f41e2-107">Вместо этого вызываемая должна перемещаться по отношениям, чтобы найти объект для текущего или последнего `instance` `accessReview` экземпляра обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="f41e2-107">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="f41e2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f41e2-108">Permissions</span></span>
<span data-ttu-id="f41e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f41e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f41e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f41e2-111">Permission type</span></span>                        | <span data-ttu-id="f41e2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f41e2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f41e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f41e2-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f41e2-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f41e2-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="f41e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f41e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f41e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f41e2-116">Not supported.</span></span> |
|<span data-ttu-id="f41e2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f41e2-117">Application</span></span>                            | <span data-ttu-id="f41e2-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="f41e2-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="f41e2-119">Подписанный пользователь также должен быть в роли каталога, что позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="f41e2-119">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="f41e2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f41e2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="f41e2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f41e2-121">Request headers</span></span>
| <span data-ttu-id="f41e2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f41e2-122">Name</span></span>         | <span data-ttu-id="f41e2-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f41e2-123">Type</span></span>        | <span data-ttu-id="f41e2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f41e2-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f41e2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f41e2-125">Authorization</span></span> | <span data-ttu-id="f41e2-126">string</span><span class="sxs-lookup"><span data-stu-id="f41e2-126">string</span></span> | <span data-ttu-id="f41e2-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f41e2-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f41e2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f41e2-129">Request body</span></span>
<span data-ttu-id="f41e2-130">Не следует поставлять тело запроса.</span><span class="sxs-lookup"><span data-stu-id="f41e2-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="f41e2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f41e2-131">Response</span></span>
<span data-ttu-id="f41e2-132">В случае успешной работы этот метод возвращает код отклика и массив `200, OK` [объектов accessReviewDecision](../resources/accessreviewdecision.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f41e2-132">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f41e2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f41e2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f41e2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f41e2-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f41e2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f41e2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="c"></a>[<span data-ttu-id="f41e2-136">C#</span><span class="sxs-lookup"><span data-stu-id="f41e2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f41e2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f41e2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f41e2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f41e2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f41e2-139">Java</span><span class="sxs-lookup"><span data-stu-id="f41e2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f41e2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f41e2-140">Response</span></span>
><span data-ttu-id="f41e2-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f41e2-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f41e2-142">См. также</span><span class="sxs-lookup"><span data-stu-id="f41e2-142">See also</span></span>

| <span data-ttu-id="f41e2-143">Метод</span><span class="sxs-lookup"><span data-stu-id="f41e2-143">Method</span></span>           | <span data-ttu-id="f41e2-144">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f41e2-144">Return Type</span></span>    |<span data-ttu-id="f41e2-145">Описание</span><span class="sxs-lookup"><span data-stu-id="f41e2-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f41e2-146">Получить accessReview</span><span class="sxs-lookup"><span data-stu-id="f41e2-146">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="f41e2-147">accessReview</span><span class="sxs-lookup"><span data-stu-id="f41e2-147">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="f41e2-148">Извлечение обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="f41e2-148">Retrieve an access review.</span></span> |
|[<span data-ttu-id="f41e2-149">Список решений accessReview</span><span class="sxs-lookup"><span data-stu-id="f41e2-149">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="f41e2-150">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span><span class="sxs-lookup"><span data-stu-id="f41e2-150">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="f41e2-151">Как рецензент, получите мои решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="f41e2-151">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="f41e2-152">Отправка напоминания accessReview</span><span class="sxs-lookup"><span data-stu-id="f41e2-152">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="f41e2-153">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f41e2-153">None.</span></span>   |   <span data-ttu-id="f41e2-154">Отправьте напоминание рецензентам accessReview.</span><span class="sxs-lookup"><span data-stu-id="f41e2-154">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="f41e2-155">Остановка accessReview</span><span class="sxs-lookup"><span data-stu-id="f41e2-155">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="f41e2-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f41e2-156">None.</span></span>   |   <span data-ttu-id="f41e2-157">Остановите accessReview.</span><span class="sxs-lookup"><span data-stu-id="f41e2-157">Stop an accessReview.</span></span> |
|[<span data-ttu-id="f41e2-158">Сброс решений accessReview</span><span class="sxs-lookup"><span data-stu-id="f41e2-158">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="f41e2-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f41e2-159">None.</span></span>   |   <span data-ttu-id="f41e2-160">Сброс решений в ходе выполнения accessReview.</span><span class="sxs-lookup"><span data-stu-id="f41e2-160">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="f41e2-161">Применение решений accessReview</span><span class="sxs-lookup"><span data-stu-id="f41e2-161">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="f41e2-162">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f41e2-162">None.</span></span>   |   <span data-ttu-id="f41e2-163">Применение решений из завершенного accessReview.</span><span class="sxs-lookup"><span data-stu-id="f41e2-163">Apply the decisions from a completed accessReview.</span></span>|


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


