---
title: 'Группа: Евалуатединамикмембершип'
description: Оцените, является ли пользователь или устройство участником динамической группы.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b49f89da63b68f15329f7f700cc7699ff07e6208
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272856"
---
# <a name="group-evaluatedynamicmembership"></a><span data-ttu-id="19a6e-103">Группа: Евалуатединамикмембершип</span><span class="sxs-lookup"><span data-stu-id="19a6e-103">group: evaluateDynamicMembership</span></span>

<span data-ttu-id="19a6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19a6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19a6e-105">Оценка того, является ли пользователь или устройство участником динамической группы.</span><span class="sxs-lookup"><span data-stu-id="19a6e-105">Evaluate whether a user or device is or would be a member of a dynamic group.</span></span> <span data-ttu-id="19a6e-106">Правило членства возвращается вместе с другими сведениями, использованными в ходе оценки.</span><span class="sxs-lookup"><span data-stu-id="19a6e-106">The membership rule is returned along with other details that were used in the evaluation.</span></span> <span data-ttu-id="19a6e-107">Эту операцию можно выполнить следующими способами:</span><span class="sxs-lookup"><span data-stu-id="19a6e-107">You can complete this operation in the following ways:</span></span> 

- <span data-ttu-id="19a6e-108">Оценка того, является ли пользователь или устройство членом указанной динамической группы.</span><span class="sxs-lookup"><span data-stu-id="19a6e-108">Evaluate whether a user or device is a member of a specified dynamic group.</span></span>  
- <span data-ttu-id="19a6e-109">Оценка того, будет ли пользователь или устройство участником динамической группы на основе идентификатора пользователя или устройства и правила членства.</span><span class="sxs-lookup"><span data-stu-id="19a6e-109">Evaluate whether a user or device would be a member of a dynamic group based on the ID of the user or device and a membership rule.</span></span>

## <a name="permissions"></a><span data-ttu-id="19a6e-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19a6e-110">Permissions</span></span>

<span data-ttu-id="19a6e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19a6e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a><span data-ttu-id="19a6e-113">Оценка динамического членства с ИДЕНТИФИКАТОРом участника и ИДЕНТИФИКАТОРом группы</span><span class="sxs-lookup"><span data-stu-id="19a6e-113">Evaluate dynamic membership with member ID and group ID</span></span>

| <span data-ttu-id="19a6e-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19a6e-114">Permission type</span></span> | <span data-ttu-id="19a6e-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19a6e-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="19a6e-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19a6e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="19a6e-117">Для пользователя: Group. Read. ALL и User. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="19a6e-117">For user: Group.Read.All and User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="19a6e-118">Для Device: Group. Read. ALL и Device. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="19a6e-118">For device: Group.Read.All and Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="19a6e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19a6e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19a6e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19a6e-120">Not supported.</span></span> |
| <span data-ttu-id="19a6e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19a6e-121">Application</span></span>                            | <span data-ttu-id="19a6e-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19a6e-122">Not supported.</span></span> |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a><span data-ttu-id="19a6e-123">Оценка динамического членства с ИДЕНТИФИКАТОРом участника и правилом членства</span><span class="sxs-lookup"><span data-stu-id="19a6e-123">Evaluate dynamic membership with member ID and membership rule</span></span>

| <span data-ttu-id="19a6e-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19a6e-124">Permission type</span></span> | <span data-ttu-id="19a6e-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19a6e-125">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="19a6e-126">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19a6e-126">Delegated (work or school account)</span></span> | <span data-ttu-id="19a6e-127">Для пользователя: User. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="19a6e-127">For user: User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="19a6e-128">Для Device: Device. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="19a6e-128">For device: Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="19a6e-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19a6e-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19a6e-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19a6e-130">Not supported.</span></span> |
| <span data-ttu-id="19a6e-131">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19a6e-131">Application</span></span>                            | <span data-ttu-id="19a6e-132">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19a6e-132">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19a6e-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19a6e-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a><span data-ttu-id="19a6e-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19a6e-134">Request headers</span></span>

| <span data-ttu-id="19a6e-135">Имя</span><span class="sxs-lookup"><span data-stu-id="19a6e-135">Name</span></span> | <span data-ttu-id="19a6e-136">Описание</span><span class="sxs-lookup"><span data-stu-id="19a6e-136">Description</span></span> |
| :--- | :---------- |
| <span data-ttu-id="19a6e-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="19a6e-137">Authorization</span></span> | <span data-ttu-id="19a6e-138">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="19a6e-138">Bearer {token}</span></span> |
| <span data-ttu-id="19a6e-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19a6e-139">Content-type</span></span>  | <span data-ttu-id="19a6e-140">application/json</span><span class="sxs-lookup"><span data-stu-id="19a6e-140">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="19a6e-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19a6e-141">Request body</span></span>

