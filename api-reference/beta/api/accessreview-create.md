---
title: Создание accessReview
description: В Azure AD доступа к функции проверки, создайте новый объект accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: de8574566a8ca1eedb1f0f55230fb91053370ccc
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016725"
---
# <a name="create-accessreview"></a><span data-ttu-id="8d464-103">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="8d464-103">Create accessReview</span></span>

> <span data-ttu-id="8d464-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8d464-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d464-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d464-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d464-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD создайте новый объект [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="8d464-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="8d464-107">Перед выполнением этого запроса, вызывающий должен иметь ранее [извлекается список бизнес-поток шаблонов](businessflowtemplate-list.md), иметь значение `businessFlowTemplateId` необходимо включить в запрос.</span><span class="sxs-lookup"><span data-stu-id="8d464-107">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="8d464-108">После выполнения этого запроса, вызывающего следует [Создать programControl](programcontrol-create.md), чтобы связать с программой проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="8d464-108">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="8d464-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d464-109">Permissions</span></span>
<span data-ttu-id="8d464-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d464-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d464-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d464-112">Permission type</span></span>                        | <span data-ttu-id="8d464-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d464-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d464-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d464-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d464-115">AccessReview.ReadWrite.All, а также должны иметь ProgramControl.ReadWrite.All для выполнения сценария с последующих вызовов для создания programControl</span><span class="sxs-lookup"><span data-stu-id="8d464-115">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with the subsequent call to create a programControl</span></span> |
|<span data-ttu-id="8d464-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d464-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d464-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d464-117">Not supported.</span></span> |
|<span data-ttu-id="8d464-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d464-118">Application</span></span>                            | <span data-ttu-id="8d464-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d464-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d464-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d464-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="8d464-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d464-121">Request headers</span></span>
| <span data-ttu-id="8d464-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8d464-122">Name</span></span>         | <span data-ttu-id="8d464-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8d464-123">Type</span></span>        | <span data-ttu-id="8d464-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8d464-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8d464-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d464-125">Authorization</span></span> | <span data-ttu-id="8d464-126">string</span><span class="sxs-lookup"><span data-stu-id="8d464-126">string</span></span> | <span data-ttu-id="8d464-127">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="8d464-127">Bearer \{token\}.</span></span> <span data-ttu-id="8d464-128">Обязательная часть.</span><span class="sxs-lookup"><span data-stu-id="8d464-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d464-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d464-129">Request body</span></span>
<span data-ttu-id="8d464-130">В тексте запроса укажите представление JSON объекта [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="8d464-130">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="8d464-131">В следующей таблице показаны свойства, которые необходимы для создания accessReview.</span><span class="sxs-lookup"><span data-stu-id="8d464-131">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="8d464-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d464-132">Property</span></span>     | <span data-ttu-id="8d464-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8d464-133">Type</span></span>        | <span data-ttu-id="8d464-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8d464-134">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="8d464-135">Имя проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="8d464-135">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="8d464-136">Дата и время при планировании проверки быть запуск.</span><span class="sxs-lookup"><span data-stu-id="8d464-136">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="8d464-137">Это должно быть даты в будущем.</span><span class="sxs-lookup"><span data-stu-id="8d464-137">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="8d464-138">Дата и время после запланированного окончания проверки.</span><span class="sxs-lookup"><span data-stu-id="8d464-138">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="8d464-139">Это должно быть более поздней, чем дата начала по крайней мере один день.</span><span class="sxs-lookup"><span data-stu-id="8d464-139">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="8d464-140">Описание, чтобы показать рецензентов.</span><span class="sxs-lookup"><span data-stu-id="8d464-140">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="8d464-141">Business поток идентификатор шаблона, полученный из [businessFlowTemplate](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="8d464-141">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="8d464-142">Тип отношения рецензент права доступа проверенные объекта, один из `self`, `delegated`, или `entityOwners`.</span><span class="sxs-lookup"><span data-stu-id="8d464-142">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="8d464-143">Объект, для которого создается проверки доступа, например, членство в группе или назначения пользователей в приложение.</span><span class="sxs-lookup"><span data-stu-id="8d464-143">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="8d464-144">Если значение равно reviewerType, указанное `delegated`, а затем вызывающий объект должен также включать `reviewers` свойство с семейством [удостоверению пользователя](../resources/useridentity.md) рецензентов.</span><span class="sxs-lookup"><span data-stu-id="8d464-144">If the reviewerType being supplied has the value `delegated`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="8d464-145">Кроме того вызывающего может включать параметры для создания серии повторяющихся review или для изменения поведения проверки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8d464-145">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="8d464-146">В частности, для создания повторяющихся review вызывающего необходимо включить `accessReviewRecurrenceSettings` в access Проверьте параметры,</span><span class="sxs-lookup"><span data-stu-id="8d464-146">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="8d464-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d464-147">Response</span></span>
<span data-ttu-id="8d464-148">Успешно завершена, этот метод возвращает `201, Created` код ответа и объект [accessReview](../resources/accessreview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8d464-148">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d464-149">Пример</span><span class="sxs-lookup"><span data-stu-id="8d464-149">Example</span></span>

<span data-ttu-id="8d464-150">Это пример создания одноразовый (не повторяющееся) доступа проверки, явно указание двух пользователей в качестве рецензентов.</span><span class="sxs-lookup"><span data-stu-id="8d464-150">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="8d464-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d464-151">Request</span></span>
<span data-ttu-id="8d464-152">В тексте запроса укажите представление объекта [accessReview](../resources/accessreview.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="8d464-152">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b",
    },
    "reviewerType" : "delegated",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval":true,
        "autoReviewEnabled":false,
        "activityDurationInDays":30,
        "autoApplyReviewResultsEnabled":false,
        "accessRecommendationsEnabled":false,
        "recurrenceSettings":{
            "recurrenceType":"onetime",
            "recurrenceEndType":"endBy",
            "durationInDays":0,
            "recurrenceCount":0
        },
        "autoReviewSettings":{
            "notReviewedResult":"Deny"
        }
    }
}
```

##### <a name="response"></a><span data-ttu-id="8d464-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d464-153">Response</span></span>
><span data-ttu-id="8d464-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d464-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
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
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
