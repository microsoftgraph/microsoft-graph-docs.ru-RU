---
title: Создание unifiedRoleAssignmentMultiple
description: Создайте новый объект unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cabca41e1935f4a17073e512ea5835d56c982643
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2021
ms.locfileid: "52710493"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="f4d5f-103">Создание unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="f4d5f-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="f4d5f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4d5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4d5f-105">Создайте [новый объект unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="f4d5f-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="f4d5f-106">Используйте этот объект для создания назначений ролей в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-106">Use this object to create role assignments in Microsoft Intune.</span></span> <span data-ttu-id="f4d5f-107">Для других Microsoft 365 приложений (например, Azure AD) используйте [унифицированную системуRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f4d5f-107">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f4d5f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4d5f-108">Permissions</span></span>

<span data-ttu-id="f4d5f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4d5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4d5f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4d5f-111">Permission type</span></span> | <span data-ttu-id="f4d5f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4d5f-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="f4d5f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4d5f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f4d5f-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d5f-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="f4d5f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4d5f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4d5f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-116">Not supported.</span></span> |
| <span data-ttu-id="f4d5f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4d5f-117">Application</span></span> | <span data-ttu-id="f4d5f-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d5f-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4d5f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4d5f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="f4d5f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4d5f-120">Request headers</span></span>

| <span data-ttu-id="f4d5f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f4d5f-121">Name</span></span> | <span data-ttu-id="f4d5f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f4d5f-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="f4d5f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4d5f-123">Authorization</span></span> | <span data-ttu-id="f4d5f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4d5f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4d5f-126">Content-type</span></span> | <span data-ttu-id="f4d5f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4d5f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4d5f-129">Request body</span></span>

<span data-ttu-id="f4d5f-130">В теле запроса поставляем представление JSON объекта [unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="f4d5f-130">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="f4d5f-131">Запрос должен иметь область, определенную в Azure AD, например область, определенную приложению, например `directoryScopeIds` `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="f4d5f-131">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="f4d5f-132">Примерами области Azure AD являются клиенты ("/"), административные единицы или приложения.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-132">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="f4d5f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d5f-133">Response</span></span>

<span data-ttu-id="f4d5f-134">В случае успешного выполнения этот метод возвращает код ответа и новый объект `201 Created` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-134">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4d5f-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="f4d5f-135">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="f4d5f-136">Пример 1. Создание назначения ролей в Intune над двумя группами областей (которые являются объектами Azure AD)</span><span class="sxs-lookup"><span data-stu-id="f4d5f-136">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="f4d5f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4d5f-137">Request</span></span>

<span data-ttu-id="f4d5f-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-138">The following is an example of the request.</span></span>
> <span data-ttu-id="f4d5f-139">**Примечание:** использование **ролиTemplateId** для **roleDefinitionId**.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-139">**Note:** the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="f4d5f-140">**RoleDefinitionId** может быть как ИД шаблона для всей службы, так и ролью, определенной для **каталогаDefinitionId.**</span><span class="sxs-lookup"><span data-stu-id="f4d5f-140">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="f4d5f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4d5f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
}
```
# <a name="c"></a>[<span data-ttu-id="f4d5f-142">C#</span><span class="sxs-lookup"><span data-stu-id="f4d5f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4d5f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4d5f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4d5f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4d5f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4d5f-145">Java</span><span class="sxs-lookup"><span data-stu-id="f4d5f-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f4d5f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d5f-146">Response</span></span>

<span data-ttu-id="f4d5f-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-147">The following is an example of the response.</span></span>
> <span data-ttu-id="f4d5f-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="f4d5f-149">Пример 2. Создание назначения ролей в Intune в области Intune для "всех устройств"</span><span class="sxs-lookup"><span data-stu-id="f4d5f-149">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="f4d5f-150">Используйте следующую информацию для создания назначений ролей Intune:</span><span class="sxs-lookup"><span data-stu-id="f4d5f-150">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="f4d5f-151">Чтобы разрешить назначения на всех устройствах Intune, используйте `AllDevices` значение **в appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="f4d5f-151">To allow assignments over all Intune devices, use the `AllDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="f4d5f-152">Чтобы разрешить назначения всем лицензированным пользователям Intune, используйте значение `AllLicensedUsers` **в appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="f4d5f-152">To allow assignments over all Intune licensed users, use the `AllLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="f4d5f-153">Чтобы разрешить назначения для всех устройств Intune и лицензированных пользователей, используйте значение `/` **в directoryScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="f4d5f-153">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="f4d5f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4d5f-154">Request</span></span>

<span data-ttu-id="f4d5f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f4d5f-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4d5f-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_intune_specific"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```
# <a name="c"></a>[<span data-ttu-id="f4d5f-157">C#</span><span class="sxs-lookup"><span data-stu-id="f4d5f-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4d5f-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4d5f-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4d5f-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4d5f-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4d5f-160">Java</span><span class="sxs-lookup"><span data-stu-id="f4d5f-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-intune-specific-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f4d5f-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d5f-161">Response</span></span>

<span data-ttu-id="f4d5f-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-162">The following is an example of the response.</span></span>
> <span data-ttu-id="f4d5f-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f4d5f-163">**Note:** The response object shown here might be shortened for readability.</span></span>

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


