---
title: 'Группа: Евалуатединамикмембершип'
description: Оцените, является ли пользователь или устройство участником динамической группы.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 41143a6b06352e0d28980d50058aeafc8da86a54
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333041"
---
# <a name="group-evaluatedynamicmembership"></a><span data-ttu-id="3d3a0-103">Группа: Евалуатединамикмембершип</span><span class="sxs-lookup"><span data-stu-id="3d3a0-103">group: evaluateDynamicMembership</span></span>

<span data-ttu-id="3d3a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d3a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d3a0-105">Оценка того, является ли пользователь или устройство участником динамической группы.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-105">Evaluate whether a user or device is or would be a member of a dynamic group.</span></span> <span data-ttu-id="3d3a0-106">Правило членства возвращается вместе с другими сведениями, использованными в ходе оценки.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-106">The membership rule is returned along with other details that were used in the evaluation.</span></span> <span data-ttu-id="3d3a0-107">Эту операцию можно выполнить следующими способами:</span><span class="sxs-lookup"><span data-stu-id="3d3a0-107">You can complete this operation in the following ways:</span></span> 

- <span data-ttu-id="3d3a0-108">Оценка того, является ли пользователь или устройство членом указанной динамической группы.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-108">Evaluate whether a user or device is a member of a specified dynamic group.</span></span>  
- <span data-ttu-id="3d3a0-109">Оценка того, будет ли пользователь или устройство участником динамической группы на основе идентификатора пользователя или устройства и правила членства.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-109">Evaluate whether a user or device would be a member of a dynamic group based on the ID of the user or device and a membership rule.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d3a0-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d3a0-110">Permissions</span></span>

<span data-ttu-id="3d3a0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d3a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a><span data-ttu-id="3d3a0-113">Оценка динамического членства с ИДЕНТИФИКАТОРом участника и ИДЕНТИФИКАТОРом группы</span><span class="sxs-lookup"><span data-stu-id="3d3a0-113">Evaluate dynamic membership with member ID and group ID</span></span>

| <span data-ttu-id="3d3a0-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d3a0-114">Permission type</span></span> | <span data-ttu-id="3d3a0-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d3a0-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="3d3a0-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d3a0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3d3a0-117">Для пользователя: Group. Read. ALL и User. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3d3a0-117">For user: Group.Read.All and User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="3d3a0-118">Для Device: Group. Read. ALL и Device. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3d3a0-118">For device: Group.Read.All and Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="3d3a0-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d3a0-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d3a0-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-120">Not supported.</span></span> |
| <span data-ttu-id="3d3a0-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d3a0-121">Application</span></span>                            | <span data-ttu-id="3d3a0-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-122">Not supported.</span></span> |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a><span data-ttu-id="3d3a0-123">Оценка динамического членства с ИДЕНТИФИКАТОРом участника и правилом членства</span><span class="sxs-lookup"><span data-stu-id="3d3a0-123">Evaluate dynamic membership with member ID and membership rule</span></span>

| <span data-ttu-id="3d3a0-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d3a0-124">Permission type</span></span> | <span data-ttu-id="3d3a0-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d3a0-125">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="3d3a0-126">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d3a0-126">Delegated (work or school account)</span></span> | <span data-ttu-id="3d3a0-127">Для пользователя: User. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3d3a0-127">For user: User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="3d3a0-128">Для Device: Device. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3d3a0-128">For device: Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="3d3a0-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d3a0-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d3a0-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-130">Not supported.</span></span> |
| <span data-ttu-id="3d3a0-131">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d3a0-131">Application</span></span>                            | <span data-ttu-id="3d3a0-132">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-132">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d3a0-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d3a0-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a><span data-ttu-id="3d3a0-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d3a0-134">Request headers</span></span>

| <span data-ttu-id="3d3a0-135">Имя</span><span class="sxs-lookup"><span data-stu-id="3d3a0-135">Name</span></span> | <span data-ttu-id="3d3a0-136">Описание</span><span class="sxs-lookup"><span data-stu-id="3d3a0-136">Description</span></span> |
| :--- | :---------- |
| <span data-ttu-id="3d3a0-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d3a0-137">Authorization</span></span> | <span data-ttu-id="3d3a0-138">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="3d3a0-138">Bearer {token}</span></span> |
| <span data-ttu-id="3d3a0-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d3a0-139">Content-type</span></span>  | <span data-ttu-id="3d3a0-140">application/json</span><span class="sxs-lookup"><span data-stu-id="3d3a0-140">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d3a0-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3d3a0-141">Request body</span></span>

