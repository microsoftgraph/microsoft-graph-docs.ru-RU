---
title: Создание Акцессревиев
description: В средстве проверки доступа Azure AD создайте новый объект Акцессревиев.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 70dd7e5790c0c6a3a0b4eb99e89aa95423bd5733
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316159"
---
# <a name="create-accessreview"></a><span data-ttu-id="959f5-103">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="959f5-103">Create accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="959f5-104">В средстве проверки [доступа](../resources/accessreviews-root.md) Azure AD создайте новый объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="959f5-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="959f5-105">Перед выполнением этого запроса абонент должен был [получить список шаблонов бизнес-процесса](businessflowtemplate-list.md), чтобы включить в запрос значение `businessFlowTemplateId` для включения в запрос.</span><span class="sxs-lookup"><span data-stu-id="959f5-105">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="959f5-106">После выполнения этого запроса вызывающий абонент должен [создать програмконтрол](programcontrol-create.md), чтобы связать проверку доступа с программой.</span><span class="sxs-lookup"><span data-stu-id="959f5-106">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="959f5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="959f5-107">Permissions</span></span>
<span data-ttu-id="959f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="959f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="959f5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="959f5-110">Permission type</span></span>                        | <span data-ttu-id="959f5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="959f5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="959f5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="959f5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="959f5-113">Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="959f5-113">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="959f5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="959f5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="959f5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="959f5-115">Not supported.</span></span> |
|<span data-ttu-id="959f5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="959f5-116">Application</span></span>                            | <span data-ttu-id="959f5-117">Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="959f5-117">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="959f5-118">Вызывающая сторона также должна иметь разрешение Програмконтрол. ReadWrite. ALL, чтобы после создания проверки доступа вызывающий абонент может создать [програмконтрол](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="959f5-118">The caller should also have ProgramControl.ReadWrite.All permission, so that after creating an access review, the caller can create a [programControl](../resources/programcontrol.md).</span></span>
<span data-ttu-id="959f5-119">Кроме того, пользователь, вошедшего в систему, должен быть членом роли каталога, который позволяет им создавать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="959f5-119">In addition, the signed in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="959f5-120">Более подробную информацию можно узнать в статье требования к ролям и разрешениям для [рецензирования Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="959f5-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="959f5-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="959f5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="959f5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="959f5-122">Request headers</span></span>
| <span data-ttu-id="959f5-123">Имя</span><span class="sxs-lookup"><span data-stu-id="959f5-123">Name</span></span>         | <span data-ttu-id="959f5-124">Тип</span><span class="sxs-lookup"><span data-stu-id="959f5-124">Type</span></span>        | <span data-ttu-id="959f5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="959f5-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="959f5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="959f5-126">Authorization</span></span> | <span data-ttu-id="959f5-127">string</span><span class="sxs-lookup"><span data-stu-id="959f5-127">string</span></span> | <span data-ttu-id="959f5-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="959f5-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="959f5-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="959f5-130">Request body</span></span>
<span data-ttu-id="959f5-131">В тексте запроса добавьте представление объекта [акцессревиев](../resources/accessreview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="959f5-131">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="959f5-132">В следующей таблице приведены свойства, необходимые при создании Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="959f5-132">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="959f5-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="959f5-133">Property</span></span>     | <span data-ttu-id="959f5-134">Тип</span><span class="sxs-lookup"><span data-stu-id="959f5-134">Type</span></span>        | <span data-ttu-id="959f5-135">Описание</span><span class="sxs-lookup"><span data-stu-id="959f5-135">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="959f5-136">Имя проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="959f5-136">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="959f5-137">Дата и время, когда выполняется запланированное начало проверки.</span><span class="sxs-lookup"><span data-stu-id="959f5-137">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="959f5-138">Это должна быть Дата в будущем.</span><span class="sxs-lookup"><span data-stu-id="959f5-138">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="959f5-139">Дата и время окончания запланированного рассмотрения.</span><span class="sxs-lookup"><span data-stu-id="959f5-139">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="959f5-140">Это должен быть по крайней мере один день позже даты начала.</span><span class="sxs-lookup"><span data-stu-id="959f5-140">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="959f5-141">Описание, которое будет отображаться для рецензентов.</span><span class="sxs-lookup"><span data-stu-id="959f5-141">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="959f5-142">Идентификатор шаблона рабочего процесса, полученный из объекта [бусинессфловтемплате](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="959f5-142">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="959f5-143">Тип отношения проверяющего к правам доступа проверенного объекта, один из `self`, `delegated`или. `entityOwners`</span><span class="sxs-lookup"><span data-stu-id="959f5-143">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="959f5-144">Объект, для которого создается проверка доступа, например членство в группе или назначения пользователей приложению.</span><span class="sxs-lookup"><span data-stu-id="959f5-144">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="959f5-145">Если предоставленное значение Ревиевертипе имеет значение `delegated`, вызывающая сторона также должна содержать `reviewers` свойство с коллекцией [userIdentity](../resources/useridentity.md) рецензентов.</span><span class="sxs-lookup"><span data-stu-id="959f5-145">If the reviewerType being supplied has the value `delegated`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="959f5-146">Если приложение вызывает этот API без вошедшего пользователя, вызывающая сторона также должна включать свойство **createdBy** , значение которого является [userIdentity](../resources/useridentity.md) пользователя, который будет идентифицирован как создатель проверки.</span><span class="sxs-lookup"><span data-stu-id="959f5-146">If your app is calling this API without a signed-in user, then the caller must also include the **createdBy** property, the value for which is a [userIdentity](../resources/useridentity.md) of the user who will be identified as the creator of the review.</span></span>

<span data-ttu-id="959f5-147">Кроме того, вызывающий может включать в себя параметры для создания повторяющихся рядов проверки или для изменения поведения проверки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="959f5-147">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="959f5-148">В частности, чтобы создать повторяющуюся проверку, вызывающая сторона должна включать в себя `accessReviewRecurrenceSettings` параметры проверки доступа,</span><span class="sxs-lookup"><span data-stu-id="959f5-148">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="959f5-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="959f5-149">Response</span></span>
<span data-ttu-id="959f5-150">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="959f5-150">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="959f5-151">Пример</span><span class="sxs-lookup"><span data-stu-id="959f5-151">Example</span></span>

<span data-ttu-id="959f5-152">Это пример создания одноразовой (не повторяющейся) проверки доступа, явно указав двух пользователей в качестве проверяющих.</span><span class="sxs-lookup"><span data-stu-id="959f5-152">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

##### <a name="request"></a><span data-ttu-id="959f5-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="959f5-153">Request</span></span>
<span data-ttu-id="959f5-154">В тексте запроса добавьте представление объекта [акцессревиев](../resources/accessreview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="959f5-154">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="959f5-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="959f5-155">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="959f5-156">C#</span><span class="sxs-lookup"><span data-stu-id="959f5-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="959f5-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="959f5-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="959f5-158">Цель — C</span><span class="sxs-lookup"><span data-stu-id="959f5-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="959f5-159">Java</span><span class="sxs-lookup"><span data-stu-id="959f5-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="959f5-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="959f5-160">Response</span></span>
><span data-ttu-id="959f5-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="959f5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
