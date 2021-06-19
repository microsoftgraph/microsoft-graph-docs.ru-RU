---
title: Обновление accessReviewScheduleDefinition
description: Обнови существующий объект accessReviewScheduleDefinition, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: be3b7603419d616ef9ea9e4da94fdb8942dc36f3
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030450"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="995c6-103">Обновление accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="995c6-103">Update accessReviewScheduleDefinition</span></span>

<span data-ttu-id="995c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="995c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="995c6-105">Обнови [существующий объект accessReviewScheduleDefinition,](../resources/accessreviewscheduledefinition.md) чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="995c6-105">Update an existing [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object to change one or more of its properties.</span></span>

>[!NOTE]
><span data-ttu-id="995c6-106">Любые обновления, сделанные в accessReviewScheduleDefinition, применяются только к будущим экземплярам.</span><span class="sxs-lookup"><span data-stu-id="995c6-106">Any updates made to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="995c6-107">В настоящее время запущенные экземпляры не могут быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="995c6-107">Currently running instances cannot be updated.</span></span>
><span data-ttu-id="995c6-108">Кроме того, этот API не предназначен для обновления свойств, включая решения, на уровне accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="995c6-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="995c6-109">Дополнительные сведения о экземплярах см. в [accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="995c6-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="995c6-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="995c6-110">Permissions</span></span>
<span data-ttu-id="995c6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="995c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="995c6-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="995c6-113">Permission type</span></span>                        | <span data-ttu-id="995c6-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="995c6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="995c6-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="995c6-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="995c6-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="995c6-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="995c6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="995c6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="995c6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="995c6-118">Not supported.</span></span>|
|<span data-ttu-id="995c6-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="995c6-119">Application</span></span>                            | <span data-ttu-id="995c6-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="995c6-120">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="995c6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="995c6-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="995c6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="995c6-122">Request headers</span></span>
| <span data-ttu-id="995c6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="995c6-123">Name</span></span>         | <span data-ttu-id="995c6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="995c6-124">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="995c6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="995c6-125">Authorization</span></span>|<span data-ttu-id="995c6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="995c6-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="995c6-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="995c6-128">Content-type</span></span> | <span data-ttu-id="995c6-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="995c6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="995c6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="995c6-131">Request body</span></span>
<span data-ttu-id="995c6-132">В теле запроса поставляем представление JSON объекта [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="995c6-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="995c6-133">В следующей таблице показаны свойства, принятые для обновления accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="995c6-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="995c6-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="995c6-134">Property</span></span> | <span data-ttu-id="995c6-135">Тип</span><span class="sxs-lookup"><span data-stu-id="995c6-135">Type</span></span> | <span data-ttu-id="995c6-136">Описание</span><span class="sxs-lookup"><span data-stu-id="995c6-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="995c6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="995c6-137">displayName</span></span> | <span data-ttu-id="995c6-138">String</span><span class="sxs-lookup"><span data-stu-id="995c6-138">String</span></span> | <span data-ttu-id="995c6-139">Имя серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="995c6-139">Name of access review series.</span></span> |
| <span data-ttu-id="995c6-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="995c6-140">descriptionForAdmins</span></span> | <span data-ttu-id="995c6-141">String</span><span class="sxs-lookup"><span data-stu-id="995c6-141">String</span></span> | <span data-ttu-id="995c6-142">Контекст обзора, предоставленного администраторам.</span><span class="sxs-lookup"><span data-stu-id="995c6-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="995c6-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="995c6-143">descriptionForReviewers</span></span> | <span data-ttu-id="995c6-144">String</span><span class="sxs-lookup"><span data-stu-id="995c6-144">String</span></span> | <span data-ttu-id="995c6-145">Контекст обзора, предоставленного рецензентам.</span><span class="sxs-lookup"><span data-stu-id="995c6-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="995c6-146">settings</span><span class="sxs-lookup"><span data-stu-id="995c6-146">settings</span></span> | [<span data-ttu-id="995c6-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="995c6-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="995c6-148">Параметры для серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="995c6-148">The settings for an access review series.</span></span> <span data-ttu-id="995c6-149">См. [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="995c6-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="995c6-150">рецензенты</span><span class="sxs-lookup"><span data-stu-id="995c6-150">reviewers</span></span> | <span data-ttu-id="995c6-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="995c6-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="995c6-152">Определяет, кто такие рецензенты.</span><span class="sxs-lookup"><span data-stu-id="995c6-152">Defines who the reviewers are.</span></span> <span data-ttu-id="995c6-153">Если нет указаны, обзор является самообнаверяемой (пользователи просматривают собственный доступ).</span><span class="sxs-lookup"><span data-stu-id="995c6-153">If none are specified, the review is a self-review (users review their own access).</span></span> <span data-ttu-id="995c6-154">Свойство **рецензентов** может быть updatable только в том случае, если отдельные пользователи назначены в качестве рецензентов.</span><span class="sxs-lookup"><span data-stu-id="995c6-154">The **reviewers** property is only updatable if individual users are assigned as reviewers.</span></span> <span data-ttu-id="995c6-155">См. [accessReviewReviewerScope.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="995c6-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |
|<span data-ttu-id="995c6-156">fallbackReviewers</span><span class="sxs-lookup"><span data-stu-id="995c6-156">fallbackReviewers</span></span>|<span data-ttu-id="995c6-157">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="995c6-157">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="995c6-158">Коллекция областей рецензентов, используемых для определения списка рецензентов откатов, которые уведомлены о необходимости принятия мер, если пользователи не найдены из указанного списка рецензентов.</span><span class="sxs-lookup"><span data-stu-id="995c6-158">A collection of reviewer scopes used to define the list of fallback reviewers who are notified to take action if no users are found from the list of reviewers specified.</span></span> <span data-ttu-id="995c6-159">Это может произойти, если либо владелец группы указан в качестве рецензента, но владелец группы не существует, либо менеджер указан в качестве рецензента, но диспетчер пользователя не существует.</span><span class="sxs-lookup"><span data-stu-id="995c6-159">This could occur when either the group owner is specified as the reviewer but the group owner does not exist, or manager is specified as reviewer but a user's manager does not exist.</span></span>|
| <span data-ttu-id="995c6-160">backupReviewers (обесценив)</span><span class="sxs-lookup"><span data-stu-id="995c6-160">backupReviewers (deprecated)</span></span>|<span data-ttu-id="995c6-161">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="995c6-161">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>| <span data-ttu-id="995c6-162">Это свойство было заменено **fallbackReviewers**.</span><span class="sxs-lookup"><span data-stu-id="995c6-162">This property has been replaced by **fallbackReviewers**.</span></span> <span data-ttu-id="995c6-163">Однако указание резервных **копийReviewers** или **fallbackReviewers** автоматически заполняет те же значения для другого свойства.</span><span class="sxs-lookup"><span data-stu-id="995c6-163">However, specifying either **backupReviewers** or **fallbackReviewers** automatically populates the same values to the other property.</span></span> |

<span data-ttu-id="995c6-164">Запрос **PUT** предполагает, что будет передан полный объект, который включает в себя все свойства, которые можно использовать, а не только обновляемые свойства.</span><span class="sxs-lookup"><span data-stu-id="995c6-164">A **PUT** request expects the full object to be passed in, which includes all writable properties, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="995c6-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="995c6-165">Response</span></span>
<span data-ttu-id="995c6-166">В случае успешной работы этот метод возвращает код `204 No Content` ответа и не возвращает текст ответа.</span><span class="sxs-lookup"><span data-stu-id="995c6-166">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="995c6-167">Примеры</span><span class="sxs-lookup"><span data-stu-id="995c6-167">Examples</span></span>

<span data-ttu-id="995c6-168">Это пример обновления displayName существующей серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="995c6-168">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="995c6-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="995c6-169">Request</span></span>
<span data-ttu-id="995c6-170">В теле запроса поставляют представление JSON о новых свойствах [объекта accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="995c6-170">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="995c6-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="995c6-171">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="995c6-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="995c6-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="995c6-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="995c6-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="995c6-174">C#</span><span class="sxs-lookup"><span data-stu-id="995c6-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="995c6-175">Java</span><span class="sxs-lookup"><span data-stu-id="995c6-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="995c6-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="995c6-176">Response</span></span>
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
