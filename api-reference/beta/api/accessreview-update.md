---
title: Обновление accessReview
description: В Azure AD access дается обзор компонента "," Обновление существующий объект accessReview изменение одно или несколько свойств.
ms.openlocfilehash: 8913377db8acea17023605f85d01c8c9ecea419b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076031"
---
# <a name="update-accessreview"></a><span data-ttu-id="01a71-103">Обновление accessReview</span><span class="sxs-lookup"><span data-stu-id="01a71-103">Update accessReview</span></span>

> <span data-ttu-id="01a71-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01a71-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01a71-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01a71-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01a71-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [accessReview](../resources/accessreview.md) изменение одно или несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="01a71-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="01a71-107">Этот интерфейс API не предназначен для изменения рецензентов или решения, принимаемые проверки.</span><span class="sxs-lookup"><span data-stu-id="01a71-107">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="01a71-108">Чтобы изменить рецензентов, используйте [addReviewer](accessreview-addreviewer.md) или [removeReviewer](accessreview-removereviewer.md) API-интерфейсы.</span><span class="sxs-lookup"><span data-stu-id="01a71-108">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="01a71-109">Остановка одноразовый review уже запущенной или уже запущен экземпляр повторяющейся проверки, раньше, использовать [Остановить](accessreview-stop.md) API и применение решения целевой группы или приложения права доступа, используйте [Применение](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="01a71-109">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API, and to apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="01a71-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01a71-110">Permissions</span></span>
<span data-ttu-id="01a71-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01a71-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01a71-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01a71-113">Permission type</span></span>                        | <span data-ttu-id="01a71-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01a71-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="01a71-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01a71-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="01a71-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01a71-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="01a71-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01a71-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01a71-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01a71-118">Not supported.</span></span> |
|<span data-ttu-id="01a71-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01a71-119">Application</span></span>                            | <span data-ttu-id="01a71-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01a71-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01a71-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01a71-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="01a71-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01a71-122">Request headers</span></span>
| <span data-ttu-id="01a71-123">Имя</span><span class="sxs-lookup"><span data-stu-id="01a71-123">Name</span></span>         | <span data-ttu-id="01a71-124">Тип</span><span class="sxs-lookup"><span data-stu-id="01a71-124">Type</span></span>        | <span data-ttu-id="01a71-125">Описание</span><span class="sxs-lookup"><span data-stu-id="01a71-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="01a71-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="01a71-126">Authorization</span></span> | <span data-ttu-id="01a71-127">string</span><span class="sxs-lookup"><span data-stu-id="01a71-127">string</span></span> | <span data-ttu-id="01a71-128">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="01a71-128">Bearer \{token\}.</span></span> <span data-ttu-id="01a71-129">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="01a71-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01a71-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01a71-130">Request body</span></span>
<span data-ttu-id="01a71-131">В тексте запроса укажите представление JSON параметров объекта [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="01a71-131">In the request body, supply a JSON representation of a parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="01a71-132">В следующей таблице показаны свойства, которые могут быть предоставлены при обновлении accessReview.</span><span class="sxs-lookup"><span data-stu-id="01a71-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="01a71-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="01a71-133">Property</span></span>     | <span data-ttu-id="01a71-134">Тип</span><span class="sxs-lookup"><span data-stu-id="01a71-134">Type</span></span>        | <span data-ttu-id="01a71-135">Description</span><span class="sxs-lookup"><span data-stu-id="01a71-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="01a71-136">Имя проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="01a71-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="01a71-137">Дата и время при планировании проверки быть запуск.</span><span class="sxs-lookup"><span data-stu-id="01a71-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="01a71-138">Это должно быть даты в будущем.</span><span class="sxs-lookup"><span data-stu-id="01a71-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="01a71-139">Дата и время после запланированного окончания проверки.</span><span class="sxs-lookup"><span data-stu-id="01a71-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="01a71-140">Это должно быть более поздней, чем дата начала по крайней мере один день.</span><span class="sxs-lookup"><span data-stu-id="01a71-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="01a71-141">Описание, чтобы показать рецензентов.</span><span class="sxs-lookup"><span data-stu-id="01a71-141">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="01a71-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="01a71-142">Response</span></span>
<span data-ttu-id="01a71-143">Успешно завершена, этот метод возвращает `204, Accepted` код ответа и объект [accessReview](../resources/accessreview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="01a71-143">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01a71-144">Пример</span><span class="sxs-lookup"><span data-stu-id="01a71-144">Example</span></span>

<span data-ttu-id="01a71-145">Это пример обновления одноразовый (не периодические) проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="01a71-145">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="01a71-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="01a71-146">Request</span></span>
<span data-ttu-id="01a71-147">В тексте запроса укажите представление JSON новых свойств объекта [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="01a71-147">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="01a71-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="01a71-148">Response</span></span>
><span data-ttu-id="01a71-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01a71-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
