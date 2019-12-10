---
title: Обновление объекта deviceAndAppManagementRoleDefinition
description: Обновление свойств объекта deviceAndAppManagementRoleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1302944df85c1ab791a6f95c8163d67b2029bef
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940681"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="dd017-103">Обновление объекта deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="dd017-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="dd017-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd017-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd017-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd017-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd017-106">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dd017-106">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd017-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dd017-107">Prerequisites</span></span>
<span data-ttu-id="dd017-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd017-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd017-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd017-110">Permission type</span></span>|<span data-ttu-id="dd017-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd017-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd017-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd017-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd017-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd017-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="dd017-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd017-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd017-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd017-115">Not supported.</span></span>|
|<span data-ttu-id="dd017-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd017-116">Application</span></span>|<span data-ttu-id="dd017-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd017-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd017-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd017-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="dd017-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dd017-119">Request headers</span></span>
|<span data-ttu-id="dd017-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd017-120">Header</span></span>|<span data-ttu-id="dd017-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dd017-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd017-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd017-122">Authorization</span></span>|<span data-ttu-id="dd017-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd017-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd017-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dd017-124">Accept</span></span>|<span data-ttu-id="dd017-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd017-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd017-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd017-126">Request body</span></span>
<span data-ttu-id="dd017-127">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd017-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="dd017-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dd017-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="dd017-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd017-129">Property</span></span>|<span data-ttu-id="dd017-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dd017-130">Type</span></span>|<span data-ttu-id="dd017-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dd017-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd017-132">id</span><span class="sxs-lookup"><span data-stu-id="dd017-132">id</span></span>|<span data-ttu-id="dd017-133">String</span><span class="sxs-lookup"><span data-stu-id="dd017-133">String</span></span>|<span data-ttu-id="dd017-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd017-134">Key of the entity.</span></span> <span data-ttu-id="dd017-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="dd017-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="dd017-136">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dd017-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="dd017-137">displayName</span><span class="sxs-lookup"><span data-stu-id="dd017-137">displayName</span></span>|<span data-ttu-id="dd017-138">Строка</span><span class="sxs-lookup"><span data-stu-id="dd017-138">String</span></span>|<span data-ttu-id="dd017-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="dd017-139">Display Name of the Role definition.</span></span> <span data-ttu-id="dd017-140">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dd017-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="dd017-141">description</span><span class="sxs-lookup"><span data-stu-id="dd017-141">description</span></span>|<span data-ttu-id="dd017-142">String</span><span class="sxs-lookup"><span data-stu-id="dd017-142">String</span></span>|<span data-ttu-id="dd017-143">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="dd017-143">Description of the Role definition.</span></span> <span data-ttu-id="dd017-144">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dd017-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="dd017-145">permissions</span><span class="sxs-lookup"><span data-stu-id="dd017-145">permissions</span></span>|<span data-ttu-id="dd017-146">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="dd017-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="dd017-147">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="dd017-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="dd017-148">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="dd017-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="dd017-149">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dd017-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="dd017-150">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="dd017-150">rolePermissions</span></span>|<span data-ttu-id="dd017-151">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="dd017-151">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="dd017-152">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="dd017-152">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="dd017-153">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="dd017-153">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="dd017-154">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dd017-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="dd017-155">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="dd017-155">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="dd017-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd017-156">Boolean</span></span>|<span data-ttu-id="dd017-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="dd017-157">Type of Role.</span></span> <span data-ttu-id="dd017-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="dd017-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="dd017-159">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dd017-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="dd017-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="dd017-160">isBuiltIn</span></span>|<span data-ttu-id="dd017-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd017-161">Boolean</span></span>|<span data-ttu-id="dd017-162">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="dd017-162">Type of Role.</span></span> <span data-ttu-id="dd017-163">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="dd017-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="dd017-164">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dd017-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="dd017-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dd017-165">roleScopeTagIds</span></span>|<span data-ttu-id="dd017-166">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dd017-166">String collection</span></span>|<span data-ttu-id="dd017-167">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="dd017-167">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dd017-168">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dd017-168">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="dd017-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd017-169">Response</span></span>
<span data-ttu-id="dd017-170">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dd017-170">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd017-171">Пример</span><span class="sxs-lookup"><span data-stu-id="dd017-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd017-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd017-172">Request</span></span>
<span data-ttu-id="dd017-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd017-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dd017-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd017-174">Response</span></span>
<span data-ttu-id="dd017-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd017-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





