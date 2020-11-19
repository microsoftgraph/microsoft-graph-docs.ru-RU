---
title: Создание Акцессревиевсчедуледефинитион
description: Создание нового объекта Акцессревиевсчедуледефинитион.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dc30208652af0989ab0b6bf0b35ebfdd50bc65d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221857"
---
# <a name="create-accessreviewscheduledefinition"></a><span data-ttu-id="a542a-103">Создание Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="a542a-103">Create accessReviewScheduleDefinition</span></span>

<span data-ttu-id="a542a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a542a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a542a-105">Создание нового объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="a542a-105">Create a new [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a542a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a542a-106">Permissions</span></span>

<span data-ttu-id="a542a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a542a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a542a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a542a-109">Permission type</span></span>                        | <span data-ttu-id="a542a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a542a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a542a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a542a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a542a-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a542a-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="a542a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a542a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a542a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a542a-114">Not supported.</span></span>|
|<span data-ttu-id="a542a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a542a-115">Application</span></span>                            | <span data-ttu-id="a542a-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a542a-116">AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="a542a-117">Вошедшего в систему пользователя также должен находиться в роли каталога, позволяющей им создавать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="a542a-117">The signed-in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="a542a-118">Более подробную информацию можно узнать в статье требования к ролям и разрешениям для [рецензирования Access](../resources/accessreviewsv2-root.md).</span><span class="sxs-lookup"><span data-stu-id="a542a-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="a542a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a542a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="a542a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a542a-120">Request headers</span></span>
| <span data-ttu-id="a542a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a542a-121">Name</span></span>         | <span data-ttu-id="a542a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a542a-122">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="a542a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a542a-123">Authorization</span></span>|<span data-ttu-id="a542a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a542a-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a542a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a542a-126">Content-type</span></span> | <span data-ttu-id="a542a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a542a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a542a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a542a-129">Request body</span></span>
<span data-ttu-id="a542a-130">В тексте запроса добавьте представление объекта [акцессревиев](../resources/accessreview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a542a-130">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="a542a-131">В следующей таблице приведены свойства, принятые для создания Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="a542a-131">The following table shows the properties accepted to create an accessReview.</span></span>

| <span data-ttu-id="a542a-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="a542a-132">Property</span></span> | <span data-ttu-id="a542a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a542a-133">Type</span></span> | <span data-ttu-id="a542a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a542a-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a542a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a542a-135">displayName</span></span> | <span data-ttu-id="a542a-136">String</span><span class="sxs-lookup"><span data-stu-id="a542a-136">String</span></span> | <span data-ttu-id="a542a-137">Имя серии проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="a542a-137">Name of access review series.</span></span> <span data-ttu-id="a542a-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a542a-138">Required.</span></span>|
| <span data-ttu-id="a542a-139">дескриптионфорадминс</span><span class="sxs-lookup"><span data-stu-id="a542a-139">descriptionForAdmins</span></span> | <span data-ttu-id="a542a-140">string</span><span class="sxs-lookup"><span data-stu-id="a542a-140">string</span></span> | <span data-ttu-id="a542a-141">Контекст проверки, предоставленной администраторам.</span><span class="sxs-lookup"><span data-stu-id="a542a-141">Context of the review provided to admins.</span></span> <span data-ttu-id="a542a-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a542a-142">Required.</span></span> |
  <span data-ttu-id="a542a-143">дескриптионфорревиеверс</span><span class="sxs-lookup"><span data-stu-id="a542a-143">descriptionForReviewers</span></span> | <span data-ttu-id="a542a-144">string</span><span class="sxs-lookup"><span data-stu-id="a542a-144">string</span></span> | <span data-ttu-id="a542a-145">Контекст проверки, предоставленной для рецензентов.</span><span class="sxs-lookup"><span data-stu-id="a542a-145">Context of the review provided to reviewers.</span></span> <span data-ttu-id="a542a-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a542a-146">Required.</span></span> |
| <span data-ttu-id="a542a-147">scope</span><span class="sxs-lookup"><span data-stu-id="a542a-147">scope</span></span> | [<span data-ttu-id="a542a-148">акцессревиевскопе</span><span class="sxs-lookup"><span data-stu-id="a542a-148">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="a542a-149">Определяет область пользователей, проверенных в группе.</span><span class="sxs-lookup"><span data-stu-id="a542a-149">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="a542a-150">Обратитесь к разделу  [акцессревиевскопе](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a542a-150">See  [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="a542a-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a542a-151">Required.</span></span>| 
| <span data-ttu-id="a542a-152">инстанцеенумератионскопе</span><span class="sxs-lookup"><span data-stu-id="a542a-152">instanceEnumerationScope</span></span> | [<span data-ttu-id="a542a-153">акцессревиевскопе</span><span class="sxs-lookup"><span data-stu-id="a542a-153">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="a542a-154">В случае проверки всех групп это определяет область, в которой будут проверяться группы.</span><span class="sxs-lookup"><span data-stu-id="a542a-154">In the case of an all groups review, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="a542a-155">Обратитесь к разделу [акцессревиевскопе](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a542a-155">See [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> | 
| <span data-ttu-id="a542a-156">параметры</span><span class="sxs-lookup"><span data-stu-id="a542a-156">settings</span></span> | [<span data-ttu-id="a542a-157">акцессревиевсчедулесеттингс</span><span class="sxs-lookup"><span data-stu-id="a542a-157">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="a542a-158">Параметры ряда проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="a542a-158">The settings for an access review series.</span></span> <span data-ttu-id="a542a-159">Здесь определяется повторение.</span><span class="sxs-lookup"><span data-stu-id="a542a-159">Recurrence is determined here.</span></span> <span data-ttu-id="a542a-160">Обратитесь к разделу [акцессревиевсчедулесеттингс](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a542a-160">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="a542a-161">обсужден</span><span class="sxs-lookup"><span data-stu-id="a542a-161">reviewers</span></span> | <span data-ttu-id="a542a-162">Коллекция [акцессревиевревиеверскопе](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="a542a-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span> | <span data-ttu-id="a542a-163">Определяет, кто является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="a542a-163">Defines who the reviewers are.</span></span> <span data-ttu-id="a542a-164">Если ничего не указано, проверка является самостоятельным обзором (пользователи, Просмотрели проверку собственного доступа).</span><span class="sxs-lookup"><span data-stu-id="a542a-164">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="a542a-165">Обратитесь к разделу [акцессревиевревиеверскопе](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a542a-165">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |


## <a name="response"></a><span data-ttu-id="a542a-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="a542a-166">Response</span></span>
<span data-ttu-id="a542a-167">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a542a-167">If successful, this method returns a `201, Created` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a542a-168">Примеры</span><span class="sxs-lookup"><span data-stu-id="a542a-168">Examples</span></span>

<span data-ttu-id="a542a-169">Это пример создания серии проверки доступа с определенным пользователем, чей идентификатор объекта пользователя — 7eae4444-D425-48b2-adf2-3c777f6256f3, в качестве проверяющего.</span><span class="sxs-lookup"><span data-stu-id="a542a-169">This is an example of creating an access review series with a specific user, whose user object id is 7eae4444-d425-48b2-adf2-3c777f6256f3, as the reviewer.</span></span> <span data-ttu-id="a542a-170">В ходе проверки просматриваются все члены определенной группы, чей объект Group ID имеет значение b7a059cb-038a-4802-8fc9-b9d1ed0c4444.</span><span class="sxs-lookup"><span data-stu-id="a542a-170">The review reviews all members of a specific group, whose group object id is b7a059cb-038a-4802-8fc9-b9d1ed0c4444.</span></span> <span data-ttu-id="a542a-171">Он повторяется еженедельно.</span><span class="sxs-lookup"><span data-stu-id="a542a-171">It recurs weekly.</span></span>

### <a name="request"></a><span data-ttu-id="a542a-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="a542a-172">Request</span></span>
<span data-ttu-id="a542a-173">В тексте запроса добавьте представление объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a542a-173">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="a542a-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="a542a-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
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
# <a name="javascript"></a>[<span data-ttu-id="a542a-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a542a-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a542a-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="a542a-176">Response</span></span>
><span data-ttu-id="a542a-p113">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a542a-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
        "userPrincipalName": "admin@microsoft.com"
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
