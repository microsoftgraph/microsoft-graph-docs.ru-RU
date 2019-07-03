---
title: Обновление Акцессревиев
description: В функции рецензирования Access в Azure AD обновите существующий объект Акцессревиев, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0072beb769c99e0da63fae0e2fff258b09e986fe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439989"
---
# <a name="update-accessreview"></a><span data-ttu-id="15cc3-103">Обновление Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="15cc3-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15cc3-104">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD обновите существующий объект [акцессревиев](../resources/accessreview.md) , чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="15cc3-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="15cc3-105">Этот API не предназначен для изменения рецензентов или решений проверки.</span><span class="sxs-lookup"><span data-stu-id="15cc3-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="15cc3-106">Чтобы изменить проверяющих, используйте API [аддревиевер](accessreview-addreviewer.md) или [ремоверевиевер](accessreview-removereviewer.md) .</span><span class="sxs-lookup"><span data-stu-id="15cc3-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="15cc3-107">Чтобы остановить уже начатую проверку или уже запущенный экземпляр повторяющегося рецензирования, используйте API [Stop](accessreview-stop.md) .</span><span class="sxs-lookup"><span data-stu-id="15cc3-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="15cc3-108">Чтобы применить решения к целевой группе или правам доступа приложения, используйте API [Apply](accessreview-apply.md) .</span><span class="sxs-lookup"><span data-stu-id="15cc3-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="15cc3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15cc3-109">Permissions</span></span>
<span data-ttu-id="15cc3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15cc3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15cc3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15cc3-112">Permission type</span></span>                        | <span data-ttu-id="15cc3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15cc3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="15cc3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15cc3-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="15cc3-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15cc3-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="15cc3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15cc3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15cc3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15cc3-117">Not supported.</span></span> |
|<span data-ttu-id="15cc3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15cc3-118">Application</span></span>                            | <span data-ttu-id="15cc3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15cc3-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15cc3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15cc3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="15cc3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15cc3-121">Request headers</span></span>
| <span data-ttu-id="15cc3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="15cc3-122">Name</span></span>         | <span data-ttu-id="15cc3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="15cc3-123">Type</span></span>        | <span data-ttu-id="15cc3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="15cc3-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="15cc3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="15cc3-125">Authorization</span></span> | <span data-ttu-id="15cc3-126">string</span><span class="sxs-lookup"><span data-stu-id="15cc3-126">string</span></span> | <span data-ttu-id="15cc3-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15cc3-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15cc3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15cc3-129">Request body</span></span>
<span data-ttu-id="15cc3-130">В тексте запроса добавьте представление параметров объекта [акцессревиев](../resources/accessreview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15cc3-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="15cc3-131">В следующей таблице приведены свойства, которые можно указать при обновлении Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="15cc3-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="15cc3-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="15cc3-132">Property</span></span>     | <span data-ttu-id="15cc3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="15cc3-133">Type</span></span>        | <span data-ttu-id="15cc3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="15cc3-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="15cc3-135">Имя проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="15cc3-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="15cc3-136">Дата и время, когда выполняется запланированное начало проверки.</span><span class="sxs-lookup"><span data-stu-id="15cc3-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="15cc3-137">Это должна быть Дата в будущем.</span><span class="sxs-lookup"><span data-stu-id="15cc3-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="15cc3-138">Дата и время окончания запланированного рассмотрения.</span><span class="sxs-lookup"><span data-stu-id="15cc3-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="15cc3-139">Это должен быть по крайней мере один день позже даты начала.</span><span class="sxs-lookup"><span data-stu-id="15cc3-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="15cc3-140">Описание, которое будет отображаться для рецензентов.</span><span class="sxs-lookup"><span data-stu-id="15cc3-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="15cc3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="15cc3-141">Response</span></span>
<span data-ttu-id="15cc3-142">В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и объект [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15cc3-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15cc3-143">Пример</span><span class="sxs-lookup"><span data-stu-id="15cc3-143">Example</span></span>

<span data-ttu-id="15cc3-144">Это пример обновления доступа к одноразовой (неповторной) проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="15cc3-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="15cc3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="15cc3-145">Request</span></span>
<span data-ttu-id="15cc3-146">В теле запроса добавьте представление новых свойств объекта [акцессревиев](../resources/accessreview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15cc3-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="15cc3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="15cc3-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="15cc3-148">C#</span><span class="sxs-lookup"><span data-stu-id="15cc3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15cc3-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="15cc3-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="15cc3-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="15cc3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="15cc3-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="15cc3-151">Response</span></span>
><span data-ttu-id="15cc3-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15cc3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
