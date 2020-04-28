---
title: Создание unifiedRoleAssignmentMultiple
description: Создание нового объекта Унифиедролеассигнментмултипле.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 35f1063e36a5ada065ec7d5ac91e91e5d57db79a
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806370"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="cc33a-103">Создание unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="cc33a-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="cc33a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc33a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc33a-105">Создание нового объекта [унифиедролеассигнментмултипле](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="cc33a-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="cc33a-106">Используйте этот объект для создания назначений ролей в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="cc33a-106">Use this object to create role assignments in Microsoft Intune.</span></span> <span data-ttu-id="cc33a-107">Для других приложений Микрсофт 365 (например, Azure AD) используйте [унифиедролеассигнмент](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cc33a-107">For other Micrsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc33a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc33a-108">Permissions</span></span>

<span data-ttu-id="cc33a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc33a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc33a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc33a-111">Permission type</span></span> | <span data-ttu-id="cc33a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc33a-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="cc33a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc33a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cc33a-114">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="cc33a-114">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="cc33a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc33a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc33a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc33a-116">Not supported.</span></span> |
| <span data-ttu-id="cc33a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc33a-117">Application</span></span> | <span data-ttu-id="cc33a-118">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="cc33a-118">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc33a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc33a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="cc33a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc33a-120">Request headers</span></span>

| <span data-ttu-id="cc33a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cc33a-121">Name</span></span> | <span data-ttu-id="cc33a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cc33a-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="cc33a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc33a-123">Authorization</span></span> | <span data-ttu-id="cc33a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc33a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cc33a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc33a-126">Content-type</span></span> | <span data-ttu-id="cc33a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc33a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc33a-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc33a-129">Request body</span></span>

<span data-ttu-id="cc33a-130">В тексте запроса добавьте представление объекта [унифиедролеассигнментмултипле](../resources/unifiedroleassignmentmultiple.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc33a-130">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="cc33a-131">В запросе должна быть область, определенная в Azure AD, например `directoryScopeIds`, или область, зависящая от `appScopeId`приложения, например.</span><span class="sxs-lookup"><span data-stu-id="cc33a-131">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="cc33a-132">Примеры областей Azure AD: клиент ("/"), административные единицы или приложения.</span><span class="sxs-lookup"><span data-stu-id="cc33a-132">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="cc33a-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc33a-133">Response</span></span>

<span data-ttu-id="cc33a-134">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [унифиедролеассигнментмултипле](../resources/unifiedroleassignmentmultiple.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc33a-134">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc33a-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc33a-135">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="cc33a-136">Пример 1: Создание назначения роли в Intune для двух групп областей (которые являются объектами Azure AD)</span><span class="sxs-lookup"><span data-stu-id="cc33a-136">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="cc33a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc33a-137">Request</span></span>

<span data-ttu-id="cc33a-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc33a-138">The following is an example of the request.</span></span> <span data-ttu-id="cc33a-139">Обратите внимание на использование параметра **ролетемплатеид** для **роледефинитионид**.</span><span class="sxs-lookup"><span data-stu-id="cc33a-139">Note the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="cc33a-140">**роледефинитионид** может быть либо идентификатором шаблона на уровне службы, либо **роледефинитионид**, зависящим от каталога.</span><span class="sxs-lookup"><span data-stu-id="cc33a-140">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc33a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc33a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
}
```
# <a name="c"></a>[<span data-ttu-id="cc33a-142">C#</span><span class="sxs-lookup"><span data-stu-id="cc33a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc33a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc33a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc33a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc33a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cc33a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc33a-145">Response</span></span>

<span data-ttu-id="cc33a-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc33a-146">The following is an example of the response.</span></span>
> <span data-ttu-id="cc33a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc33a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"]
}
```

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="cc33a-149">Пример 2: Создание назначения роли в Intune в области, зависящей от Intune, для "All Devices".</span><span class="sxs-lookup"><span data-stu-id="cc33a-149">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="cc33a-150">Используйте следующие сведения для создания назначений ролей Intune:</span><span class="sxs-lookup"><span data-stu-id="cc33a-150">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="cc33a-151">Чтобы разрешить назначения на всех устройствах Intune, используйте `allDevices` значение в **аппскопеидс**.</span><span class="sxs-lookup"><span data-stu-id="cc33a-151">To allow assignments over all Intune devices, use the `allDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="cc33a-152">Чтобы разрешить назначения для всех пользователей, лицензированных в Intune `allLicensedUsers` , используйте значение в **аппскопеидс**.</span><span class="sxs-lookup"><span data-stu-id="cc33a-152">To allow assignments over all Intune licensed users, use the `allLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="cc33a-153">Чтобы разрешить назначения для всех устройств Intune и лицензированных пользователей, используйте `/` значение в **директорископеидс**.</span><span class="sxs-lookup"><span data-stu-id="cc33a-153">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="cc33a-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc33a-154">Request</span></span>

<span data-ttu-id="cc33a-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc33a-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc33a-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc33a-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_intune_specific"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```
# <a name="c"></a>[<span data-ttu-id="cc33a-157">C#</span><span class="sxs-lookup"><span data-stu-id="cc33a-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc33a-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc33a-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc33a-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc33a-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cc33a-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc33a-160">Response</span></span>

<span data-ttu-id="cc33a-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc33a-161">The following is an example of the response.</span></span>
> <span data-ttu-id="cc33a-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc33a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
