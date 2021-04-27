---
title: Создание accessReviewScheduleDefinition
description: Создайте новый объект accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a26c081af41658cebcff1db5d1608907f5b25034
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048374"
---
# <a name="create-accessreviewscheduledefinition"></a><span data-ttu-id="80cf0-103">Создание accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="80cf0-103">Create accessReviewScheduleDefinition</span></span>

<span data-ttu-id="80cf0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80cf0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80cf0-105">Создайте новый [объект accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="80cf0-105">Create a new [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80cf0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80cf0-106">Permissions</span></span>

<span data-ttu-id="80cf0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80cf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80cf0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80cf0-109">Permission type</span></span>                        | <span data-ttu-id="80cf0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80cf0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="80cf0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80cf0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="80cf0-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80cf0-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="80cf0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80cf0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80cf0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80cf0-114">Not supported.</span></span>|
|<span data-ttu-id="80cf0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="80cf0-115">Application</span></span>                            | <span data-ttu-id="80cf0-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80cf0-116">AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="80cf0-117">При входе пользователь должен также быть в роли каталога, что позволяет им создавать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="80cf0-117">The signed-in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="80cf0-118">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="80cf0-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="80cf0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80cf0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="80cf0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80cf0-120">Request headers</span></span>
| <span data-ttu-id="80cf0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="80cf0-121">Name</span></span>         | <span data-ttu-id="80cf0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="80cf0-122">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="80cf0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80cf0-123">Authorization</span></span>|<span data-ttu-id="80cf0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80cf0-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="80cf0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="80cf0-126">Content-type</span></span> | <span data-ttu-id="80cf0-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80cf0-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80cf0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80cf0-129">Request body</span></span>
<span data-ttu-id="80cf0-130">В теле запроса поставляем представление JSON объекта [accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="80cf0-130">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="80cf0-131">В следующей таблице показаны свойства, принятые для создания accessReview.</span><span class="sxs-lookup"><span data-stu-id="80cf0-131">The following table shows the properties accepted to create an accessReview.</span></span>

| <span data-ttu-id="80cf0-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="80cf0-132">Property</span></span> | <span data-ttu-id="80cf0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="80cf0-133">Type</span></span> | <span data-ttu-id="80cf0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="80cf0-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="80cf0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="80cf0-135">displayName</span></span> | <span data-ttu-id="80cf0-136">String</span><span class="sxs-lookup"><span data-stu-id="80cf0-136">String</span></span> | <span data-ttu-id="80cf0-137">Имя серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="80cf0-137">Name of access review series.</span></span> <span data-ttu-id="80cf0-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80cf0-138">Required.</span></span>|
| <span data-ttu-id="80cf0-139">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="80cf0-139">descriptionForAdmins</span></span> | <span data-ttu-id="80cf0-140">String</span><span class="sxs-lookup"><span data-stu-id="80cf0-140">string</span></span> | <span data-ttu-id="80cf0-141">Контекст обзора, предоставленного администраторам.</span><span class="sxs-lookup"><span data-stu-id="80cf0-141">Context of the review provided to admins.</span></span> <span data-ttu-id="80cf0-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80cf0-142">Required.</span></span> |
  <span data-ttu-id="80cf0-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="80cf0-143">descriptionForReviewers</span></span> | <span data-ttu-id="80cf0-144">String</span><span class="sxs-lookup"><span data-stu-id="80cf0-144">string</span></span> | <span data-ttu-id="80cf0-145">Контекст обзора, предоставленного рецензентам.</span><span class="sxs-lookup"><span data-stu-id="80cf0-145">Context of the review provided to reviewers.</span></span> <span data-ttu-id="80cf0-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80cf0-146">Required.</span></span> |
| <span data-ttu-id="80cf0-147">область</span><span class="sxs-lookup"><span data-stu-id="80cf0-147">scope</span></span> | [<span data-ttu-id="80cf0-148">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="80cf0-148">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="80cf0-149">Определяет область пользователей, рассмотренных в группе.</span><span class="sxs-lookup"><span data-stu-id="80cf0-149">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="80cf0-150">См.  [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="80cf0-150">See  [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="80cf0-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80cf0-151">Required.</span></span>| 
| <span data-ttu-id="80cf0-152">instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="80cf0-152">instanceEnumerationScope</span></span> | [<span data-ttu-id="80cf0-153">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="80cf0-153">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="80cf0-154">В случае проверки всех групп определяется область, в которой будут рассмотрены группы.</span><span class="sxs-lookup"><span data-stu-id="80cf0-154">In the case of an all groups review, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="80cf0-155">См. [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="80cf0-155">See [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> | 
| <span data-ttu-id="80cf0-156">settings</span><span class="sxs-lookup"><span data-stu-id="80cf0-156">settings</span></span> | [<span data-ttu-id="80cf0-157">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="80cf0-157">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="80cf0-158">Параметры для серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="80cf0-158">The settings for an access review series.</span></span> <span data-ttu-id="80cf0-159">Здесь определяется повторяемость.</span><span class="sxs-lookup"><span data-stu-id="80cf0-159">Recurrence is determined here.</span></span> <span data-ttu-id="80cf0-160">См. [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="80cf0-160">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="80cf0-161">рецензенты</span><span class="sxs-lookup"><span data-stu-id="80cf0-161">reviewers</span></span> | <span data-ttu-id="80cf0-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="80cf0-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span> | <span data-ttu-id="80cf0-163">Определяет, кто такие рецензенты.</span><span class="sxs-lookup"><span data-stu-id="80cf0-163">Defines who the reviewers are.</span></span> <span data-ttu-id="80cf0-164">Если нет указаны, обзор является самообнаверяемой (пользователи рассмотрели обзор собственного доступа).</span><span class="sxs-lookup"><span data-stu-id="80cf0-164">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="80cf0-165">См. [accessReviewReviewerScope.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="80cf0-165">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |


## <a name="response"></a><span data-ttu-id="80cf0-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="80cf0-166">Response</span></span>
<span data-ttu-id="80cf0-167">В случае успешной работы этот метод возвращает код ответа и `201, Created` [объект accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="80cf0-167">If successful, this method returns a `201, Created` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80cf0-168">Примеры</span><span class="sxs-lookup"><span data-stu-id="80cf0-168">Examples</span></span>

<span data-ttu-id="80cf0-169">Это пример создания серии обзоров доступа с определенным пользователем, имя объекта пользователя которого 7eae4444-d425-48b2-adf2-3c777f6256f3, как рецензент.</span><span class="sxs-lookup"><span data-stu-id="80cf0-169">This is an example of creating an access review series with a specific user, whose user object id is 7eae4444-d425-48b2-adf2-3c777f6256f3, as the reviewer.</span></span> <span data-ttu-id="80cf0-170">В обзоре рассматриваются все члены определенной группы, чьи групповой объектный id b7a059cb-038a-4802-8fc9-b9d1ed0c4444.</span><span class="sxs-lookup"><span data-stu-id="80cf0-170">The review reviews all members of a specific group, whose group object id is b7a059cb-038a-4802-8fc9-b9d1ed0c4444.</span></span> <span data-ttu-id="80cf0-171">Он повторяется еженедельно.</span><span class="sxs-lookup"><span data-stu-id="80cf0-171">It recurs weekly.</span></span>

### <a name="request"></a><span data-ttu-id="80cf0-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="80cf0-172">Request</span></span>
<span data-ttu-id="80cf0-173">В теле запроса поставляем представление JSON объекта [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="80cf0-173">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="80cf0-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="80cf0-174">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="80cf0-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80cf0-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="80cf0-176">C#</span><span class="sxs-lookup"><span data-stu-id="80cf0-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80cf0-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80cf0-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80cf0-178">Java</span><span class="sxs-lookup"><span data-stu-id="80cf0-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80cf0-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="80cf0-179">Response</span></span>
><span data-ttu-id="80cf0-180">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="80cf0-180">**Note:** The response object shown here might be shortened for readability.</span></span>
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
