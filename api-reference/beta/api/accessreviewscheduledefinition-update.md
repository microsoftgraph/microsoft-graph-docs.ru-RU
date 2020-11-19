---
title: Обновление Акцессревиевсчедуледефинитион
description: Обновление существующего объекта Акцессревиевсчедуледефинитион для изменения одного или нескольких его свойств.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 06b69bb9e6defcbadb4694d4042fa3bb690ee0f4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221788"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="15453-103">Обновление Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="15453-103">Update accessReviewScheduleDefinition</span></span>

<span data-ttu-id="15453-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15453-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15453-105">Обновление существующего объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) для изменения одного или нескольких его свойств.</span><span class="sxs-lookup"><span data-stu-id="15453-105">Update an existing [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object to change one or more of its properties.</span></span>

>[!NOTE]
><span data-ttu-id="15453-106">Любые изменения, внесенные в Акцессревиевсчедуледефинитион, применяются только к будущим экземплярам.</span><span class="sxs-lookup"><span data-stu-id="15453-106">Any updates made to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="15453-107">Не удается обновить экземпляры, запущенные в текущий момент.</span><span class="sxs-lookup"><span data-stu-id="15453-107">Currently running instances cannot be updated.</span></span>
><span data-ttu-id="15453-108">Кроме того, этот API не предназначен для обновления свойств, в том числе решений, на уровне Акцессревиевинстанце.</span><span class="sxs-lookup"><span data-stu-id="15453-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="15453-109">Дополнительные сведения о экземплярах можно найти в разделе [акцессревиевинстанце](../resources/accessreviewinstance.md) .</span><span class="sxs-lookup"><span data-stu-id="15453-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="15453-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15453-110">Permissions</span></span>
<span data-ttu-id="15453-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15453-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15453-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15453-113">Permission type</span></span>                        | <span data-ttu-id="15453-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15453-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="15453-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15453-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="15453-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15453-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="15453-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15453-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15453-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15453-118">Not supported.</span></span>|
|<span data-ttu-id="15453-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="15453-119">Application</span></span>                            | <span data-ttu-id="15453-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15453-120">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15453-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15453-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="15453-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15453-122">Request headers</span></span>
| <span data-ttu-id="15453-123">Имя</span><span class="sxs-lookup"><span data-stu-id="15453-123">Name</span></span>         | <span data-ttu-id="15453-124">Описание</span><span class="sxs-lookup"><span data-stu-id="15453-124">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="15453-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15453-125">Authorization</span></span>|<span data-ttu-id="15453-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15453-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="15453-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15453-128">Content-type</span></span> | <span data-ttu-id="15453-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15453-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15453-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15453-131">Request body</span></span>
<span data-ttu-id="15453-132">В тексте запроса добавьте представление объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15453-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="15453-133">В следующей таблице приведены свойства, принятые для обновления Акцессревиевсчедуледефинитион.</span><span class="sxs-lookup"><span data-stu-id="15453-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="15453-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="15453-134">Property</span></span> | <span data-ttu-id="15453-135">Тип</span><span class="sxs-lookup"><span data-stu-id="15453-135">Type</span></span> | <span data-ttu-id="15453-136">Описание</span><span class="sxs-lookup"><span data-stu-id="15453-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="15453-137">displayName</span><span class="sxs-lookup"><span data-stu-id="15453-137">displayName</span></span> | <span data-ttu-id="15453-138">String</span><span class="sxs-lookup"><span data-stu-id="15453-138">String</span></span> | <span data-ttu-id="15453-139">Имя серии проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="15453-139">Name of access review series.</span></span> |
| <span data-ttu-id="15453-140">дескриптионфорадминс</span><span class="sxs-lookup"><span data-stu-id="15453-140">descriptionForAdmins</span></span> | <span data-ttu-id="15453-141">String</span><span class="sxs-lookup"><span data-stu-id="15453-141">String</span></span> | <span data-ttu-id="15453-142">Контекст проверки, предоставленной администраторам.</span><span class="sxs-lookup"><span data-stu-id="15453-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="15453-143">дескриптионфорревиеверс</span><span class="sxs-lookup"><span data-stu-id="15453-143">descriptionForReviewers</span></span> | <span data-ttu-id="15453-144">String</span><span class="sxs-lookup"><span data-stu-id="15453-144">String</span></span> | <span data-ttu-id="15453-145">Контекст проверки, предоставленной для рецензентов.</span><span class="sxs-lookup"><span data-stu-id="15453-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="15453-146">параметры</span><span class="sxs-lookup"><span data-stu-id="15453-146">settings</span></span> | [<span data-ttu-id="15453-147">акцессревиевсчедулесеттингс</span><span class="sxs-lookup"><span data-stu-id="15453-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="15453-148">Параметры ряда проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="15453-148">The settings for an access review series.</span></span> <span data-ttu-id="15453-149">Обратитесь к разделу [акцессревиевсчедулесеттингс](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="15453-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="15453-150">обсужден</span><span class="sxs-lookup"><span data-stu-id="15453-150">reviewers</span></span> | <span data-ttu-id="15453-151">Коллекция [акцессревиевревиеверскопе](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="15453-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="15453-152">Определяет, кто является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="15453-152">Defines who the reviewers are.</span></span> <span data-ttu-id="15453-153">Если ничего не указано, проверка является самостоятельным обзором (пользователи, Просмотрели проверку собственного доступа).</span><span class="sxs-lookup"><span data-stu-id="15453-153">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="15453-154">Свойство рецензентов можно обновлять только в том случае, если назначены отдельные пользователи в качестве проверяющих.</span><span class="sxs-lookup"><span data-stu-id="15453-154">The Reviewers property is only updatable if individual users assigned are as reviewers.</span></span> <span data-ttu-id="15453-155">Обратитесь к разделу [акцессревиевревиеверскопе](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="15453-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> | 

<span data-ttu-id="15453-156">Обратите внимание, что запрос PUT ожидает, что передается весь объект, в который включаются все доступные для записи свойства, а не только обновляемые свойства.</span><span class="sxs-lookup"><span data-stu-id="15453-156">Note that a PUT request expects the full object to be passed in, in which all writable properties are included, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="15453-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="15453-157">Response</span></span>
<span data-ttu-id="15453-158">В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="15453-158">If successful, this method returns a `204, Accepted` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15453-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="15453-159">Examples</span></span>

<span data-ttu-id="15453-160">Ниже приведен пример обновления displayName существующего ряда проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="15453-160">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="15453-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="15453-161">Request</span></span>
<span data-ttu-id="15453-162">В теле запроса добавьте представление новых свойств объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15453-162">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="15453-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="15453-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewScheduleDefinition"
}-->
```http
PUT https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6

{
  "id": "60860cdd-fb4d-4054-91ba-f75e04444aa6",
  "displayName": "Test world UPDATED NAME!",
  "descriptionForAdmins": "Test world",
  "descriptionForReviewers": "Test world",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "instanceEnumerationScope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 3,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-15"
      }
    }
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="15453-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15453-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15453-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15453-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="15453-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="15453-166">Response</span></span>
><span data-ttu-id="15453-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15453-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
