---
title: Обновление accessReviewScheduleDefinition
description: Обнови существующий объект accessReviewScheduleDefinition, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0fe437806ee9fdb71535c16dab8c7ff07f631f39
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579636"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="687fe-103">Обновление accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="687fe-103">Update accessReviewScheduleDefinition</span></span>

<span data-ttu-id="687fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="687fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="687fe-105">Обнови [существующий объект accessReviewScheduleDefinition,](../resources/accessreviewscheduledefinition.md) чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="687fe-105">Update an existing [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object to change one or more of its properties.</span></span>

>[!NOTE]
><span data-ttu-id="687fe-106">Любые обновления, сделанные в accessReviewScheduleDefinition, применяются только к будущим экземплярам.</span><span class="sxs-lookup"><span data-stu-id="687fe-106">Any updates made to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="687fe-107">В настоящее время запущенные экземпляры не могут быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="687fe-107">Currently running instances cannot be updated.</span></span>
><span data-ttu-id="687fe-108">Кроме того, этот API не предназначен для обновления свойств, включая решения, на уровне accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="687fe-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="687fe-109">Дополнительные сведения о экземплярах см. в [accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="687fe-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="687fe-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="687fe-110">Permissions</span></span>
<span data-ttu-id="687fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="687fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="687fe-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="687fe-113">Permission type</span></span>                        | <span data-ttu-id="687fe-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="687fe-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="687fe-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="687fe-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="687fe-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="687fe-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="687fe-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="687fe-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="687fe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="687fe-118">Not supported.</span></span>|
|<span data-ttu-id="687fe-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="687fe-119">Application</span></span>                            | <span data-ttu-id="687fe-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="687fe-120">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="687fe-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="687fe-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="687fe-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="687fe-122">Request headers</span></span>
| <span data-ttu-id="687fe-123">Имя</span><span class="sxs-lookup"><span data-stu-id="687fe-123">Name</span></span>         | <span data-ttu-id="687fe-124">Описание</span><span class="sxs-lookup"><span data-stu-id="687fe-124">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="687fe-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="687fe-125">Authorization</span></span>|<span data-ttu-id="687fe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="687fe-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="687fe-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="687fe-128">Content-type</span></span> | <span data-ttu-id="687fe-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="687fe-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="687fe-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="687fe-131">Request body</span></span>
<span data-ttu-id="687fe-132">В теле запроса поставляем представление JSON объекта [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="687fe-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="687fe-133">В следующей таблице показаны свойства, принятые для обновления accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="687fe-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="687fe-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="687fe-134">Property</span></span> | <span data-ttu-id="687fe-135">Тип</span><span class="sxs-lookup"><span data-stu-id="687fe-135">Type</span></span> | <span data-ttu-id="687fe-136">Описание</span><span class="sxs-lookup"><span data-stu-id="687fe-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="687fe-137">displayName</span><span class="sxs-lookup"><span data-stu-id="687fe-137">displayName</span></span> | <span data-ttu-id="687fe-138">Строка</span><span class="sxs-lookup"><span data-stu-id="687fe-138">String</span></span> | <span data-ttu-id="687fe-139">Имя серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="687fe-139">Name of access review series.</span></span> |
| <span data-ttu-id="687fe-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="687fe-140">descriptionForAdmins</span></span> | <span data-ttu-id="687fe-141">Строка</span><span class="sxs-lookup"><span data-stu-id="687fe-141">String</span></span> | <span data-ttu-id="687fe-142">Контекст обзора, предоставленного администраторам.</span><span class="sxs-lookup"><span data-stu-id="687fe-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="687fe-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="687fe-143">descriptionForReviewers</span></span> | <span data-ttu-id="687fe-144">Строка</span><span class="sxs-lookup"><span data-stu-id="687fe-144">String</span></span> | <span data-ttu-id="687fe-145">Контекст обзора, предоставленного рецензентам.</span><span class="sxs-lookup"><span data-stu-id="687fe-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="687fe-146">settings</span><span class="sxs-lookup"><span data-stu-id="687fe-146">settings</span></span> | [<span data-ttu-id="687fe-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="687fe-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="687fe-148">Параметры для серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="687fe-148">The settings for an access review series.</span></span> <span data-ttu-id="687fe-149">См. [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="687fe-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="687fe-150">рецензенты</span><span class="sxs-lookup"><span data-stu-id="687fe-150">reviewers</span></span> | <span data-ttu-id="687fe-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="687fe-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="687fe-152">Определяет, кто такие рецензенты.</span><span class="sxs-lookup"><span data-stu-id="687fe-152">Defines who the reviewers are.</span></span> <span data-ttu-id="687fe-153">Если нет указаны, обзор является самообнаверяемой (пользователи рассмотрели обзор собственного доступа).</span><span class="sxs-lookup"><span data-stu-id="687fe-153">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="687fe-154">Свойство Reviewers является updatable только в том случае, если отдельные пользователи назначены в качестве рецензентов.</span><span class="sxs-lookup"><span data-stu-id="687fe-154">The Reviewers property is only updatable if individual users assigned are as reviewers.</span></span> <span data-ttu-id="687fe-155">См. [accessReviewReviewerScope.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="687fe-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> | 

<span data-ttu-id="687fe-156">Запрос **PUT** предполагает, что будет передан полный объект, который включает в себя все свойства, которые можно использовать, а не только обновляемые свойства.</span><span class="sxs-lookup"><span data-stu-id="687fe-156">A **PUT** request expects the full object to be passed in, which includes all writable properties, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="687fe-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="687fe-157">Response</span></span>
<span data-ttu-id="687fe-158">В случае успешной работы этот метод возвращает код `204 No Content` ответа и не возвращает текст ответа.</span><span class="sxs-lookup"><span data-stu-id="687fe-158">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="687fe-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="687fe-159">Examples</span></span>

<span data-ttu-id="687fe-160">Это пример обновления displayName существующей серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="687fe-160">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="687fe-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="687fe-161">Request</span></span>
<span data-ttu-id="687fe-162">В теле запроса поставляют представление JSON о новых свойствах [объекта accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="687fe-162">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="687fe-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="687fe-163">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="687fe-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="687fe-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="687fe-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="687fe-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="687fe-166">C#</span><span class="sxs-lookup"><span data-stu-id="687fe-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="687fe-167">Java</span><span class="sxs-lookup"><span data-stu-id="687fe-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="687fe-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="687fe-168">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
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
