---
title: Создание accessReview
description: В функции обзоров доступа Azure AD создайте новый объект accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8942fc5db772b33ca50f0e71f939c9b04bb8b948
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048514"
---
# <a name="create-accessreview"></a><span data-ttu-id="2953c-103">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="2953c-103">Create accessReview</span></span>

<span data-ttu-id="2953c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2953c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2953c-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) создайте новый [объект accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="2953c-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="2953c-106">Прежде чем сделать этот запрос, [](businessflowtemplate-list.md)звонявший должен ранее получить список шаблонов бизнес-потока, чтобы иметь значение включить `businessFlowTemplateId` в запрос.</span><span class="sxs-lookup"><span data-stu-id="2953c-106">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of `businessFlowTemplateId` to include in the request.</span></span>

<span data-ttu-id="2953c-107">После этого запроса вызываемая должна [создать программуControl,](programcontrol-create.md)чтобы связать обзор доступа с программой.</span><span class="sxs-lookup"><span data-stu-id="2953c-107">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="2953c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2953c-108">Permissions</span></span>

<span data-ttu-id="2953c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2953c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2953c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2953c-111">Permission type</span></span>                        | <span data-ttu-id="2953c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2953c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2953c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2953c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2953c-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2953c-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="2953c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2953c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2953c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2953c-116">Not supported.</span></span> |
|<span data-ttu-id="2953c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2953c-117">Application</span></span>                            | <span data-ttu-id="2953c-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="2953c-118">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="2953c-119">Вызываемая должна также иметь разрешение ProgramControl.ReadWrite.All, чтобы после создания обзора доступа вызываемая мог создать [программуControl](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="2953c-119">The caller should also have ProgramControl.ReadWrite.All permission, so that after creating an access review, the caller can create a [programControl](../resources/programcontrol.md).</span></span>
<span data-ttu-id="2953c-120">Кроме того, подписанный пользователь также должен быть в роли каталога, что позволяет им создавать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="2953c-120">In addition, the signed in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="2953c-121">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviews-root.md)</span><span class="sxs-lookup"><span data-stu-id="2953c-121">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="2953c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2953c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="2953c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2953c-123">Request headers</span></span>
| <span data-ttu-id="2953c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="2953c-124">Name</span></span>         | <span data-ttu-id="2953c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2953c-125">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="2953c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2953c-126">Authorization</span></span> | <span data-ttu-id="2953c-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2953c-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="2953c-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2953c-129">Content-type</span></span> | <span data-ttu-id="2953c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2953c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2953c-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2953c-132">Request body</span></span>
<span data-ttu-id="2953c-133">В теле запроса поставляем представление JSON объекта [accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="2953c-133">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="2953c-134">В следующей таблице показаны свойства, необходимые при создании accessReview.</span><span class="sxs-lookup"><span data-stu-id="2953c-134">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="2953c-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="2953c-135">Property</span></span>     | <span data-ttu-id="2953c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="2953c-136">Type</span></span>        | <span data-ttu-id="2953c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="2953c-137">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | <span data-ttu-id="2953c-138">Имя обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="2953c-138">The access review name.</span></span>  |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="2953c-139">DateTime, когда планируется начать проверку.</span><span class="sxs-lookup"><span data-stu-id="2953c-139">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="2953c-140">Это должна быть дата в будущем.</span><span class="sxs-lookup"><span data-stu-id="2953c-140">This must be a date in the future.</span></span>   |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="2953c-141">DateTime, когда проверка должна завершиться.</span><span class="sxs-lookup"><span data-stu-id="2953c-141">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="2953c-142">Это должно быть по крайней мере на один день позже даты начала.</span><span class="sxs-lookup"><span data-stu-id="2953c-142">This must be at least one day later than the start date.</span></span>   |
| `description`             |`String`                                                        | <span data-ttu-id="2953c-143">Описание, чтобы показать рецензентам.</span><span class="sxs-lookup"><span data-stu-id="2953c-143">The description, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="2953c-144">Идентификатор шаблона бизнес-потока, полученный из [businessFlowTemplate.](../resources/businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="2953c-144">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="2953c-145">Тип отношения рецензента к правам доступа к рассмотренного объекта, одного из `self` , `delegated` или `entityOwners` .</span><span class="sxs-lookup"><span data-stu-id="2953c-145">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="2953c-146">Объект, для которого создается обзор доступа, например членство в группе или назначения пользователей приложению.</span><span class="sxs-lookup"><span data-stu-id="2953c-146">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="2953c-147">Если предоставленный reviewerType имеет значение, то вызываемая должна также включать свойство с коллекцией `delegated` `reviewers` [userIdentity](../resources/useridentity.md) рецензентов.</span><span class="sxs-lookup"><span data-stu-id="2953c-147">If the reviewerType being supplied has the value `delegated`, then the caller must also include the `reviewers` property, with a collection of [userIdentity](../resources/useridentity.md) of the reviewers.</span></span>

<span data-ttu-id="2953c-148">Если приложение вызывает этот API без подписанного пользователя, вызываемая должна также включать свойство **createdBy,** значение для которого является [объектом userIdentity](../resources/useridentity.md) пользователя, который будет определен в качестве создателя отзыва.</span><span class="sxs-lookup"><span data-stu-id="2953c-148">If your app is calling this API without a signed-in user, then the caller must also include the **createdBy** property, the value for which is a [userIdentity](../resources/useridentity.md) of the user who will be identified as the creator of the review.</span></span>

<span data-ttu-id="2953c-149">Кроме того, вызывающее может включать параметры, чтобы создать повторяющиеся серии обзоров или изменить поведение проверки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2953c-149">In addition, the caller can include settings, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="2953c-150">В частности, чтобы создать повторяющийся обзор, вызывающий должен включить параметры обзора `accessReviewRecurrenceSettings` доступа,</span><span class="sxs-lookup"><span data-stu-id="2953c-150">In particular, to create a recurring review, the caller must include the `accessReviewRecurrenceSettings` within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="2953c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2953c-151">Response</span></span>
<span data-ttu-id="2953c-152">В случае успешной работы этот метод возвращает код отклика и `201, Created` [объект accessReview](../resources/accessreview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2953c-152">If successful, this method returns a `201, Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2953c-153">Пример</span><span class="sxs-lookup"><span data-stu-id="2953c-153">Example</span></span>

<span data-ttu-id="2953c-154">Это пример создания разового (не повторяющегося) обзора доступа, явно указывав двух пользователей в качестве рецензентов.</span><span class="sxs-lookup"><span data-stu-id="2953c-154">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

### <a name="request"></a><span data-ttu-id="2953c-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="2953c-155">Request</span></span>
<span data-ttu-id="2953c-156">В теле запроса поставляем JSON-представление [объекта accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="2953c-156">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="2953c-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="2953c-157">HTTP</span></span>](#tab/http)
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
        "id": "99025615-a0b1-47ec-9117-35377b10998b"
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
# <a name="c"></a>[<span data-ttu-id="2953c-158">C#</span><span class="sxs-lookup"><span data-stu-id="2953c-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2953c-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2953c-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2953c-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2953c-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2953c-161">Java</span><span class="sxs-lookup"><span data-stu-id="2953c-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2953c-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="2953c-162">Response</span></span>
><span data-ttu-id="2953c-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2953c-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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


