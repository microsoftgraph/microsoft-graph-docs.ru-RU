---
title: Предоставление appRoleAssignment группе
description: Предоставление назначения роли приложения группе.
localization_priority: Priority
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: 89fbcd89f637c98bed4355712fc9acb0d8fb4749
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041297"
---
# <a name="grant-an-approleassignment-to-a-group"></a><span data-ttu-id="e1a2e-103">Предоставление appRoleAssignment группе</span><span class="sxs-lookup"><span data-stu-id="e1a2e-103">Grant an appRoleAssignment to a group</span></span>

<span data-ttu-id="e1a2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1a2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1a2e-105">Используйте этот API, чтобы назначить роль приложения группе.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-105">Use this API to assign an app role to a group.</span></span> <span data-ttu-id="e1a2e-106">Роль будет считаться назначенной всем непосредственным участникам группы.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-106">All direct members of the group will be considered assigned.</span></span> <span data-ttu-id="e1a2e-107">Чтобы предоставить назначение роли приложения группе, нужны три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="e1a2e-107">To grant an app role assignment to a group, you need three identifiers:</span></span>

- <span data-ttu-id="e1a2e-108">`principalId`: `id` группы, которой нужно назначить роль приложения.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-108">`principalId`: The `id` of the group to which you are assigning the app role.</span></span>
- <span data-ttu-id="e1a2e-109">`resourceId`: `id` ресурса `servicePrincipal`, который определяет роль приложения.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-109">`resourceId`: The `id` of the resource `servicePrincipal` which has defined the app role.</span></span>
- <span data-ttu-id="e1a2e-110">`appRoleId`: `id` объекта `appRole` (определенного в субъекте-службе ресурса) для назначения группе.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-110">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the group.</span></span>

<span data-ttu-id="e1a2e-111">Чтобы [использовать группу для управления доступом к приложениям](/azure/active-directory/users-groups-roles/groups-saasapps), могут потребоваться дополнительные лицензии.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-111">Additional licenses might be required to [use a group to manage access to applications](/azure/active-directory/users-groups-roles/groups-saasapps).</span></span>

## <a name="permissions"></a><span data-ttu-id="e1a2e-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1a2e-112">Permissions</span></span>

<span data-ttu-id="e1a2e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1a2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1a2e-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1a2e-115">Permission type</span></span>      | <span data-ttu-id="e1a2e-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1a2e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1a2e-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1a2e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e1a2e-118">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1a2e-118">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e1a2e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1a2e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1a2e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-120">Not supported.</span></span>    |
|<span data-ttu-id="e1a2e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1a2e-121">Application</span></span> | <span data-ttu-id="e1a2e-122">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1a2e-122">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1a2e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1a2e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="e1a2e-124">Рекомендуется создавать назначения ролей приложения, используя отношение `appRoleAssignedTo` _ресурса_ субъекта-службы вместо отношения `appRoleAssignments` назначенного пользователя, группы или субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-124">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1a2e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1a2e-125">Request headers</span></span>

| <span data-ttu-id="e1a2e-126">Имя</span><span class="sxs-lookup"><span data-stu-id="e1a2e-126">Name</span></span>       | <span data-ttu-id="e1a2e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e1a2e-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e1a2e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1a2e-128">Authorization</span></span> | <span data-ttu-id="e1a2e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1a2e-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1a2e-131">Content-type</span></span> | <span data-ttu-id="e1a2e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1a2e-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1a2e-134">Request body</span></span>

<span data-ttu-id="e1a2e-135">В тексте запроса укажите представление JSON для объекта [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e1a2e-135">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e1a2e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1a2e-136">Response</span></span>

<span data-ttu-id="e1a2e-137">В случае успеха этот метод возвращает в тексте отклика код отклика `201 Created` и объект [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e1a2e-137">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1a2e-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="e1a2e-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1a2e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1a2e-139">Request</span></span>

<span data-ttu-id="e1a2e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e1a2e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1a2e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment_1"
}-->

```http
POST https://graph.microsoft.com/beta/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments
Content-Type: application/json

{
  "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
  "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055",
  "appRoleId": "00000000-0000-0000-0000-000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="e1a2e-142">C#</span><span class="sxs-lookup"><span data-stu-id="e1a2e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1a2e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1a2e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1a2e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1a2e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1a2e-145">Java</span><span class="sxs-lookup"><span data-stu-id="e1a2e-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e1a2e-146">В этом примере `{id}` и `{principalId-value}` станут `id` назначенной группы.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-146">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned group.</span></span>

### <a name="response"></a><span data-ttu-id="e1a2e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1a2e-147">Response</span></span>

<span data-ttu-id="e1a2e-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-148">Here is an example of the response.</span></span> 

><span data-ttu-id="e1a2e-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-149">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('7679d9a4-2323-44cd-b5c2-673ec88d8b12')/appRoleAssignments/$entity",
  "id": "pNl5diMjzUS1wmc-yI2LEkGgWqFFrFdLhG2Ly2CysL4",
  "deletedDateTime": null,
  "appRoleId": "00000000-0000-0000-0000-000000000000",
  "creationTimestamp": "2021-02-19T17:55:08.3369542Z",
  "principalDisplayName": "Young techmakers",
  "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
  "principalType": "Group",
  "resourceDisplayName": "Yammer",
  "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055"
}
```

<span data-ttu-id="e1a2e-150">В этом примере обратите внимание, что значение, используемое в качестве **ИД** пользователя в URL-адресе запроса (`cde330e5-2150-4c11-9c5b-14bfdc948c79`), совпадает со свойством **principalId** в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="e1a2e-150">In this example, note that the value used as the user **id** in the request URL (`cde330e5-2150-4c11-9c5b-14bfdc948c79`) is the same as the **principalId** property in the body.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
