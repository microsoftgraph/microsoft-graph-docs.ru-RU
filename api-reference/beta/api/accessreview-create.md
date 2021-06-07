---
title: Создание accessReview
description: В функции обзоров доступа Azure AD создайте новый объект accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fd1f6c25dcc4013c1abc3d39dafa63723a1e3ea0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751120"
---
# <a name="create-accessreview"></a><span data-ttu-id="eb041-103">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="eb041-103">Create accessReview</span></span>

<span data-ttu-id="eb041-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb041-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb041-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) создайте новый [объект accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="eb041-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="eb041-106">Прежде чем сделать этот запрос, [](businessflowtemplate-list.md)звонявший должен ранее получить список шаблонов бизнес-потока, чтобы включить в запрос значение **businessFlowTemplateId.**</span><span class="sxs-lookup"><span data-stu-id="eb041-106">Before making this request, the caller must have previously [retrieved the list of business flow templates](businessflowtemplate-list.md), to have the value of **businessFlowTemplateId** to include in the request.</span></span>

<span data-ttu-id="eb041-107">После этого запроса вызываемая должна [создать программуControl,](programcontrol-create.md)чтобы связать обзор доступа с программой.</span><span class="sxs-lookup"><span data-stu-id="eb041-107">After making this request, the caller should [create a programControl](programcontrol-create.md), to link the access review to a program.</span></span>  

## <a name="permissions"></a><span data-ttu-id="eb041-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb041-108">Permissions</span></span>

