---
title: Обновление accessReviewScheduleDefinition
description: Обновление существующего объекта accessReviewScheduleDefinition, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 57d1be0916331e342c5d37a29daf2785afe3c644
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943597"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="8b589-103">Обновление accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="8b589-103">Update accessReviewScheduleDefinition</span></span>

<span data-ttu-id="8b589-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b589-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b589-105">Обновление существующего [объекта accessReviewScheduleDefinition,](../resources/accessreviewscheduledefinition.md) чтобы изменить одно или несколько его свойств.</span><span class="sxs-lookup"><span data-stu-id="8b589-105">Update an existing [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object to change one or more of its properties.</span></span>

>[!NOTE]
><span data-ttu-id="8b589-106">Любые обновления accessReviewScheduleDefinition применяются только к будущим экземплярам.</span><span class="sxs-lookup"><span data-stu-id="8b589-106">Any updates made to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="8b589-107">В настоящее время не удается обновить запущенные экземпляры.</span><span class="sxs-lookup"><span data-stu-id="8b589-107">Currently running instances cannot be updated.</span></span>
><span data-ttu-id="8b589-108">Кроме того, этот API не предназначен для обновления свойств, включая решения, на уровне accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="8b589-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="8b589-109">Дополнительные сведения об [экземплярах см. в accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="8b589-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b589-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b589-110">Permissions</span></span>
<span data-ttu-id="8b589-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b589-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b589-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b589-113">Permission type</span></span>                        | <span data-ttu-id="8b589-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b589-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b589-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b589-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b589-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b589-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="8b589-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b589-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b589-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b589-118">Not supported.</span></span>|
|<span data-ttu-id="8b589-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="8b589-119">Application</span></span>                            | <span data-ttu-id="8b589-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b589-120">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b589-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b589-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="8b589-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b589-122">Request headers</span></span>
| <span data-ttu-id="8b589-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8b589-123">Name</span></span>         | <span data-ttu-id="8b589-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8b589-124">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="8b589-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b589-125">Authorization</span></span>|<span data-ttu-id="8b589-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b589-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="8b589-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b589-128">Content-type</span></span> | <span data-ttu-id="8b589-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b589-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b589-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b589-131">Request body</span></span>
<span data-ttu-id="8b589-132">В теле запроса предопределение представления объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="8b589-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="8b589-133">В следующей таблице показаны свойства, принятые для обновления объекта accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8b589-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="8b589-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b589-134">Property</span></span> | <span data-ttu-id="8b589-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8b589-135">Type</span></span> | <span data-ttu-id="8b589-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8b589-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8b589-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8b589-137">displayName</span></span> | <span data-ttu-id="8b589-138">String</span><span class="sxs-lookup"><span data-stu-id="8b589-138">String</span></span> | <span data-ttu-id="8b589-139">Название серии отзывов о доступе.</span><span class="sxs-lookup"><span data-stu-id="8b589-139">Name of access review series.</span></span> |
| <span data-ttu-id="8b589-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="8b589-140">descriptionForAdmins</span></span> | <span data-ttu-id="8b589-141">String</span><span class="sxs-lookup"><span data-stu-id="8b589-141">String</span></span> | <span data-ttu-id="8b589-142">Контекст проверки, предоставленной администраторам.</span><span class="sxs-lookup"><span data-stu-id="8b589-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="8b589-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="8b589-143">descriptionForReviewers</span></span> | <span data-ttu-id="8b589-144">String</span><span class="sxs-lookup"><span data-stu-id="8b589-144">String</span></span> | <span data-ttu-id="8b589-145">Контекст отзыва, предоставленного рецензентам.</span><span class="sxs-lookup"><span data-stu-id="8b589-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="8b589-146">settings</span><span class="sxs-lookup"><span data-stu-id="8b589-146">settings</span></span> | [<span data-ttu-id="8b589-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="8b589-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="8b589-148">Параметры для серии отзывов о доступе.</span><span class="sxs-lookup"><span data-stu-id="8b589-148">The settings for an access review series.</span></span> <span data-ttu-id="8b589-149">См. [accessReviewScheduleSettings.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b589-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="8b589-150">рецензенты</span><span class="sxs-lookup"><span data-stu-id="8b589-150">reviewers</span></span> | <span data-ttu-id="8b589-151">[Коллекция accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="8b589-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="8b589-152">Определяет, кто такие рецензенты.</span><span class="sxs-lookup"><span data-stu-id="8b589-152">Defines who the reviewers are.</span></span> <span data-ttu-id="8b589-153">Если ни один из них не указан, отзыв будет самообнаправлением (пользователи просмотрели свой собственный доступ).</span><span class="sxs-lookup"><span data-stu-id="8b589-153">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="8b589-154">Свойство "Рецензенты" может быть только updatable, если отдельные пользователи назначены как рецензенты.</span><span class="sxs-lookup"><span data-stu-id="8b589-154">The Reviewers property is only updatable if individual users assigned are as reviewers.</span></span> <span data-ttu-id="8b589-155">См. [accessReviewReviewerScope.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8b589-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> | 

<span data-ttu-id="8b589-156">Обратите внимание, что запрос PUT предполагает, что будет передан весь объект, в который включаются все свойства, в которые можно вписать, а не только обновляемые свойства.</span><span class="sxs-lookup"><span data-stu-id="8b589-156">Note that a PUT request expects the full object to be passed in, in which all writable properties are included, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="8b589-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b589-157">Response</span></span>
<span data-ttu-id="8b589-158">В случае успеха этот метод возвращает код `204, Accepted` отклика без тела отклика.</span><span class="sxs-lookup"><span data-stu-id="8b589-158">If successful, this method returns a `204, Accepted` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b589-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b589-159">Examples</span></span>

<span data-ttu-id="8b589-160">Это пример обновления displayName существующего ряда отзывов о доступе.</span><span class="sxs-lookup"><span data-stu-id="8b589-160">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="8b589-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b589-161">Request</span></span>
<span data-ttu-id="8b589-162">В теле запроса предопределение представления новых свойств объекта [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="8b589-162">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="8b589-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b589-163">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="8b589-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b589-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b589-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b589-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8b589-166">C#</span><span class="sxs-lookup"><span data-stu-id="8b589-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b589-167">Java</span><span class="sxs-lookup"><span data-stu-id="8b589-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="8b589-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b589-168">Response</span></span>
><span data-ttu-id="8b589-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b589-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