<span data-ttu-id="19a6e-142">В тексте запроса укажите необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="19a6e-142">In the request body, supply the required properties.</span></span>

<span data-ttu-id="19a6e-143">В следующей таблице перечислены свойства, которые необходимы при оценке членства в группе.</span><span class="sxs-lookup"><span data-stu-id="19a6e-143">The following table lists the properties that are required when you evaluate group membership.</span></span>

| <span data-ttu-id="19a6e-144">Параметр</span><span class="sxs-lookup"><span data-stu-id="19a6e-144">Parameter</span></span> | <span data-ttu-id="19a6e-145">Тип</span><span class="sxs-lookup"><span data-stu-id="19a6e-145">Type</span></span> | <span data-ttu-id="19a6e-146">Описание</span><span class="sxs-lookup"><span data-stu-id="19a6e-146">Description</span></span> |
| :-------- | :--- | :---------- |
| <span data-ttu-id="19a6e-147">Идентификатора</span><span class="sxs-lookup"><span data-stu-id="19a6e-147">memberId</span></span> | <span data-ttu-id="19a6e-148">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="19a6e-148">String collection</span></span> | <span data-ttu-id="19a6e-149">memberId это идентификатор объекта для оцениваемого пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="19a6e-149">memberId is the object Id of the user or device to be evaluated.</span></span> |
| <span data-ttu-id="19a6e-150">membershipRule</span><span class="sxs-lookup"><span data-stu-id="19a6e-150">membershipRule</span></span> | <span data-ttu-id="19a6e-151">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="19a6e-151">String collection</span></span> | <span data-ttu-id="19a6e-152">Правило, используемое для оценки членства.</span><span class="sxs-lookup"><span data-stu-id="19a6e-152">The rule that is used for membership evaluation.</span></span> <span data-ttu-id="19a6e-153">Если это свойство не указано, оценивается правило для существующей группы.</span><span class="sxs-lookup"><span data-stu-id="19a6e-153">If this property is not provided, the rule for the existing group is evaluated.</span></span> <span data-ttu-id="19a6e-154">Если это свойство указано, то пользователь или устройство оцениваются для возможного членства в группе с тем же правилом.</span><span class="sxs-lookup"><span data-stu-id="19a6e-154">If this property is provided, the user or device is evaluated for possible membership in a group with the same rule.</span></span> <span data-ttu-id="19a6e-155">Дополнительные сведения см. [в статье динамическое правило членства для групп в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span><span class="sxs-lookup"><span data-stu-id="19a6e-155">For more information, see [Dynamic membership rules for groups in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span>|

## <a name="response"></a><span data-ttu-id="19a6e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="19a6e-156">Response</span></span>

<span data-ttu-id="19a6e-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [евалуатединамикмембершипресулт](../resources/evaluatedynamicmembershipresult.md) .</span><span class="sxs-lookup"><span data-stu-id="19a6e-157">If successful, this method returns a `200 OK` response code and an [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="19a6e-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="19a6e-158">Examples</span></span>

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a><span data-ttu-id="19a6e-159">Пример 1: Оценка того, является ли пользователь или устройство участником существующей группы</span><span class="sxs-lookup"><span data-stu-id="19a6e-159">Example 1: Evaluate if a user or device is a member of an existing group</span></span>

#### <a name="request"></a><span data-ttu-id="19a6e-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="19a6e-160">Request</span></span>

<span data-ttu-id="19a6e-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19a6e-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="19a6e-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="19a6e-162">HTTP</span></span>](#tab/http)
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

#### <a name="response"></a><span data-ttu-id="19a6e-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="19a6e-163">Response</span></span>

<span data-ttu-id="19a6e-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="19a6e-164">The following is an example of the response.</span></span> 

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

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a><span data-ttu-id="19a6e-165">Пример 2: Оценка того, будет ли пользователь или устройство участником группы на основе правила членства</span><span class="sxs-lookup"><span data-stu-id="19a6e-165">Example 2: Evaluate if a user or device would be a member of a group based on a membership rule</span></span>

#### <a name="request"></a><span data-ttu-id="19a6e-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="19a6e-166">Request</span></span>

<span data-ttu-id="19a6e-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19a6e-167">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="19a6e-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="19a6e-168">Response</span></span>

<span data-ttu-id="19a6e-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="19a6e-169">The following is an example of the response.</span></span> 

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
