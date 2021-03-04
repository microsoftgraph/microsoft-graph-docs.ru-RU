---
title: Обновление accessReviewScheduleDefinition
description: Обнови существующий объект accessReviewScheduleDefinition, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6d03271d78dea64edf1c410a4bf30886c3e13603
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439018"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="66401-103">Обновление accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="66401-103">Update accessReviewScheduleDefinition</span></span>

<span data-ttu-id="66401-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66401-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66401-105">Обнови [существующий объект accessReviewScheduleDefinition,](../resources/accessreviewscheduledefinition.md) чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="66401-105">Update an existing [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object to change one or more of its properties.</span></span>

>[!NOTE]
><span data-ttu-id="66401-106">Любые обновления, сделанные в accessReviewScheduleDefinition, применяются только к будущим экземплярам.</span><span class="sxs-lookup"><span data-stu-id="66401-106">Any updates made to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="66401-107">В настоящее время запущенные экземпляры не могут быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="66401-107">Currently running instances cannot be updated.</span></span>
><span data-ttu-id="66401-108">Кроме того, этот API не предназначен для обновления свойств, включая решения, на уровне accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="66401-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="66401-109">Дополнительные сведения о экземплярах см. в [accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="66401-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="66401-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66401-110">Permissions</span></span>
<span data-ttu-id="66401-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66401-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66401-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66401-113">Permission type</span></span>                        | <span data-ttu-id="66401-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66401-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="66401-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66401-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="66401-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66401-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="66401-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66401-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66401-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66401-118">Not supported.</span></span>|
|<span data-ttu-id="66401-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="66401-119">Application</span></span>                            | <span data-ttu-id="66401-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66401-120">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66401-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66401-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="66401-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66401-122">Request headers</span></span>
| <span data-ttu-id="66401-123">Имя</span><span class="sxs-lookup"><span data-stu-id="66401-123">Name</span></span>         | <span data-ttu-id="66401-124">Описание</span><span class="sxs-lookup"><span data-stu-id="66401-124">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="66401-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66401-125">Authorization</span></span>|<span data-ttu-id="66401-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66401-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="66401-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66401-128">Content-type</span></span> | <span data-ttu-id="66401-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66401-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66401-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66401-131">Request body</span></span>
<span data-ttu-id="66401-132">В теле запроса поставляем представление JSON объекта [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="66401-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="66401-133">В следующей таблице показаны свойства, принятые для обновления accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="66401-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="66401-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="66401-134">Property</span></span> | <span data-ttu-id="66401-135">Тип</span><span class="sxs-lookup"><span data-stu-id="66401-135">Type</span></span> | <span data-ttu-id="66401-136">Описание</span><span class="sxs-lookup"><span data-stu-id="66401-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="66401-137">displayName</span><span class="sxs-lookup"><span data-stu-id="66401-137">displayName</span></span> | <span data-ttu-id="66401-138">String</span><span class="sxs-lookup"><span data-stu-id="66401-138">String</span></span> | <span data-ttu-id="66401-139">Имя серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="66401-139">Name of access review series.</span></span> |
| <span data-ttu-id="66401-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="66401-140">descriptionForAdmins</span></span> | <span data-ttu-id="66401-141">String</span><span class="sxs-lookup"><span data-stu-id="66401-141">String</span></span> | <span data-ttu-id="66401-142">Контекст обзора, предоставленного администраторам.</span><span class="sxs-lookup"><span data-stu-id="66401-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="66401-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="66401-143">descriptionForReviewers</span></span> | <span data-ttu-id="66401-144">String</span><span class="sxs-lookup"><span data-stu-id="66401-144">String</span></span> | <span data-ttu-id="66401-145">Контекст обзора, предоставленного рецензентам.</span><span class="sxs-lookup"><span data-stu-id="66401-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="66401-146">параметры</span><span class="sxs-lookup"><span data-stu-id="66401-146">settings</span></span> | [<span data-ttu-id="66401-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="66401-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="66401-148">Параметры для серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="66401-148">The settings for an access review series.</span></span> <span data-ttu-id="66401-149">См. [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="66401-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="66401-150">рецензенты</span><span class="sxs-lookup"><span data-stu-id="66401-150">reviewers</span></span> | <span data-ttu-id="66401-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="66401-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="66401-152">Определяет, кто такие рецензенты.</span><span class="sxs-lookup"><span data-stu-id="66401-152">Defines who the reviewers are.</span></span> <span data-ttu-id="66401-153">Если нет указаны, обзор является самообнаверяемой (пользователи рассмотрели обзор собственного доступа).</span><span class="sxs-lookup"><span data-stu-id="66401-153">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="66401-154">Свойство Reviewers является updatable только в том случае, если отдельные пользователи назначены в качестве рецензентов.</span><span class="sxs-lookup"><span data-stu-id="66401-154">The Reviewers property is only updatable if individual users assigned are as reviewers.</span></span> <span data-ttu-id="66401-155">См. [accessReviewReviewerScope.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="66401-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> | 

<span data-ttu-id="66401-156">Обратите внимание, что запрос PUT ожидает, что будет передан полный объект, в который включены все рукописные свойства, а не только обновляемые свойства.</span><span class="sxs-lookup"><span data-stu-id="66401-156">Note that a PUT request expects the full object to be passed in, in which all writable properties are included, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="66401-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="66401-157">Response</span></span>
<span data-ttu-id="66401-158">В случае успешной работы этот метод возвращает код `204, Accepted` ответа и не возвращает текст ответа.</span><span class="sxs-lookup"><span data-stu-id="66401-158">If successful, this method returns a `204, Accepted` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66401-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="66401-159">Examples</span></span>

<span data-ttu-id="66401-160">Это пример обновления displayName существующей серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="66401-160">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="66401-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="66401-161">Request</span></span>
<span data-ttu-id="66401-162">В теле запроса поставляют представление JSON о новых свойствах [объекта accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="66401-162">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="66401-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="66401-163">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="66401-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66401-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66401-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66401-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="66401-166">C#</span><span class="sxs-lookup"><span data-stu-id="66401-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66401-167">Java</span><span class="sxs-lookup"><span data-stu-id="66401-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="66401-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="66401-168">Response</span></span>
><span data-ttu-id="66401-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66401-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
