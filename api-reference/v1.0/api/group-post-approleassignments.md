---
title: Предоставление Аппролеассигнмент группе
description: Предоставьте группе назначение роли приложения.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a58bc51eb9e173854ef075d6dec9f81ff1c617a1
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334996"
---
# <a name="grant-an-approleassignment-to-a-group"></a><span data-ttu-id="8ba4c-103">Предоставление Аппролеассигнмент группе</span><span class="sxs-lookup"><span data-stu-id="8ba4c-103">Grant an appRoleAssignment to a group</span></span>

<span data-ttu-id="8ba4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ba4c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ba4c-105">Используйте этот API, чтобы назначить роль приложения группе.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-105">Use this API to assign an app role to a group.</span></span> <span data-ttu-id="8ba4c-106">Все непосредственные участники группы будут считаться назначенными.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-106">All direct members of the group will be considered assigned.</span></span> <span data-ttu-id="8ba4c-107">Чтобы назначить роль приложения группе, вам понадобятся три идентификатора:</span><span class="sxs-lookup"><span data-stu-id="8ba4c-107">To grant an app role assignment to a group, you need three identifiers:</span></span>

- <span data-ttu-id="8ba4c-108">`principalId`: `id` Группа, в которую назначается роль приложения.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-108">`principalId`: The `id` of the group to which you are assigning the app role.</span></span>
- <span data-ttu-id="8ba4c-109">`resourceId`: Ресурс, в `id` `servicePrincipal` котором определена роль приложения.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-109">`resourceId`: The `id` of the resource `servicePrincipal` which has defined the app role.</span></span>
- <span data-ttu-id="8ba4c-110">`appRoleId`: Значение параметра `id` `appRole` (определенного для субъекта-службы ресурсов), назначаемое группе.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-110">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the group.</span></span>

<span data-ttu-id="8ba4c-111">Чтобы [использовать группу для управления доступом к приложениям](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-saasapps), может потребоваться дополнительная лицензия.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-111">Additional licenses might be required to [use a group to manage access to applications](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-saasapps).</span></span>

## <a name="permissions"></a><span data-ttu-id="8ba4c-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ba4c-112">Permissions</span></span>

<span data-ttu-id="8ba4c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ba4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ba4c-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ba4c-115">Permission type</span></span>      | <span data-ttu-id="8ba4c-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ba4c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ba4c-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ba4c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8ba4c-118">Аппролеассигнмент. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="8ba4c-118">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8ba4c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ba4c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ba4c-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-120">Not supported.</span></span>    |
|<span data-ttu-id="8ba4c-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ba4c-121">Application</span></span> | <span data-ttu-id="8ba4c-122">Аппролеассигнмент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8ba4c-122">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ba4c-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ba4c-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="8ba4c-124">Рекомендуется создавать назначения ролей приложений с помощью `appRoleAssignedTo` отношения между субъектом службы _ресурсов_ , а не с `appRoleAssignments` назначенным пользователем, группой или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-124">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ba4c-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ba4c-125">Request headers</span></span>

| <span data-ttu-id="8ba4c-126">Имя</span><span class="sxs-lookup"><span data-stu-id="8ba4c-126">Name</span></span>       | <span data-ttu-id="8ba4c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="8ba4c-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="8ba4c-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ba4c-128">Authorization</span></span> | <span data-ttu-id="8ba4c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8ba4c-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ba4c-131">Content-type</span></span> | <span data-ttu-id="8ba4c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ba4c-134">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ba4c-134">Request body</span></span>

<span data-ttu-id="8ba4c-135">В тексте запроса добавьте представление объекта [аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-135">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8ba4c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ba4c-136">Response</span></span>

<span data-ttu-id="8ba4c-137">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-137">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ba4c-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="8ba4c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ba4c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ba4c-139">Request</span></span>

<span data-ttu-id="8ba4c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8ba4c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ba4c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="8ba4c-142">C#</span><span class="sxs-lookup"><span data-stu-id="8ba4c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ba4c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ba4c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ba4c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ba4c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ba4c-145">Java</span><span class="sxs-lookup"><span data-stu-id="8ba4c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="8ba4c-146">В этом примере `{id}` и то, и `{principalId-value}` другое — это `id` назначенная группа.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-146">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned group.</span></span>

### <a name="response"></a><span data-ttu-id="8ba4c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ba4c-147">Response</span></span>

<span data-ttu-id="8ba4c-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-148">Here is an example of the response.</span></span> 

><span data-ttu-id="8ba4c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ba4c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "id": "id-value",
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalType": "principalType-value",
  "principalId": "principalId-value",
  "principalDisplayName": "principalDisplayName-value",
  "resourceId": "resourceId-value",
  "resourceDisplayName": "resourceDisplayName-value"
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
