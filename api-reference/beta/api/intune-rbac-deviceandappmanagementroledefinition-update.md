---
title: Обновление объекта deviceAndAppManagementRoleDefinition
description: Обновление свойств объекта deviceAndAppManagementRoleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c45697610a3565d8447401df5d2bf00e94ac5fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459823"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="7ed5d-103">Обновление объекта deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7ed5d-103">Update deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="7ed5d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7ed5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ed5d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ed5d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ed5d-107">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ed5d-107">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ed5d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7ed5d-108">Prerequisites</span></span>
<span data-ttu-id="7ed5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ed5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ed5d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ed5d-111">Permission type</span></span>|<span data-ttu-id="7ed5d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ed5d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ed5d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ed5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ed5d-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed5d-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="7ed5d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ed5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ed5d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-116">Not supported.</span></span>|
|<span data-ttu-id="7ed5d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ed5d-117">Application</span></span>|<span data-ttu-id="7ed5d-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed5d-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ed5d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ed5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="7ed5d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7ed5d-120">Request headers</span></span>
|<span data-ttu-id="7ed5d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ed5d-121">Header</span></span>|<span data-ttu-id="7ed5d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7ed5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ed5d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ed5d-123">Authorization</span></span>|<span data-ttu-id="7ed5d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ed5d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7ed5d-125">Accept</span></span>|<span data-ttu-id="7ed5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ed5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ed5d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ed5d-127">Request body</span></span>
<span data-ttu-id="7ed5d-128">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="7ed5d-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ed5d-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="7ed5d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ed5d-130">Property</span></span>|<span data-ttu-id="7ed5d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7ed5d-131">Type</span></span>|<span data-ttu-id="7ed5d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7ed5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ed5d-133">id</span><span class="sxs-lookup"><span data-stu-id="7ed5d-133">id</span></span>|<span data-ttu-id="7ed5d-134">String</span><span class="sxs-lookup"><span data-stu-id="7ed5d-134">String</span></span>|<span data-ttu-id="7ed5d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-135">Key of the entity.</span></span> <span data-ttu-id="7ed5d-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="7ed5d-137">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ed5d-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7ed5d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7ed5d-138">displayName</span></span>|<span data-ttu-id="7ed5d-139">Строка</span><span class="sxs-lookup"><span data-stu-id="7ed5d-139">String</span></span>|<span data-ttu-id="7ed5d-140">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-140">Display Name of the Role definition.</span></span> <span data-ttu-id="7ed5d-141">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ed5d-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7ed5d-142">description</span><span class="sxs-lookup"><span data-stu-id="7ed5d-142">description</span></span>|<span data-ttu-id="7ed5d-143">String</span><span class="sxs-lookup"><span data-stu-id="7ed5d-143">String</span></span>|<span data-ttu-id="7ed5d-144">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-144">Description of the Role definition.</span></span> <span data-ttu-id="7ed5d-145">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ed5d-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7ed5d-146">permissions</span><span class="sxs-lookup"><span data-stu-id="7ed5d-146">permissions</span></span>|<span data-ttu-id="7ed5d-147">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="7ed5d-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="7ed5d-148">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7ed5d-149">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="7ed5d-150">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ed5d-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7ed5d-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="7ed5d-151">rolePermissions</span></span>|<span data-ttu-id="7ed5d-152">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="7ed5d-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="7ed5d-153">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="7ed5d-154">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="7ed5d-155">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ed5d-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7ed5d-156">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="7ed5d-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="7ed5d-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ed5d-157">Boolean</span></span>|<span data-ttu-id="7ed5d-158">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-158">Type of Role.</span></span> <span data-ttu-id="7ed5d-159">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="7ed5d-160">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ed5d-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7ed5d-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="7ed5d-161">isBuiltIn</span></span>|<span data-ttu-id="7ed5d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ed5d-162">Boolean</span></span>|<span data-ttu-id="7ed5d-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-163">Type of Role.</span></span> <span data-ttu-id="7ed5d-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="7ed5d-165">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ed5d-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="7ed5d-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7ed5d-166">roleScopeTagIds</span></span>|<span data-ttu-id="7ed5d-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7ed5d-167">String collection</span></span>|<span data-ttu-id="7ed5d-168">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-168">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7ed5d-169">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="7ed5d-169">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7ed5d-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ed5d-170">Response</span></span>
<span data-ttu-id="7ed5d-171">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-171">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ed5d-172">Пример</span><span class="sxs-lookup"><span data-stu-id="7ed5d-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ed5d-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ed5d-173">Request</span></span>
<span data-ttu-id="7ed5d-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1229

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="7ed5d-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ed5d-175">Response</span></span>
<span data-ttu-id="7ed5d-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ed5d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1278

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





