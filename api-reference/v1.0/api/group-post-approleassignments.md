---
title: Предоставление appRoleAssignment группе
description: Предоставление назначения роли приложения группе.
localization_priority: Priority
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: e17f94e0b1d62015bfbff8d849c4d205a48cba2a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949930"
---
# <a name="grant-an-approleassignment-to-a-group"></a><span data-ttu-id="cacdc-103">Предоставление appRoleAssignment группе</span><span class="sxs-lookup"><span data-stu-id="cacdc-103">Grant an appRoleAssignment to a group</span></span>

<span data-ttu-id="cacdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cacdc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cacdc-105">Используйте этот API, чтобы назначить роль приложения группе.</span><span class="sxs-lookup"><span data-stu-id="cacdc-105">Use this API to assign an app role to a group.</span></span> <span data-ttu-id="cacdc-106">Роль будет считаться назначенной всем непосредственным участникам группы.</span><span class="sxs-lookup"><span data-stu-id="cacdc-106">All direct members of the group will be considered assigned.</span></span> <span data-ttu-id="cacdc-107">Чтобы предоставить назначение роли приложения группе, нужны три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="cacdc-107">To grant an app role assignment to a group, you need three identifiers:</span></span>

- <span data-ttu-id="cacdc-108">`principalId`: `id` группы, которой нужно назначить роль приложения.</span><span class="sxs-lookup"><span data-stu-id="cacdc-108">`principalId`: The `id` of the group to which you are assigning the app role.</span></span>
- <span data-ttu-id="cacdc-109">`resourceId`: `id` ресурса `servicePrincipal`, который определяет роль приложения.</span><span class="sxs-lookup"><span data-stu-id="cacdc-109">`resourceId`: The `id` of the resource `servicePrincipal` which has defined the app role.</span></span>
- <span data-ttu-id="cacdc-110">`appRoleId`: `id` объекта `appRole` (определенного в субъекте-службе ресурса) для назначения группе.</span><span class="sxs-lookup"><span data-stu-id="cacdc-110">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the group.</span></span>

<span data-ttu-id="cacdc-111">Чтобы [использовать группу для управления доступом к приложениям](/azure/active-directory/users-groups-roles/groups-saasapps), могут потребоваться дополнительные лицензии.</span><span class="sxs-lookup"><span data-stu-id="cacdc-111">Additional licenses might be required to [use a group to manage access to applications](/azure/active-directory/users-groups-roles/groups-saasapps).</span></span>

## <a name="permissions"></a><span data-ttu-id="cacdc-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cacdc-112">Permissions</span></span>

<span data-ttu-id="cacdc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cacdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cacdc-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cacdc-115">Permission type</span></span>      | <span data-ttu-id="cacdc-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cacdc-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cacdc-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cacdc-117">Delegated (work or school account)</span></span> | <span data-ttu-id="cacdc-118">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cacdc-118">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cacdc-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cacdc-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cacdc-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cacdc-120">Not supported.</span></span>    |
|<span data-ttu-id="cacdc-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cacdc-121">Application</span></span> | <span data-ttu-id="cacdc-122">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cacdc-122">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cacdc-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cacdc-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="cacdc-124">Рекомендуется создавать назначения ролей приложения, используя отношение `appRoleAssignedTo` _ресурса_ субъекта-службы вместо отношения `appRoleAssignments` назначенного пользователя, группы или субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="cacdc-124">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cacdc-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cacdc-125">Request headers</span></span>

| <span data-ttu-id="cacdc-126">Имя</span><span class="sxs-lookup"><span data-stu-id="cacdc-126">Name</span></span>       | <span data-ttu-id="cacdc-127">Описание</span><span class="sxs-lookup"><span data-stu-id="cacdc-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="cacdc-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cacdc-128">Authorization</span></span> | <span data-ttu-id="cacdc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cacdc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cacdc-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cacdc-131">Content-type</span></span> | <span data-ttu-id="cacdc-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cacdc-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cacdc-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cacdc-134">Request body</span></span>

<span data-ttu-id="cacdc-135">В тексте запроса укажите представление JSON для объекта [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cacdc-135">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cacdc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cacdc-136">Response</span></span>

<span data-ttu-id="cacdc-137">В случае успеха этот метод возвращает в тексте отклика код отклика `201 Created` и объект [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cacdc-137">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cacdc-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="cacdc-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cacdc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cacdc-139">Request</span></span>

<span data-ttu-id="cacdc-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cacdc-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cacdc-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cacdc-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments
Content-Type: application/json

{
  "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
  "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055",
  "appRoleId": "00000000-0000-0000-0000-000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="cacdc-142">C#</span><span class="sxs-lookup"><span data-stu-id="cacdc-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cacdc-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cacdc-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cacdc-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cacdc-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cacdc-145">Java</span><span class="sxs-lookup"><span data-stu-id="cacdc-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="cacdc-146">В этом примере `{id}` и `{principalId-value}` станут `id` назначенной группы.</span><span class="sxs-lookup"><span data-stu-id="cacdc-146">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned group.</span></span>

### <a name="response"></a><span data-ttu-id="cacdc-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="cacdc-147">Response</span></span>

<span data-ttu-id="cacdc-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cacdc-148">Here is an example of the response.</span></span> 

><span data-ttu-id="cacdc-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cacdc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('7679d9a4-2323-44cd-b5c2-673ec88d8b12')/appRoleAssignments/$entity",
  "id": "pNl5diMjzUS1wmc-yI2LEkGgWqFFrFdLhG2Ly2CysL4",
  "deletedDateTime": null,
  "appRoleId": "00000000-0000-0000-0000-000000000000",
  "createdDateTime": "2021-02-19T17:55:08.3369542Z",
  "principalDisplayName": "Young techmakers",
  "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
  "principalType": "Group",
  "resourceDisplayName": "Yammer",
  "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055"
}
```

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
