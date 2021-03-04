---
title: Обновление accessReview
description: В функции обзоров доступа Azure AD обновим существующий объект accessReview, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6de1862411d20f1e1fc68fc202a5e59aa888f165
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439263"
---
# <a name="update-accessreview"></a><span data-ttu-id="b20e7-103">Обновление accessReview</span><span class="sxs-lookup"><span data-stu-id="b20e7-103">Update accessReview</span></span>

<span data-ttu-id="b20e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b20e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b20e7-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) обновим существующий [объект accessReview,](../resources/accessreview.md) чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="b20e7-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="b20e7-106">Этот API не предназначен для изменения рецензентов или решений проверки.</span><span class="sxs-lookup"><span data-stu-id="b20e7-106">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="b20e7-107">Чтобы изменить рецензентов, используйте [API addReviewer](accessreview-addreviewer.md) или [removeReviewer.](accessreview-removereviewer.md)</span><span class="sxs-lookup"><span data-stu-id="b20e7-107">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="b20e7-108">Чтобы остановить уже запущенный разовую проверку или уже запущенный экземпляр повторяющегося обзора, используйте API [остановки.](accessreview-stop.md)</span><span class="sxs-lookup"><span data-stu-id="b20e7-108">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="b20e7-109">Чтобы применить решения к правам доступа к целевой группе или приложению, используйте [применимый](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="b20e7-109">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="b20e7-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b20e7-110">Permissions</span></span>
<span data-ttu-id="b20e7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b20e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b20e7-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b20e7-113">Permission type</span></span>                        | <span data-ttu-id="b20e7-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b20e7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b20e7-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b20e7-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="b20e7-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b20e7-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b20e7-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b20e7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b20e7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b20e7-118">Not supported.</span></span> |
|<span data-ttu-id="b20e7-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="b20e7-119">Application</span></span>                            | <span data-ttu-id="b20e7-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="b20e7-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="b20e7-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b20e7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="b20e7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b20e7-122">Request headers</span></span>
| <span data-ttu-id="b20e7-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b20e7-123">Name</span></span>         | <span data-ttu-id="b20e7-124">Тип</span><span class="sxs-lookup"><span data-stu-id="b20e7-124">Type</span></span>        | <span data-ttu-id="b20e7-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b20e7-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b20e7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b20e7-126">Authorization</span></span> | <span data-ttu-id="b20e7-127">string</span><span class="sxs-lookup"><span data-stu-id="b20e7-127">string</span></span> | <span data-ttu-id="b20e7-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b20e7-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b20e7-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b20e7-130">Request body</span></span>
<span data-ttu-id="b20e7-131">В теле запроса поставляем представление JSON параметров [объекта accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="b20e7-131">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="b20e7-132">В следующей таблице показаны свойства, которые можно получить при обновлении accessReview.</span><span class="sxs-lookup"><span data-stu-id="b20e7-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="b20e7-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="b20e7-133">Property</span></span>     | <span data-ttu-id="b20e7-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b20e7-134">Type</span></span>        | <span data-ttu-id="b20e7-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b20e7-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="b20e7-136">Имя обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="b20e7-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="b20e7-137">DateTime, когда планируется начать проверку.</span><span class="sxs-lookup"><span data-stu-id="b20e7-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="b20e7-138">Это должна быть дата в будущем.</span><span class="sxs-lookup"><span data-stu-id="b20e7-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="b20e7-139">DateTime, когда проверка должна завершиться.</span><span class="sxs-lookup"><span data-stu-id="b20e7-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="b20e7-140">Это должно быть по крайней мере на один день позже даты начала.</span><span class="sxs-lookup"><span data-stu-id="b20e7-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="b20e7-141">Описание, чтобы показать рецензентам.</span><span class="sxs-lookup"><span data-stu-id="b20e7-141">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="b20e7-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b20e7-142">Response</span></span>
<span data-ttu-id="b20e7-143">В случае успешной работы этот метод возвращает код отклика и `204, Accepted` [объект accessReview](../resources/accessreview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b20e7-143">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b20e7-144">Пример</span><span class="sxs-lookup"><span data-stu-id="b20e7-144">Example</span></span>

<span data-ttu-id="b20e7-145">Это пример обновления разового (не повторяемого) обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="b20e7-145">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="b20e7-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b20e7-146">Request</span></span>
<span data-ttu-id="b20e7-147">В теле запроса поставляем представление JSON о новых свойствах [объекта accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="b20e7-147">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="b20e7-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="b20e7-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b20e7-149">C#</span><span class="sxs-lookup"><span data-stu-id="b20e7-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b20e7-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b20e7-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b20e7-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b20e7-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b20e7-152">Java</span><span class="sxs-lookup"><span data-stu-id="b20e7-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b20e7-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b20e7-153">Response</span></span>
><span data-ttu-id="b20e7-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b20e7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


