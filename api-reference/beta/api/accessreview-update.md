---
title: Обновление Акцессревиев
description: В функции рецензирования Access в Azure AD обновите существующий объект Акцессревиев, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 41fbea3d7a934f71fa7923bc50651339976af888
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258788"
---
# <a name="update-accessreview"></a><span data-ttu-id="39a46-103">Обновление Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="39a46-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39a46-104">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD обновите существующий объект [акцессревиев](../resources/accessreview.md) , чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="39a46-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="39a46-105">Этот API не предназначен для изменения рецензентов или решений проверки.</span><span class="sxs-lookup"><span data-stu-id="39a46-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="39a46-106">Чтобы изменить проверяющих, используйте API [аддревиевер](accessreview-addreviewer.md) или [ремоверевиевер](accessreview-removereviewer.md) .</span><span class="sxs-lookup"><span data-stu-id="39a46-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="39a46-107">Чтобы остановить уже начатую проверку или уже запущенный экземпляр повторяющегося рецензирования, используйте API [Stop](accessreview-stop.md) .</span><span class="sxs-lookup"><span data-stu-id="39a46-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="39a46-108">Чтобы применить решения к целевой группе или правам доступа приложения, используйте API [Apply](accessreview-apply.md) .</span><span class="sxs-lookup"><span data-stu-id="39a46-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="39a46-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39a46-109">Permissions</span></span>
<span data-ttu-id="39a46-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39a46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39a46-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39a46-112">Permission type</span></span>                        | <span data-ttu-id="39a46-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39a46-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="39a46-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39a46-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="39a46-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39a46-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="39a46-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39a46-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39a46-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39a46-117">Not supported.</span></span> |
|<span data-ttu-id="39a46-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39a46-118">Application</span></span>                            | <span data-ttu-id="39a46-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39a46-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39a46-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39a46-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="39a46-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39a46-121">Request headers</span></span>
| <span data-ttu-id="39a46-122">Имя</span><span class="sxs-lookup"><span data-stu-id="39a46-122">Name</span></span>         | <span data-ttu-id="39a46-123">Тип</span><span class="sxs-lookup"><span data-stu-id="39a46-123">Type</span></span>        | <span data-ttu-id="39a46-124">Описание</span><span class="sxs-lookup"><span data-stu-id="39a46-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="39a46-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="39a46-125">Authorization</span></span> | <span data-ttu-id="39a46-126">string</span><span class="sxs-lookup"><span data-stu-id="39a46-126">string</span></span> | <span data-ttu-id="39a46-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39a46-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39a46-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39a46-129">Request body</span></span>
<span data-ttu-id="39a46-130">В тексте запроса добавьте представление параметров объекта [акцессревиев](../resources/accessreview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39a46-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="39a46-131">В следующей таблице приведены свойства, которые можно указать при обновлении Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="39a46-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="39a46-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="39a46-132">Property</span></span>     | <span data-ttu-id="39a46-133">Тип</span><span class="sxs-lookup"><span data-stu-id="39a46-133">Type</span></span>        | <span data-ttu-id="39a46-134">Описание</span><span class="sxs-lookup"><span data-stu-id="39a46-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="39a46-135">Имя проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="39a46-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="39a46-136">Дата и время, когда выполняется запланированное начало проверки.</span><span class="sxs-lookup"><span data-stu-id="39a46-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="39a46-137">Это должна быть Дата в будущем.</span><span class="sxs-lookup"><span data-stu-id="39a46-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="39a46-138">Дата и время окончания запланированного рассмотрения.</span><span class="sxs-lookup"><span data-stu-id="39a46-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="39a46-139">Это должен быть по крайней мере один день позже даты начала.</span><span class="sxs-lookup"><span data-stu-id="39a46-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="39a46-140">Описание, которое будет отображаться для рецензентов.</span><span class="sxs-lookup"><span data-stu-id="39a46-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="39a46-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="39a46-141">Response</span></span>
<span data-ttu-id="39a46-142">В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и объект [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39a46-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39a46-143">Пример</span><span class="sxs-lookup"><span data-stu-id="39a46-143">Example</span></span>

<span data-ttu-id="39a46-144">Это пример обновления доступа к одноразовой (неповторной) проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="39a46-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="39a46-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="39a46-145">Request</span></span>
<span data-ttu-id="39a46-146">В теле запроса добавьте представление новых свойств объекта [акцессревиев](../resources/accessreview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39a46-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="39a46-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="39a46-147">Response</span></span>
><span data-ttu-id="39a46-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39a46-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="39a46-150">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="39a46-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="39a46-151">C#</span><span class="sxs-lookup"><span data-stu-id="39a46-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="39a46-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="39a46-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_accessReview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="39a46-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="39a46-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_accessReview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
