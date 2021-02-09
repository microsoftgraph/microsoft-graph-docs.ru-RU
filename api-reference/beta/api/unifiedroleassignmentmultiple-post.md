---
title: Создание unifiedRoleAssignmentMultiple
description: Создание объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cf393fb8a47bc797993120fc7a23865b5647fae4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154707"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="f7cfc-103">Создание unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="f7cfc-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="f7cfc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7cfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7cfc-105">Создание объекта [unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="f7cfc-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="f7cfc-106">Используйте этот объект для создания назначений ролей в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-106">Use this object to create role assignments in Microsoft Intune.</span></span> <span data-ttu-id="f7cfc-107">Для других приложений Microsoft 365 (например, Azure AD) используйте [unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f7cfc-107">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7cfc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7cfc-108">Permissions</span></span>

<span data-ttu-id="f7cfc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7cfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7cfc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7cfc-111">Permission type</span></span> | <span data-ttu-id="f7cfc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7cfc-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="f7cfc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7cfc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f7cfc-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7cfc-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="f7cfc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7cfc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7cfc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-116">Not supported.</span></span> |
| <span data-ttu-id="f7cfc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7cfc-117">Application</span></span> | <span data-ttu-id="f7cfc-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7cfc-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7cfc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7cfc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="f7cfc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7cfc-120">Request headers</span></span>

| <span data-ttu-id="f7cfc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f7cfc-121">Name</span></span> | <span data-ttu-id="f7cfc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f7cfc-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="f7cfc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7cfc-123">Authorization</span></span> | <span data-ttu-id="f7cfc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7cfc-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7cfc-126">Content-type</span></span> | <span data-ttu-id="f7cfc-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7cfc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7cfc-129">Request body</span></span>

<span data-ttu-id="f7cfc-130">В теле запроса укатите представление объекта [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-130">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="f7cfc-131">Запрос должен иметь область, определенную в Azure AD, например, область `directoryScopeIds` приложения, `appScopeId` например.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-131">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="f7cfc-132">Примерами области Azure AD являются клиент ("/"), административные единицы или приложения.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-132">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="f7cfc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7cfc-133">Response</span></span>

<span data-ttu-id="f7cfc-134">В случае успешного выполнения этот метод возвращает код отклика и новый объект `201 Created` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-134">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7cfc-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="f7cfc-135">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="f7cfc-136">Пример 1. Создание назначения роли в Intune для двух групп областей (которые являются объектами Azure AD)</span><span class="sxs-lookup"><span data-stu-id="f7cfc-136">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="f7cfc-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7cfc-137">Request</span></span>

<span data-ttu-id="f7cfc-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-138">The following is an example of the request.</span></span>
> <span data-ttu-id="f7cfc-139">**Примечание.** Использование **roleTemplateId** для **roleDefinitionId.**</span><span class="sxs-lookup"><span data-stu-id="f7cfc-139">**Note:** the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="f7cfc-140">**roleDefinitionId** может быть либо ИД шаблона для всей службы, либо каталогом **roleDefinitionId.**</span><span class="sxs-lookup"><span data-stu-id="f7cfc-140">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="f7cfc-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7cfc-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f7cfc-142">C#</span><span class="sxs-lookup"><span data-stu-id="f7cfc-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7cfc-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7cfc-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7cfc-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7cfc-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7cfc-145">Java</span><span class="sxs-lookup"><span data-stu-id="f7cfc-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f7cfc-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7cfc-146">Response</span></span>

<span data-ttu-id="f7cfc-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-147">The following is an example of the response.</span></span>
> <span data-ttu-id="f7cfc-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="f7cfc-150">Пример 2. Создание назначения роли в Intune в определенной для Intune области "все устройства"</span><span class="sxs-lookup"><span data-stu-id="f7cfc-150">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="f7cfc-151">Используйте следующие сведения для создания назначений ролей Intune:</span><span class="sxs-lookup"><span data-stu-id="f7cfc-151">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="f7cfc-152">Чтобы разрешить назначения на всех устройствах Intune, используйте значение `AllDevices` **в appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="f7cfc-152">To allow assignments over all Intune devices, use the `AllDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="f7cfc-153">Чтобы разрешить назначения всем лицензированным пользователям Intune, используйте значение `AllLicensedUsers` **в appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="f7cfc-153">To allow assignments over all Intune licensed users, use the `AllLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="f7cfc-154">Чтобы разрешить назначения для всех устройств Intune и лицензированных пользователей, используйте значение `/` **в directoryScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="f7cfc-154">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="f7cfc-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7cfc-155">Request</span></span>

<span data-ttu-id="f7cfc-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f7cfc-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7cfc-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f7cfc-158">C#</span><span class="sxs-lookup"><span data-stu-id="f7cfc-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7cfc-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7cfc-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7cfc-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7cfc-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7cfc-161">Java</span><span class="sxs-lookup"><span data-stu-id="f7cfc-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-intune-specific-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f7cfc-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7cfc-162">Response</span></span>

<span data-ttu-id="f7cfc-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-163">The following is an example of the response.</span></span>
> <span data-ttu-id="f7cfc-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7cfc-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