<span data-ttu-id="3d3a0-142">В тексте запроса укажите необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-142">In the request body, supply the required properties.</span></span>

<span data-ttu-id="3d3a0-143">В следующей таблице перечислены свойства, которые необходимы при оценке членства в группе.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-143">The following table lists the properties that are required when you evaluate group membership.</span></span>

| <span data-ttu-id="3d3a0-144">Параметр</span><span class="sxs-lookup"><span data-stu-id="3d3a0-144">Parameter</span></span> | <span data-ttu-id="3d3a0-145">Тип</span><span class="sxs-lookup"><span data-stu-id="3d3a0-145">Type</span></span> | <span data-ttu-id="3d3a0-146">Описание</span><span class="sxs-lookup"><span data-stu-id="3d3a0-146">Description</span></span> |
| :-------- | :--- | :---------- |
| <span data-ttu-id="3d3a0-147">Идентификатора</span><span class="sxs-lookup"><span data-stu-id="3d3a0-147">memberId</span></span> | <span data-ttu-id="3d3a0-148">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="3d3a0-148">String collection</span></span> | <span data-ttu-id="3d3a0-149">memberId это идентификатор объекта для оцениваемого пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-149">memberId is the object Id of the user or device to be evaluated.</span></span> |
| <span data-ttu-id="3d3a0-150">membershipRule</span><span class="sxs-lookup"><span data-stu-id="3d3a0-150">membershipRule</span></span> | <span data-ttu-id="3d3a0-151">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="3d3a0-151">String collection</span></span> | <span data-ttu-id="3d3a0-152">Правило, используемое для оценки членства.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-152">The rule that is used for membership evaluation.</span></span> <span data-ttu-id="3d3a0-153">Если это свойство не указано, оценивается правило для существующей группы.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-153">If this property is not provided, the rule for the existing group is evaluated.</span></span> <span data-ttu-id="3d3a0-154">Если это свойство указано, то пользователь или устройство оцениваются для возможного членства в группе с тем же правилом.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-154">If this property is provided, the user or device is evaluated for possible membership in a group with the same rule.</span></span> <span data-ttu-id="3d3a0-155">Дополнительные сведения см. [в статье динамическое правило членства для групп в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span><span class="sxs-lookup"><span data-stu-id="3d3a0-155">For more information, see [Dynamic membership rules for groups in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span>|

## <a name="response"></a><span data-ttu-id="3d3a0-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d3a0-156">Response</span></span>

<span data-ttu-id="3d3a0-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [евалуатединамикмембершипресулт](../resources/evaluatedynamicmembershipresult.md) .</span><span class="sxs-lookup"><span data-stu-id="3d3a0-157">If successful, this method returns a `200 OK` response code and an [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="3d3a0-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="3d3a0-158">Examples</span></span>

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a><span data-ttu-id="3d3a0-159">Пример 1: Оценка того, является ли пользователь или устройство участником существующей группы</span><span class="sxs-lookup"><span data-stu-id="3d3a0-159">Example 1: Evaluate if a user or device is a member of an existing group</span></span>

#### <a name="request"></a><span data-ttu-id="3d3a0-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d3a0-160">Request</span></span>

<span data-ttu-id="3d3a0-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3d3a0-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d3a0-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33"
}
```
# <a name="c"></a>[<span data-ttu-id="3d3a0-163">C#</span><span class="sxs-lookup"><span data-stu-id="3d3a0-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d3a0-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d3a0-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d3a0-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d3a0-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3d3a0-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d3a0-166">Response</span></span>

<span data-ttu-id="3d3a0-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-167">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}

```

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a><span data-ttu-id="3d3a0-168">Пример 2: Оценка того, будет ли пользователь или устройство участником группы на основе правила членства</span><span class="sxs-lookup"><span data-stu-id="3d3a0-168">Example 2: Evaluate if a user or device would be a member of a group based on a membership rule</span></span>

#### <a name="request"></a><span data-ttu-id="3d3a0-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d3a0-169">Request</span></span>

<span data-ttu-id="3d3a0-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3d3a0-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d3a0-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership"
}-->

```http
POST https://graph.microsoft.com/beta/groups/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33",
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")"
}
```
# <a name="c"></a>[<span data-ttu-id="3d3a0-172">C#</span><span class="sxs-lookup"><span data-stu-id="3d3a0-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d3a0-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d3a0-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d3a0-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d3a0-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3d3a0-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d3a0-175">Response</span></span>

<span data-ttu-id="3d3a0-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3d3a0-176">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: evaluateDynamicMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
