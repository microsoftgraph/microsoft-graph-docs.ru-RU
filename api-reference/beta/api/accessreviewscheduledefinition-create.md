---
title: Создание accessReviewScheduleDefinition
description: Создание объекта accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0a3b9d7f9f4513bb92d7f5ba2de66a83fee8e233
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981188"
---
# <a name="create-accessreviewscheduledefinition"></a><span data-ttu-id="63a45-103">Создание accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="63a45-103">Create accessReviewScheduleDefinition</span></span>

<span data-ttu-id="63a45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63a45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63a45-105">Создание объекта [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="63a45-105">Create a new [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="63a45-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63a45-106">Permissions</span></span>

<span data-ttu-id="63a45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63a45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63a45-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63a45-109">Permission type</span></span>                        | <span data-ttu-id="63a45-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63a45-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="63a45-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63a45-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="63a45-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63a45-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="63a45-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63a45-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63a45-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63a45-114">Not supported.</span></span>|
|<span data-ttu-id="63a45-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="63a45-115">Application</span></span>                            | <span data-ttu-id="63a45-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63a45-116">AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="63a45-117">Во входе пользователя также должна быть роль каталога, которая позволяет создать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="63a45-117">The signed-in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="63a45-118">Дополнительные сведения см. в требованиях к роли и разрешениям для [проверки доступа.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="63a45-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="63a45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63a45-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="63a45-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63a45-120">Request headers</span></span>
| <span data-ttu-id="63a45-121">Имя</span><span class="sxs-lookup"><span data-stu-id="63a45-121">Name</span></span>         | <span data-ttu-id="63a45-122">Описание</span><span class="sxs-lookup"><span data-stu-id="63a45-122">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="63a45-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63a45-123">Authorization</span></span>|<span data-ttu-id="63a45-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63a45-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="63a45-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63a45-126">Content-type</span></span> | <span data-ttu-id="63a45-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63a45-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63a45-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63a45-129">Request body</span></span>
<span data-ttu-id="63a45-130">В теле запроса укажу представление объекта [accessReview](../resources/accessreview.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="63a45-130">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="63a45-131">В следующей таблице показаны свойства, принятые для создания accessReview.</span><span class="sxs-lookup"><span data-stu-id="63a45-131">The following table shows the properties accepted to create an accessReview.</span></span>

| <span data-ttu-id="63a45-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="63a45-132">Property</span></span> | <span data-ttu-id="63a45-133">Тип</span><span class="sxs-lookup"><span data-stu-id="63a45-133">Type</span></span> | <span data-ttu-id="63a45-134">Описание</span><span class="sxs-lookup"><span data-stu-id="63a45-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="63a45-135">displayName</span><span class="sxs-lookup"><span data-stu-id="63a45-135">displayName</span></span> | <span data-ttu-id="63a45-136">String</span><span class="sxs-lookup"><span data-stu-id="63a45-136">String</span></span> | <span data-ttu-id="63a45-137">Название серии отзывов о доступе.</span><span class="sxs-lookup"><span data-stu-id="63a45-137">Name of access review series.</span></span> <span data-ttu-id="63a45-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63a45-138">Required.</span></span>|
| <span data-ttu-id="63a45-139">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="63a45-139">descriptionForAdmins</span></span> | <span data-ttu-id="63a45-140">string</span><span class="sxs-lookup"><span data-stu-id="63a45-140">string</span></span> | <span data-ttu-id="63a45-141">Контекст проверки, предоставленной администраторам.</span><span class="sxs-lookup"><span data-stu-id="63a45-141">Context of the review provided to admins.</span></span> <span data-ttu-id="63a45-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63a45-142">Required.</span></span> |
  <span data-ttu-id="63a45-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="63a45-143">descriptionForReviewers</span></span> | <span data-ttu-id="63a45-144">string</span><span class="sxs-lookup"><span data-stu-id="63a45-144">string</span></span> | <span data-ttu-id="63a45-145">Контекст отзыва, предоставленного рецензентам.</span><span class="sxs-lookup"><span data-stu-id="63a45-145">Context of the review provided to reviewers.</span></span> <span data-ttu-id="63a45-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63a45-146">Required.</span></span> |
| <span data-ttu-id="63a45-147">scope</span><span class="sxs-lookup"><span data-stu-id="63a45-147">scope</span></span> | [<span data-ttu-id="63a45-148">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="63a45-148">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="63a45-149">Определяет область пользователей, проверяемую в группе.</span><span class="sxs-lookup"><span data-stu-id="63a45-149">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="63a45-150">См. [accessReviewScope.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="63a45-150">See  [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="63a45-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63a45-151">Required.</span></span>| 
| <span data-ttu-id="63a45-152">instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="63a45-152">instanceEnumerationScope</span></span> | [<span data-ttu-id="63a45-153">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="63a45-153">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="63a45-154">В случае проверки всех групп это определяет область проверки групп.</span><span class="sxs-lookup"><span data-stu-id="63a45-154">In the case of an all groups review, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="63a45-155">См. [accessReviewScope.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="63a45-155">See [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> | 
| <span data-ttu-id="63a45-156">параметры</span><span class="sxs-lookup"><span data-stu-id="63a45-156">settings</span></span> | [<span data-ttu-id="63a45-157">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="63a45-157">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="63a45-158">Параметры для серии отзывов о доступе.</span><span class="sxs-lookup"><span data-stu-id="63a45-158">The settings for an access review series.</span></span> <span data-ttu-id="63a45-159">Здесь определяется повторение.</span><span class="sxs-lookup"><span data-stu-id="63a45-159">Recurrence is determined here.</span></span> <span data-ttu-id="63a45-160">См. [accessReviewScheduleSettings.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="63a45-160">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="63a45-161">рецензенты</span><span class="sxs-lookup"><span data-stu-id="63a45-161">reviewers</span></span> | <span data-ttu-id="63a45-162">[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="63a45-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span> | <span data-ttu-id="63a45-163">Определяет, кто такие рецензенты.</span><span class="sxs-lookup"><span data-stu-id="63a45-163">Defines who the reviewers are.</span></span> <span data-ttu-id="63a45-164">Если ни один из них не указан, отзыв будет самообссвешенным (пользователи просмотрели свой собственный доступ).</span><span class="sxs-lookup"><span data-stu-id="63a45-164">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="63a45-165">См. [accessReviewReviewerScope.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="63a45-165">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |


## <a name="response"></a><span data-ttu-id="63a45-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="63a45-166">Response</span></span>
<span data-ttu-id="63a45-167">В случае успеха этот метод возвращает код отклика и объект `201, Created` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="63a45-167">If successful, this method returns a `201, Created` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63a45-168">Примеры</span><span class="sxs-lookup"><span data-stu-id="63a45-168">Examples</span></span>

<span data-ttu-id="63a45-169">Это пример создания серии отзывов о доступе с определенным пользователем, ид объекта пользователя — 7eae4444-d425-48b2-adf2-3c777f6256f3 в качестве рецензента.</span><span class="sxs-lookup"><span data-stu-id="63a45-169">This is an example of creating an access review series with a specific user, whose user object id is 7eae4444-d425-48b2-adf2-3c777f6256f3, as the reviewer.</span></span> <span data-ttu-id="63a45-170">Проверка проверяет всех членов определенной группы, у которых есть ид объекта группы b7a059cb-038a-4802-8fc9-b9d1ed0c4444.</span><span class="sxs-lookup"><span data-stu-id="63a45-170">The review reviews all members of a specific group, whose group object id is b7a059cb-038a-4802-8fc9-b9d1ed0c4444.</span></span> <span data-ttu-id="63a45-171">Она повторяется еженедельно.</span><span class="sxs-lookup"><span data-stu-id="63a45-171">It recurs weekly.</span></span>

### <a name="request"></a><span data-ttu-id="63a45-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="63a45-172">Request</span></span>
<span data-ttu-id="63a45-173">В теле запроса предопределение представления объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="63a45-173">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="63a45-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="63a45-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Test create",
  "descriptionForAdmins": "New scheduled access review",
  "descriptionForReviewers": "If you have any questions, contact jerry@contoso.com",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0c4444/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [
    {
      "query": "/users/7eae4444-d425-48b2-adf2-3c777f6256f3",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 1,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-08T12:02:30.667Z"
      }
    }
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="63a45-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63a45-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="63a45-176">C#</span><span class="sxs-lookup"><span data-stu-id="63a45-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63a45-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63a45-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63a45-178">Java</span><span class="sxs-lookup"><span data-stu-id="63a45-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63a45-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="63a45-179">Response</span></span>
><span data-ttu-id="63a45-p113">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63a45-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "29f2d16e-9ca6-4052-bbfe-802c48944448",
    "displayName": "Test create",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
    "status": "NotStarted",
    "descriptionForAdmins": "Test create",
    "descriptionForReviewers": "Test create",
    "instanceEnumerationScope": null,
    "createdBy": {
        "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "/groups/b74444cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "/users/7eae986b-d425-48b2-adf2-3c777f4444f3",
            "queryType": "MicrosoftGraph",
            "queryRoot": "decisions"
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 1,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "weekly",
                "interval": 1,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "noEnd",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2020-09-08",
                "endDate": null
            }
        },
        "applyActions": []
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
