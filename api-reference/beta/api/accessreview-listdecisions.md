---
title: Список решений Акцессревиев
description: В функции проверок доступа Azure AD извлекаются решения объекта Акцессревиев.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 123eeb46ba38937722e68bee6aaa001c86320106
ms.sourcegitcommit: 4bdcb5cd3227ff009e10868f2936b3153372b87a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/25/2019
ms.locfileid: "33299642"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="72cf3-103">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="72cf3-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72cf3-104">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD извлекаются решения объекта [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="72cf3-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="72cf3-105">Обратите внимание, что для повторяющейся проверки доступа `decisions` связь не будет.</span><span class="sxs-lookup"><span data-stu-id="72cf3-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="72cf3-106">Вместо этого вызывающий объект должен перейти `instance` по связи, чтобы `accessReview` найти объект для текущего или последнего экземпляра проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="72cf3-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="72cf3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72cf3-107">Permissions</span></span>
<span data-ttu-id="72cf3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72cf3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72cf3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72cf3-110">Permission type</span></span>                        | <span data-ttu-id="72cf3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72cf3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="72cf3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72cf3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="72cf3-113">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="72cf3-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="72cf3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72cf3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72cf3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72cf3-115">Not supported.</span></span> |
|<span data-ttu-id="72cf3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72cf3-116">Application</span></span>                            | <span data-ttu-id="72cf3-117">Акцессревиев. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="72cf3-117">AccessReview.Read.All</span></span> |

 <span data-ttu-id="72cf3-118">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="72cf3-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="72cf3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72cf3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="72cf3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72cf3-120">Request headers</span></span>
| <span data-ttu-id="72cf3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="72cf3-121">Name</span></span>         | <span data-ttu-id="72cf3-122">Тип</span><span class="sxs-lookup"><span data-stu-id="72cf3-122">Type</span></span>        | <span data-ttu-id="72cf3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="72cf3-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="72cf3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="72cf3-124">Authorization</span></span> | <span data-ttu-id="72cf3-125">string</span><span class="sxs-lookup"><span data-stu-id="72cf3-125">string</span></span> | <span data-ttu-id="72cf3-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72cf3-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72cf3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72cf3-128">Request body</span></span>
<span data-ttu-id="72cf3-129">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="72cf3-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="72cf3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="72cf3-130">Response</span></span>
<span data-ttu-id="72cf3-131">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиевдеЦисион](../resources/accessreviewdecision.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72cf3-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72cf3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="72cf3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72cf3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="72cf3-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```

##### <a name="response"></a><span data-ttu-id="72cf3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="72cf3-134">Response</span></span>
><span data-ttu-id="72cf3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72cf3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="72cf3-137">См. также</span><span class="sxs-lookup"><span data-stu-id="72cf3-137">See also</span></span>

| <span data-ttu-id="72cf3-138">Метод</span><span class="sxs-lookup"><span data-stu-id="72cf3-138">Method</span></span>           | <span data-ttu-id="72cf3-139">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72cf3-139">Return Type</span></span>    |<span data-ttu-id="72cf3-140">Описание</span><span class="sxs-lookup"><span data-stu-id="72cf3-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72cf3-141">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="72cf3-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="72cf3-142">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="72cf3-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="72cf3-143">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="72cf3-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="72cf3-144">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="72cf3-144">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="72cf3-145">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="72cf3-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="72cf3-146">В качестве проверяющего получите мое решение Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="72cf3-146">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="72cf3-147">Отправка напоминания о Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="72cf3-147">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="72cf3-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="72cf3-148">None.</span></span>   |   <span data-ttu-id="72cf3-149">Отправьте напоминание рецензентам Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="72cf3-149">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="72cf3-150">Остановить Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="72cf3-150">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="72cf3-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="72cf3-151">None.</span></span>   |   <span data-ttu-id="72cf3-152">Остановка Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="72cf3-152">Stop an accessReview.</span></span> |
|[<span data-ttu-id="72cf3-153">Сброс решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="72cf3-153">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="72cf3-154">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="72cf3-154">None.</span></span>   |   <span data-ttu-id="72cf3-155">Сброс решений во время выполнения Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="72cf3-155">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="72cf3-156">Применение решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="72cf3-156">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="72cf3-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="72cf3-157">None.</span></span>   |   <span data-ttu-id="72cf3-158">Применение решений из завершенной Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="72cf3-158">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