<span data-ttu-id="eb041-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb041-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb041-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb041-111">Permission type</span></span>                        | <span data-ttu-id="eb041-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb041-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb041-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb041-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb041-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb041-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="eb041-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb041-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb041-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb041-116">Not supported.</span></span> |
|<span data-ttu-id="eb041-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="eb041-117">Application</span></span>                            | <span data-ttu-id="eb041-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="eb041-118">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="eb041-119">Вызываемая должна также иметь разрешение ProgramControl.ReadWrite.All, чтобы после создания обзора доступа вызываемая мог создать [программуControl](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="eb041-119">The caller should also have ProgramControl.ReadWrite.All permission, so that after creating an access review, the caller can create a [programControl](../resources/programcontrol.md).</span></span>
<span data-ttu-id="eb041-120">Кроме того, подписанный пользователь также должен быть в роли каталога, что позволяет им создавать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="eb041-120">In addition, the signed in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="eb041-121">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviews-root.md)</span><span class="sxs-lookup"><span data-stu-id="eb041-121">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="eb041-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb041-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a><span data-ttu-id="eb041-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb041-123">Request headers</span></span>
| <span data-ttu-id="eb041-124">Имя</span><span class="sxs-lookup"><span data-stu-id="eb041-124">Name</span></span>         | <span data-ttu-id="eb041-125">Описание</span><span class="sxs-lookup"><span data-stu-id="eb041-125">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="eb041-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb041-126">Authorization</span></span> | <span data-ttu-id="eb041-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb041-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="eb041-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb041-129">Content-type</span></span> | <span data-ttu-id="eb041-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb041-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb041-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb041-132">Request body</span></span>
<span data-ttu-id="eb041-133">В теле запроса поставляем представление JSON объекта [accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="eb041-133">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="eb041-134">В следующей таблице показаны свойства, необходимые при создании accessReview.</span><span class="sxs-lookup"><span data-stu-id="eb041-134">The following table shows the properties that are required when you create an accessReview.</span></span>

| <span data-ttu-id="eb041-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb041-135">Property</span></span>     | <span data-ttu-id="eb041-136">Тип</span><span class="sxs-lookup"><span data-stu-id="eb041-136">Type</span></span>        | <span data-ttu-id="eb041-137">Описание</span><span class="sxs-lookup"><span data-stu-id="eb041-137">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eb041-138">displayName</span><span class="sxs-lookup"><span data-stu-id="eb041-138">displayName</span></span>             |<span data-ttu-id="eb041-139">String</span><span class="sxs-lookup"><span data-stu-id="eb041-139">String</span></span>                                                        | <span data-ttu-id="eb041-140">Имя обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="eb041-140">The access review name.</span></span>  |
| <span data-ttu-id="eb041-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="eb041-141">startDateTime</span></span>           |<span data-ttu-id="eb041-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb041-142">DateTimeOffset</span></span>                                                | <span data-ttu-id="eb041-143">DateTime, когда планируется начать проверку.</span><span class="sxs-lookup"><span data-stu-id="eb041-143">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="eb041-144">Это должна быть дата в будущем.</span><span class="sxs-lookup"><span data-stu-id="eb041-144">This must be a date in the future.</span></span>   |
| <span data-ttu-id="eb041-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="eb041-145">endDateTime</span></span>             |<span data-ttu-id="eb041-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb041-146">DateTimeOffset</span></span>                                                | <span data-ttu-id="eb041-147">DateTime, когда проверка должна завершиться.</span><span class="sxs-lookup"><span data-stu-id="eb041-147">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="eb041-148">Это должно быть по крайней мере на один день позже даты начала.</span><span class="sxs-lookup"><span data-stu-id="eb041-148">This must be at least one day later than the start date.</span></span>   |
| <span data-ttu-id="eb041-149">description</span><span class="sxs-lookup"><span data-stu-id="eb041-149">description</span></span>             |<span data-ttu-id="eb041-150">String</span><span class="sxs-lookup"><span data-stu-id="eb041-150">String</span></span>                                                        | <span data-ttu-id="eb041-151">Описание, чтобы показать рецензентам.</span><span class="sxs-lookup"><span data-stu-id="eb041-151">The description, to show to the reviewers.</span></span> |
| <span data-ttu-id="eb041-152">businessFlowTemplateId</span><span class="sxs-lookup"><span data-stu-id="eb041-152">businessFlowTemplateId</span></span>  |<span data-ttu-id="eb041-153">String</span><span class="sxs-lookup"><span data-stu-id="eb041-153">String</span></span>                                                        | <span data-ttu-id="eb041-154">Идентификатор шаблона бизнес-потока, полученный из [businessFlowTemplate.](../resources/businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="eb041-154">The business flow template identifier, obtained from a [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span>  |
| <span data-ttu-id="eb041-155">reviewerType</span><span class="sxs-lookup"><span data-stu-id="eb041-155">reviewerType</span></span>            |<span data-ttu-id="eb041-156">String</span><span class="sxs-lookup"><span data-stu-id="eb041-156">String</span></span>                                                        | <span data-ttu-id="eb041-157">Тип отношения рецензента к правам доступа к рассмотренного объекта, одного из `self` , `delegated` или `entityOwners` .</span><span class="sxs-lookup"><span data-stu-id="eb041-157">The relationship type of reviewer to the access rights of the reviewed object, one of `self`, `delegated`, or `entityOwners`.</span></span> | 
| <span data-ttu-id="eb041-158">reviewedEntity</span><span class="sxs-lookup"><span data-stu-id="eb041-158">reviewedEntity</span></span>          |[<span data-ttu-id="eb041-159">identity</span><span class="sxs-lookup"><span data-stu-id="eb041-159">identity</span></span>](../resources/identity.md)                                     | <span data-ttu-id="eb041-160">Объект, для которого создается обзор доступа, например членство в группе или назначения пользователей приложению.</span><span class="sxs-lookup"><span data-stu-id="eb041-160">The object for which an access review is created, such as the membership of a group or the assignments of users to an application.</span></span> | 


<span data-ttu-id="eb041-161">Если **reviewerType** имеет значение, то вызывавший должен также включать свойство рецензентов с коллекцией объектов `delegated` [userIdentity,](../resources/useridentity.md) представляющих рецензентов. </span><span class="sxs-lookup"><span data-stu-id="eb041-161">If the **reviewerType** has the value `delegated`, then the caller must also include the **reviewers** property, with a collection of [userIdentity](../resources/useridentity.md) objects representing the reviewers.</span></span>

<span data-ttu-id="eb041-162">Если приложение вызывает этот API без подписанного пользователя, вызываемая должна также включать свойство **createdBy,** значение для которого является [объектом userIdentity](../resources/useridentity.md) пользователя, который будет определен в качестве создателя отзыва.</span><span class="sxs-lookup"><span data-stu-id="eb041-162">If your app is calling this API without a signed-in user, then the caller must also include the **createdBy** property, the value for which is a [userIdentity](../resources/useridentity.md) of the user who will be identified as the creator of the review.</span></span>

<span data-ttu-id="eb041-163">Кроме того, вызывающее может включать **параметры,** чтобы создать повторяющиеся серии обзоров или изменить поведение проверки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="eb041-163">In addition, the caller can include **settings**, to create a recurring review series or to change from the default review behavior.</span></span> <span data-ttu-id="eb041-164">В частности, чтобы создать повторяющийся обзор, звонящая должна включить [accessReviewRecurrenceSettings](../resources/accessreviewrecurrencesettings.md) в параметры обзора доступа,</span><span class="sxs-lookup"><span data-stu-id="eb041-164">In particular, to create a recurring review, the caller must include the [accessReviewRecurrenceSettings](../resources/accessreviewrecurrencesettings.md) within the access review settings,</span></span>


## <a name="response"></a><span data-ttu-id="eb041-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb041-165">Response</span></span>
<span data-ttu-id="eb041-166">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект accessReview](../resources/accessreview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="eb041-166">If successful, this method returns a `201 Created` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb041-167">Пример</span><span class="sxs-lookup"><span data-stu-id="eb041-167">Example</span></span>

<span data-ttu-id="eb041-168">Это пример создания разового (не повторяющегося) обзора доступа, явно указывав двух пользователей в качестве рецензентов.</span><span class="sxs-lookup"><span data-stu-id="eb041-168">This is an example of creating a one-time (not recurring) access review, explicitly specifying two users as the reviewers.</span></span>

### <a name="request"></a><span data-ttu-id="eb041-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb041-169">Request</span></span>
<span data-ttu-id="eb041-170">В теле запроса поставляем JSON-представление [объекта accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="eb041-170">In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb041-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb041-171">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eb041-172">C#</span><span class="sxs-lookup"><span data-stu-id="eb041-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb041-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb041-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb041-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb041-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb041-175">Java</span><span class="sxs-lookup"><span data-stu-id="eb041-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb041-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb041-176">Response</span></span>
><span data-ttu-id="eb041-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eb041-177">**Note:** The response object shown here might be shortened for readability.</span></span>
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


