---
title: Обновление accessReview
description: В функции обзоров доступа Azure AD обновим существующий объект accessReview, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 817cf535c68a775c7a90a639e09120e226c46115
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751010"
---
# <a name="update-accessreview"></a><span data-ttu-id="e610a-103">Обновление accessReview</span><span class="sxs-lookup"><span data-stu-id="e610a-103">Update accessReview</span></span>

<span data-ttu-id="e610a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e610a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e610a-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) обновим существующий [объект accessReview,](../resources/accessreview.md) чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="e610a-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="e610a-106">Этот API не предназначен для изменения рецензентов или решений проверки.</span><span class="sxs-lookup"><span data-stu-id="e610a-106">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="e610a-107">Чтобы изменить рецензентов, используйте [API addReviewer](accessreview-addreviewer.md) или [removeReviewer.](accessreview-removereviewer.md)</span><span class="sxs-lookup"><span data-stu-id="e610a-107">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="e610a-108">Чтобы остановить уже запущенный разовую проверку или уже запущенный экземпляр повторяющегося обзора, используйте API [остановки.](accessreview-stop.md)</span><span class="sxs-lookup"><span data-stu-id="e610a-108">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="e610a-109">Чтобы применить решения к правам доступа к целевой группе или приложению, используйте [применимый](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="e610a-109">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="e610a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e610a-110">Permissions</span></span>
<span data-ttu-id="e610a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e610a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e610a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e610a-113">Permission type</span></span>                        | <span data-ttu-id="e610a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e610a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e610a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e610a-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e610a-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e610a-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="e610a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e610a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e610a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e610a-118">Not supported.</span></span> |
|<span data-ttu-id="e610a-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="e610a-119">Application</span></span>                            | <span data-ttu-id="e610a-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="e610a-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="e610a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e610a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="e610a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e610a-122">Request headers</span></span>
| <span data-ttu-id="e610a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e610a-123">Name</span></span>         | <span data-ttu-id="e610a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e610a-124">Type</span></span>        | <span data-ttu-id="e610a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e610a-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e610a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e610a-126">Authorization</span></span> | <span data-ttu-id="e610a-127">string</span><span class="sxs-lookup"><span data-stu-id="e610a-127">string</span></span> | <span data-ttu-id="e610a-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e610a-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e610a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e610a-130">Request body</span></span>
<span data-ttu-id="e610a-131">В теле запроса поставляем представление JSON параметров [объекта accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="e610a-131">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="e610a-132">В следующей таблице показаны свойства, которые можно получить при обновлении accessReview.</span><span class="sxs-lookup"><span data-stu-id="e610a-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="e610a-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="e610a-133">Property</span></span>      | <span data-ttu-id="e610a-134">Тип</span><span class="sxs-lookup"><span data-stu-id="e610a-134">Type</span></span>           | <span data-ttu-id="e610a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="e610a-135">Description</span></span>                                                                                                |
|:--------------|:---------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e610a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e610a-136">displayName</span></span>   | <span data-ttu-id="e610a-137">String</span><span class="sxs-lookup"><span data-stu-id="e610a-137">String</span></span>         | <span data-ttu-id="e610a-138">Имя обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="e610a-138">The access review name.</span></span>                                                                                    |
| <span data-ttu-id="e610a-139">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e610a-139">startDateTime</span></span> | <span data-ttu-id="e610a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e610a-140">DateTimeOffset</span></span> | <span data-ttu-id="e610a-141">DateTime, когда планируется начать проверку.</span><span class="sxs-lookup"><span data-stu-id="e610a-141">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="e610a-142">Это должна быть дата в будущем.</span><span class="sxs-lookup"><span data-stu-id="e610a-142">This must be a date in the future.</span></span>                 |
| <span data-ttu-id="e610a-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e610a-143">endDateTime</span></span>   | <span data-ttu-id="e610a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e610a-144">DateTimeOffset</span></span> | <span data-ttu-id="e610a-145">DateTime, когда проверка должна завершиться.</span><span class="sxs-lookup"><span data-stu-id="e610a-145">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="e610a-146">Это должно быть по крайней мере на один день позже даты начала.</span><span class="sxs-lookup"><span data-stu-id="e610a-146">This must be at least one day later than the start date.</span></span> |
| <span data-ttu-id="e610a-147">description</span><span class="sxs-lookup"><span data-stu-id="e610a-147">description</span></span>   | <span data-ttu-id="e610a-148">String</span><span class="sxs-lookup"><span data-stu-id="e610a-148">String</span></span>         | <span data-ttu-id="e610a-149">Описание, чтобы показать рецензентам.</span><span class="sxs-lookup"><span data-stu-id="e610a-149">The description, to show to the reviewers.</span></span>                                                                 |



## <a name="response"></a><span data-ttu-id="e610a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e610a-150">Response</span></span>
<span data-ttu-id="e610a-151">В случае успешной работы этот метод возвращает код отклика и `204 Accepted` [объект accessReview](../resources/accessreview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e610a-151">If successful, this method returns a `204 Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e610a-152">Пример</span><span class="sxs-lookup"><span data-stu-id="e610a-152">Example</span></span>

<span data-ttu-id="e610a-153">Это пример обновления разового (не повторяемого) обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="e610a-153">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="e610a-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="e610a-154">Request</span></span>
<span data-ttu-id="e610a-155">В теле запроса поставляем представление JSON о новых свойствах [объекта accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="e610a-155">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="e610a-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="e610a-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews/006111db-0810-4494-a6df-904d368bd81b
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```
# <a name="c"></a>[<span data-ttu-id="e610a-157">C#</span><span class="sxs-lookup"><span data-stu-id="e610a-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e610a-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e610a-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e610a-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e610a-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e610a-160">Java</span><span class="sxs-lookup"><span data-stu-id="e610a-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e610a-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="e610a-161">Response</span></span>
><span data-ttu-id="e610a-162">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e610a-162">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


