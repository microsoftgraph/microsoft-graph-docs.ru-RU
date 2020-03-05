---
title: Обновление Акцессревиев
description: В функции рецензирования Access в Azure AD обновите существующий объект Акцессревиев, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e711aafa474b8d701e69f8f541625aaf8f1f4a9c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441819"
---
# <a name="update-accessreview"></a><span data-ttu-id="7f64d-103">Обновление Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="7f64d-103">Update accessReview</span></span>

<span data-ttu-id="7f64d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7f64d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f64d-105">В функции [рецензирования Access](../resources/accessreviews-root.md) в Azure AD обновите существующий объект [акцессревиев](../resources/accessreview.md) , чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="7f64d-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="7f64d-106">Этот API не предназначен для изменения рецензентов или решений проверки.</span><span class="sxs-lookup"><span data-stu-id="7f64d-106">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="7f64d-107">Чтобы изменить проверяющих, используйте API [аддревиевер](accessreview-addreviewer.md) или [ремоверевиевер](accessreview-removereviewer.md) .</span><span class="sxs-lookup"><span data-stu-id="7f64d-107">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="7f64d-108">Чтобы остановить уже начатую проверку или уже запущенный экземпляр повторяющегося рецензирования, используйте API [Stop](accessreview-stop.md) .</span><span class="sxs-lookup"><span data-stu-id="7f64d-108">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="7f64d-109">Чтобы применить решения к целевой группе или правам доступа приложения, используйте API [Apply](accessreview-apply.md) .</span><span class="sxs-lookup"><span data-stu-id="7f64d-109">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="7f64d-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f64d-110">Permissions</span></span>
<span data-ttu-id="7f64d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f64d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f64d-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f64d-113">Permission type</span></span>                        | <span data-ttu-id="7f64d-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f64d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f64d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f64d-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f64d-116">Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7f64d-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="7f64d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f64d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f64d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f64d-118">Not supported.</span></span> |
|<span data-ttu-id="7f64d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f64d-119">Application</span></span>                            | <span data-ttu-id="7f64d-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="7f64d-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f64d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f64d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="7f64d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f64d-122">Request headers</span></span>
| <span data-ttu-id="7f64d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7f64d-123">Name</span></span>         | <span data-ttu-id="7f64d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7f64d-124">Type</span></span>        | <span data-ttu-id="7f64d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7f64d-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7f64d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f64d-126">Authorization</span></span> | <span data-ttu-id="7f64d-127">string</span><span class="sxs-lookup"><span data-stu-id="7f64d-127">string</span></span> | <span data-ttu-id="7f64d-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f64d-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f64d-130">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f64d-130">Request body</span></span>
<span data-ttu-id="7f64d-131">В тексте запроса добавьте представление параметров объекта [акцессревиев](../resources/accessreview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f64d-131">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="7f64d-132">В следующей таблице приведены свойства, которые можно указать при обновлении Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="7f64d-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="7f64d-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f64d-133">Property</span></span>     | <span data-ttu-id="7f64d-134">Тип</span><span class="sxs-lookup"><span data-stu-id="7f64d-134">Type</span></span>        | <span data-ttu-id="7f64d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="7f64d-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="7f64d-136">Имя проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="7f64d-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="7f64d-137">Дата и время, когда выполняется запланированное начало проверки.</span><span class="sxs-lookup"><span data-stu-id="7f64d-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="7f64d-138">Это должна быть Дата в будущем.</span><span class="sxs-lookup"><span data-stu-id="7f64d-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="7f64d-139">Дата и время окончания запланированного рассмотрения.</span><span class="sxs-lookup"><span data-stu-id="7f64d-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="7f64d-140">Это должен быть по крайней мере один день позже даты начала.</span><span class="sxs-lookup"><span data-stu-id="7f64d-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="7f64d-141">Описание, которое будет отображаться для рецензентов.</span><span class="sxs-lookup"><span data-stu-id="7f64d-141">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="7f64d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f64d-142">Response</span></span>
<span data-ttu-id="7f64d-143">В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и объект [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f64d-143">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f64d-144">Пример</span><span class="sxs-lookup"><span data-stu-id="7f64d-144">Example</span></span>

<span data-ttu-id="7f64d-145">Это пример обновления доступа к одноразовой (неповторной) проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="7f64d-145">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="7f64d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f64d-146">Request</span></span>
<span data-ttu-id="7f64d-147">В теле запроса добавьте представление новых свойств объекта [акцессревиев](../resources/accessreview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f64d-147">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="7f64d-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f64d-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7f64d-149">C#</span><span class="sxs-lookup"><span data-stu-id="7f64d-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f64d-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f64d-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f64d-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f64d-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7f64d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f64d-152">Response</span></span>
><span data-ttu-id="7f64d-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f64d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
