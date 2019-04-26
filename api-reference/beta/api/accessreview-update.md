---
title: Обновление Акцессревиев
description: В функции рецензирования Access в Azure AD обновите существующий объект Акцессревиев, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b1c2c1fc0ea94c7d595725fbcc303e1534b1c204
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323009"
---
# <a name="update-accessreview"></a><span data-ttu-id="d8025-103">Обновление Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="d8025-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8025-104">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD обновите существующий объект [акцессревиев](../resources/accessreview.md) , чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="d8025-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="d8025-105">Этот API не предназначен для изменения рецензентов или решений проверки.</span><span class="sxs-lookup"><span data-stu-id="d8025-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="d8025-106">Чтобы изменить проверяющих, используйте API [аддревиевер](accessreview-addreviewer.md) или [ремоверевиевер](accessreview-removereviewer.md) .</span><span class="sxs-lookup"><span data-stu-id="d8025-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="d8025-107">Чтобы остановить уже начатую проверку или уже запущенный экземпляр повторяющегося рецензирования, используйте API [Stop](accessreview-stop.md) .</span><span class="sxs-lookup"><span data-stu-id="d8025-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="d8025-108">Чтобы применить решения к целевой группе или правам доступа приложения, используйте API [Apply](accessreview-apply.md) .</span><span class="sxs-lookup"><span data-stu-id="d8025-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="d8025-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8025-109">Permissions</span></span>
<span data-ttu-id="d8025-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8025-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8025-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8025-112">Permission type</span></span>                        | <span data-ttu-id="d8025-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8025-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8025-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8025-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8025-115">Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d8025-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d8025-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8025-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8025-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8025-117">Not supported.</span></span> |
|<span data-ttu-id="d8025-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8025-118">Application</span></span>                            | <span data-ttu-id="d8025-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8025-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8025-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8025-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="d8025-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8025-121">Request headers</span></span>
| <span data-ttu-id="d8025-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d8025-122">Name</span></span>         | <span data-ttu-id="d8025-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d8025-123">Type</span></span>        | <span data-ttu-id="d8025-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d8025-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d8025-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8025-125">Authorization</span></span> | <span data-ttu-id="d8025-126">string</span><span class="sxs-lookup"><span data-stu-id="d8025-126">string</span></span> | <span data-ttu-id="d8025-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8025-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8025-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8025-129">Request body</span></span>
<span data-ttu-id="d8025-130">В тексте запроса добавьте представление параметров объекта [Акцессревиев](../resources/accessreview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8025-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="d8025-131">В следующей таблице приведены свойства, которые можно указать при обновлении Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="d8025-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="d8025-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8025-132">Property</span></span>     | <span data-ttu-id="d8025-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d8025-133">Type</span></span>        | <span data-ttu-id="d8025-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d8025-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="d8025-135">Имя проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="d8025-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="d8025-136">Дата и время, когда выполняется запланированное начало проверки.</span><span class="sxs-lookup"><span data-stu-id="d8025-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="d8025-137">Это должна быть Дата в будущем.</span><span class="sxs-lookup"><span data-stu-id="d8025-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="d8025-138">Дата и время окончания запланированного рассмотрения.</span><span class="sxs-lookup"><span data-stu-id="d8025-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="d8025-139">Это должен быть по крайней мере один день позже даты начала.</span><span class="sxs-lookup"><span data-stu-id="d8025-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="d8025-140">Описание, которое будет отображаться для рецензентов.</span><span class="sxs-lookup"><span data-stu-id="d8025-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="d8025-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8025-141">Response</span></span>
<span data-ttu-id="d8025-142">В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и объект [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8025-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8025-143">Пример</span><span class="sxs-lookup"><span data-stu-id="d8025-143">Example</span></span>

<span data-ttu-id="d8025-144">Это пример обновления доступа к одноразовой (неповторной) проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="d8025-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="d8025-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8025-145">Request</span></span>
<span data-ttu-id="d8025-146">В теле запроса добавьте представление новых свойств объекта [Акцессревиев](../resources/accessreview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8025-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="d8025-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8025-147">Response</span></span>
><span data-ttu-id="d8025-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8025-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
