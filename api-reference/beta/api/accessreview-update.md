---
title: Обновление accessReview
description: В Azure AD access дается обзор компонента "," Обновление существующий объект accessReview изменение одно или несколько свойств.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1256ccdabea8eb5c0c0ffb3365e0c87276999236
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524368"
---
# <a name="update-accessreview"></a><span data-ttu-id="0a9c7-103">Обновление accessReview</span><span class="sxs-lookup"><span data-stu-id="0a9c7-103">Update accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a9c7-104">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [accessReview](../resources/accessreview.md) изменение одно или несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="0a9c7-105">Этот интерфейс API не предназначен для изменения рецензентов или решения, принимаемые проверки.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-105">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="0a9c7-106">Чтобы изменить рецензентов, используйте [addReviewer](accessreview-addreviewer.md) или [removeReviewer](accessreview-removereviewer.md) API-интерфейсы.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-106">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="0a9c7-107">Чтобы остановить одноразовый review уже запущенной или уже запущен экземпляр повторяющейся проверки, раньше, используйте [Остановить](accessreview-stop.md) API.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-107">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="0a9c7-108">Чтобы применить решения для целевой группы или приложения права доступа, используйте [Применение](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-108">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="0a9c7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a9c7-109">Permissions</span></span>
<span data-ttu-id="0a9c7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a9c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a9c7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a9c7-112">Permission type</span></span>                        | <span data-ttu-id="0a9c7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a9c7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a9c7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a9c7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a9c7-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a9c7-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="0a9c7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a9c7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a9c7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-117">Not supported.</span></span> |
|<span data-ttu-id="0a9c7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a9c7-118">Application</span></span>                            | <span data-ttu-id="0a9c7-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a9c7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a9c7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="0a9c7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a9c7-121">Request headers</span></span>
| <span data-ttu-id="0a9c7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0a9c7-122">Name</span></span>         | <span data-ttu-id="0a9c7-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0a9c7-123">Type</span></span>        | <span data-ttu-id="0a9c7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0a9c7-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0a9c7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a9c7-125">Authorization</span></span> | <span data-ttu-id="0a9c7-126">string</span><span class="sxs-lookup"><span data-stu-id="0a9c7-126">string</span></span> | <span data-ttu-id="0a9c7-127">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="0a9c7-127">Bearer \{token\}.</span></span> <span data-ttu-id="0a9c7-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a9c7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a9c7-129">Request body</span></span>
<span data-ttu-id="0a9c7-130">В тексте запроса укажите представление JSON параметров объекта [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="0a9c7-130">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="0a9c7-131">В следующей таблице показаны свойства, которые могут быть предоставлены при обновлении accessReview.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="0a9c7-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a9c7-132">Property</span></span>     | <span data-ttu-id="0a9c7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0a9c7-133">Type</span></span>        | <span data-ttu-id="0a9c7-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0a9c7-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="0a9c7-135">Имя проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="0a9c7-136">Дата и время при планировании проверки быть запуск.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="0a9c7-137">Это должно быть даты в будущем.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="0a9c7-138">Дата и время после запланированного окончания проверки.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="0a9c7-139">Это должно быть более поздней, чем дата начала по крайней мере один день.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="0a9c7-140">Описание, чтобы показать рецензентов.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-140">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="0a9c7-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a9c7-141">Response</span></span>
<span data-ttu-id="0a9c7-142">Успешно завершена, этот метод возвращает `204, Accepted` код ответа и объект [accessReview](../resources/accessreview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-142">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a9c7-143">Пример</span><span class="sxs-lookup"><span data-stu-id="0a9c7-143">Example</span></span>

<span data-ttu-id="0a9c7-144">Это пример обновления одноразовый (не периодические) проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-144">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="0a9c7-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a9c7-145">Request</span></span>
<span data-ttu-id="0a9c7-146">В тексте запроса укажите представление JSON новых свойств объекта [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="0a9c7-146">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews('006111db-0810-4494-a6df-904d368bd81b')
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```

##### <a name="response"></a><span data-ttu-id="0a9c7-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a9c7-147">Response</span></span>
><span data-ttu-id="0a9c7-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a9c7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/accessreview-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
