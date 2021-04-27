---
title: Обновление accessReview
description: В функции обзоров доступа Azure AD обновим существующий объект accessReview, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1b3870b4d44847d93fb2438c9f61d8ac3529433e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048444"
---
# <a name="update-accessreview"></a><span data-ttu-id="a2cae-103">Обновление accessReview</span><span class="sxs-lookup"><span data-stu-id="a2cae-103">Update accessReview</span></span>

<span data-ttu-id="a2cae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2cae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2cae-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) обновим существующий [объект accessReview,](../resources/accessreview.md) чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="a2cae-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="a2cae-106">Этот API не предназначен для изменения рецензентов или решений проверки.</span><span class="sxs-lookup"><span data-stu-id="a2cae-106">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="a2cae-107">Чтобы изменить рецензентов, используйте [API addReviewer](accessreview-addreviewer.md) или [removeReviewer.](accessreview-removereviewer.md)</span><span class="sxs-lookup"><span data-stu-id="a2cae-107">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="a2cae-108">Чтобы остановить уже запущенный разовую проверку или уже запущенный экземпляр повторяющегося обзора, используйте API [остановки.](accessreview-stop.md)</span><span class="sxs-lookup"><span data-stu-id="a2cae-108">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="a2cae-109">Чтобы применить решения к правам доступа к целевой группе или приложению, используйте [применимый](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="a2cae-109">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="a2cae-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2cae-110">Permissions</span></span>
<span data-ttu-id="a2cae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2cae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2cae-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2cae-113">Permission type</span></span>                        | <span data-ttu-id="a2cae-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2cae-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2cae-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2cae-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2cae-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2cae-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="a2cae-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2cae-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2cae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2cae-118">Not supported.</span></span> |
|<span data-ttu-id="a2cae-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="a2cae-119">Application</span></span>                            | <span data-ttu-id="a2cae-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="a2cae-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2cae-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2cae-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="a2cae-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2cae-122">Request headers</span></span>
| <span data-ttu-id="a2cae-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a2cae-123">Name</span></span>         | <span data-ttu-id="a2cae-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a2cae-124">Type</span></span>        | <span data-ttu-id="a2cae-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a2cae-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a2cae-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2cae-126">Authorization</span></span> | <span data-ttu-id="a2cae-127">string</span><span class="sxs-lookup"><span data-stu-id="a2cae-127">string</span></span> | <span data-ttu-id="a2cae-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2cae-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2cae-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2cae-130">Request body</span></span>
<span data-ttu-id="a2cae-131">В теле запроса поставляем представление JSON параметров [объекта accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="a2cae-131">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="a2cae-132">В следующей таблице показаны свойства, которые можно получить при обновлении accessReview.</span><span class="sxs-lookup"><span data-stu-id="a2cae-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="a2cae-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2cae-133">Property</span></span>     | <span data-ttu-id="a2cae-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a2cae-134">Type</span></span>        | <span data-ttu-id="a2cae-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a2cae-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="a2cae-136">Имя обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="a2cae-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="a2cae-137">DateTime, когда планируется начать проверку.</span><span class="sxs-lookup"><span data-stu-id="a2cae-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="a2cae-138">Это должна быть дата в будущем.</span><span class="sxs-lookup"><span data-stu-id="a2cae-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="a2cae-139">DateTime, когда проверка должна завершиться.</span><span class="sxs-lookup"><span data-stu-id="a2cae-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="a2cae-140">Это должно быть по крайней мере на один день позже даты начала.</span><span class="sxs-lookup"><span data-stu-id="a2cae-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="a2cae-141">Описание, чтобы показать рецензентам.</span><span class="sxs-lookup"><span data-stu-id="a2cae-141">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="a2cae-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2cae-142">Response</span></span>
<span data-ttu-id="a2cae-143">В случае успешной работы этот метод возвращает код отклика и `204, Accepted` [объект accessReview](../resources/accessreview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a2cae-143">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2cae-144">Пример</span><span class="sxs-lookup"><span data-stu-id="a2cae-144">Example</span></span>

<span data-ttu-id="a2cae-145">Это пример обновления разового (не повторяемого) обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="a2cae-145">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="a2cae-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2cae-146">Request</span></span>
<span data-ttu-id="a2cae-147">В теле запроса поставляем представление JSON о новых свойствах [объекта accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="a2cae-147">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="a2cae-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2cae-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a2cae-149">C#</span><span class="sxs-lookup"><span data-stu-id="a2cae-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2cae-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2cae-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2cae-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2cae-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2cae-152">Java</span><span class="sxs-lookup"><span data-stu-id="a2cae-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a2cae-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2cae-153">Response</span></span>
><span data-ttu-id="a2cae-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a2cae-154">**Note:** The response object shown here might be shortened for readability.</span></span>
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


