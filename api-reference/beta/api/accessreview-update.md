---
title: Обновление accessReview
description: В Azure AD access дается обзор компонента "," Обновление существующий объект accessReview изменение одно или несколько свойств.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e4e74daa092c6f18c845c7f0c468af90385b899b
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016753"
---
# <a name="update-accessreview"></a><span data-ttu-id="a43ec-103">Обновление accessReview</span><span class="sxs-lookup"><span data-stu-id="a43ec-103">Update accessReview</span></span>

> <span data-ttu-id="a43ec-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a43ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a43ec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a43ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a43ec-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [accessReview](../resources/accessreview.md) изменение одно или несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="a43ec-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to change one or more of its properties.</span></span>

<span data-ttu-id="a43ec-107">Этот интерфейс API не предназначен для изменения рецензентов или решения, принимаемые проверки.</span><span class="sxs-lookup"><span data-stu-id="a43ec-107">This API is not intended to change the reviewers or decisions of a review.</span></span>  <span data-ttu-id="a43ec-108">Чтобы изменить рецензентов, используйте [addReviewer](accessreview-addreviewer.md) или [removeReviewer](accessreview-removereviewer.md) API-интерфейсы.</span><span class="sxs-lookup"><span data-stu-id="a43ec-108">To change the reviewers, use the [addReviewer](accessreview-addreviewer.md) or [removeReviewer](accessreview-removereviewer.md) APIs.</span></span>  <span data-ttu-id="a43ec-109">Чтобы остановить одноразовый review уже запущенной или уже запущен экземпляр повторяющейся проверки, раньше, используйте [Остановить](accessreview-stop.md) API.</span><span class="sxs-lookup"><span data-stu-id="a43ec-109">To stop an already-started one-time review, or an already-started instance of a recurring review, early, use the [stop](accessreview-stop.md) API.</span></span> <span data-ttu-id="a43ec-110">Чтобы применить решения для целевой группы или приложения права доступа, используйте [Применение](accessreview-apply.md) API.</span><span class="sxs-lookup"><span data-stu-id="a43ec-110">To apply the decisions to the target group or app access rights, use the [apply](accessreview-apply.md) API.</span></span> 


## <a name="permissions"></a><span data-ttu-id="a43ec-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a43ec-111">Permissions</span></span>
<span data-ttu-id="a43ec-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a43ec-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a43ec-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a43ec-114">Permission type</span></span>                        | <span data-ttu-id="a43ec-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a43ec-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a43ec-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a43ec-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="a43ec-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a43ec-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="a43ec-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a43ec-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a43ec-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a43ec-119">Not supported.</span></span> |
|<span data-ttu-id="a43ec-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a43ec-120">Application</span></span>                            | <span data-ttu-id="a43ec-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a43ec-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a43ec-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a43ec-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="a43ec-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a43ec-123">Request headers</span></span>
| <span data-ttu-id="a43ec-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a43ec-124">Name</span></span>         | <span data-ttu-id="a43ec-125">Тип</span><span class="sxs-lookup"><span data-stu-id="a43ec-125">Type</span></span>        | <span data-ttu-id="a43ec-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a43ec-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a43ec-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a43ec-127">Authorization</span></span> | <span data-ttu-id="a43ec-128">string</span><span class="sxs-lookup"><span data-stu-id="a43ec-128">string</span></span> | <span data-ttu-id="a43ec-129">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="a43ec-129">Bearer \{token\}.</span></span> <span data-ttu-id="a43ec-130">Обязательная часть.</span><span class="sxs-lookup"><span data-stu-id="a43ec-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a43ec-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a43ec-131">Request body</span></span>
<span data-ttu-id="a43ec-132">В тексте запроса укажите представление JSON параметров объекта [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="a43ec-132">In the request body, supply a JSON representation of the parameters of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="a43ec-133">В следующей таблице показаны свойства, которые могут быть предоставлены при обновлении accessReview.</span><span class="sxs-lookup"><span data-stu-id="a43ec-133">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="a43ec-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="a43ec-134">Property</span></span>     | <span data-ttu-id="a43ec-135">Тип</span><span class="sxs-lookup"><span data-stu-id="a43ec-135">Type</span></span>        | <span data-ttu-id="a43ec-136">Описание</span><span class="sxs-lookup"><span data-stu-id="a43ec-136">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="a43ec-137">Имя проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="a43ec-137">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="a43ec-138">Дата и время при планировании проверки быть запуск.</span><span class="sxs-lookup"><span data-stu-id="a43ec-138">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="a43ec-139">Это должно быть даты в будущем.</span><span class="sxs-lookup"><span data-stu-id="a43ec-139">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="a43ec-140">Дата и время после запланированного окончания проверки.</span><span class="sxs-lookup"><span data-stu-id="a43ec-140">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="a43ec-141">Это должно быть более поздней, чем дата начала по крайней мере один день.</span><span class="sxs-lookup"><span data-stu-id="a43ec-141">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="a43ec-142">Описание, чтобы показать рецензентов.</span><span class="sxs-lookup"><span data-stu-id="a43ec-142">The description, to show to the reviewers.</span></span> |



## <a name="response"></a><span data-ttu-id="a43ec-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a43ec-143">Response</span></span>
<span data-ttu-id="a43ec-144">Успешно завершена, этот метод возвращает `204, Accepted` код ответа и объект [accessReview](../resources/accessreview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a43ec-144">If successful, this method returns a `204, Accepted` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a43ec-145">Пример</span><span class="sxs-lookup"><span data-stu-id="a43ec-145">Example</span></span>

<span data-ttu-id="a43ec-146">Это пример обновления одноразовый (не периодические) проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="a43ec-146">This is an example of updating a one-time (not reoccurring) access review.</span></span>

##### <a name="request"></a><span data-ttu-id="a43ec-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="a43ec-147">Request</span></span>
<span data-ttu-id="a43ec-148">В тексте запроса укажите представление JSON новых свойств объекта [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="a43ec-148">In the request body, supply a JSON representation of the new properties of the [accessReview](../resources/accessreview.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="a43ec-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="a43ec-149">Response</span></span>
><span data-ttu-id="a43ec-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a43ec-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
