---
title: Список решений Акцессревиев
description: В функции проверок доступа Azure AD извлекаются решения объекта Акцессревиев.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fee4b4adc4bc4e33964575976c67cfeaa077a34c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323729"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="fce26-103">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fce26-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fce26-104">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD извлекаются решения объекта [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="fce26-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="fce26-105">Обратите внимание, что для повторяющейся проверки доступа `decisions` связь не будет.</span><span class="sxs-lookup"><span data-stu-id="fce26-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="fce26-106">Вместо этого вызывающий объект должен перейти `instance` по связи, чтобы `accessReview` найти объект для текущего или последнего экземпляра проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="fce26-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="fce26-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fce26-107">Permissions</span></span>
<span data-ttu-id="fce26-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fce26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fce26-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fce26-110">Permission type</span></span>                        | <span data-ttu-id="fce26-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fce26-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fce26-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fce26-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fce26-113">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fce26-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="fce26-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fce26-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fce26-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fce26-115">Not supported.</span></span> |
|<span data-ttu-id="fce26-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fce26-116">Application</span></span>                            | <span data-ttu-id="fce26-117">Акцессревиев. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="fce26-117">AccessReview.Read.All</span></span> |

 <span data-ttu-id="fce26-118">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="fce26-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="fce26-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fce26-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="fce26-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fce26-120">Request headers</span></span>
| <span data-ttu-id="fce26-121">Имя</span><span class="sxs-lookup"><span data-stu-id="fce26-121">Name</span></span>         | <span data-ttu-id="fce26-122">Тип</span><span class="sxs-lookup"><span data-stu-id="fce26-122">Type</span></span>        | <span data-ttu-id="fce26-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fce26-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fce26-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fce26-124">Authorization</span></span> | <span data-ttu-id="fce26-125">string</span><span class="sxs-lookup"><span data-stu-id="fce26-125">string</span></span> | <span data-ttu-id="fce26-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fce26-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fce26-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fce26-128">Request body</span></span>
<span data-ttu-id="fce26-129">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="fce26-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="fce26-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fce26-130">Response</span></span>
<span data-ttu-id="fce26-131">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиевдеЦисион](../resources/accessreviewdecision.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fce26-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fce26-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fce26-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fce26-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fce26-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```

##### <a name="response"></a><span data-ttu-id="fce26-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fce26-134">Response</span></span>
><span data-ttu-id="fce26-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fce26-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="fce26-137">См. также</span><span class="sxs-lookup"><span data-stu-id="fce26-137">See also</span></span>

| <span data-ttu-id="fce26-138">Метод</span><span class="sxs-lookup"><span data-stu-id="fce26-138">Method</span></span>           | <span data-ttu-id="fce26-139">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fce26-139">Return Type</span></span>    |<span data-ttu-id="fce26-140">Описание</span><span class="sxs-lookup"><span data-stu-id="fce26-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fce26-141">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fce26-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="fce26-142">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fce26-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="fce26-143">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="fce26-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="fce26-144">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fce26-144">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="fce26-145">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="fce26-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="fce26-146">В качестве проверяющего получите мое решение Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="fce26-146">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="fce26-147">Отправка напоминания о Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fce26-147">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="fce26-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fce26-148">None.</span></span>   |   <span data-ttu-id="fce26-149">Отправьте напоминание рецензентам Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="fce26-149">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="fce26-150">Остановить Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fce26-150">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="fce26-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fce26-151">None.</span></span>   |   <span data-ttu-id="fce26-152">Остановка Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="fce26-152">Stop an accessReview.</span></span> |
|[<span data-ttu-id="fce26-153">Сброс решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fce26-153">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="fce26-154">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fce26-154">None.</span></span>   |   <span data-ttu-id="fce26-155">Сброс решений во время выполнения Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="fce26-155">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="fce26-156">Применение решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fce26-156">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="fce26-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fce26-157">None.</span></span>   |   <span data-ttu-id="fce26-158">Применение решений из завершенной Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="fce26-158">Apply the decisions from a completed accessReview.</span></span>|


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
