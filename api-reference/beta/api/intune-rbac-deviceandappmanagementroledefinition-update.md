---
title: Обновление объекта deviceAndAppManagementRoleDefinition
description: Обновление свойств объекта deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4061ef29268343adbb623cf9c7fe018bdce60517
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43421298"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="38f34-103">Обновление объекта deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="38f34-103">Update deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="38f34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38f34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38f34-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38f34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38f34-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38f34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38f34-107">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="38f34-107">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38f34-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="38f34-108">Prerequisites</span></span>
<span data-ttu-id="38f34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38f34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38f34-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38f34-111">Permission type</span></span>|<span data-ttu-id="38f34-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38f34-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38f34-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38f34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38f34-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38f34-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="38f34-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38f34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38f34-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38f34-116">Not supported.</span></span>|
|<span data-ttu-id="38f34-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="38f34-117">Application</span></span>|<span data-ttu-id="38f34-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38f34-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38f34-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38f34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="38f34-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="38f34-120">Request headers</span></span>
|<span data-ttu-id="38f34-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38f34-121">Header</span></span>|<span data-ttu-id="38f34-122">Значение</span><span class="sxs-lookup"><span data-stu-id="38f34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38f34-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38f34-123">Authorization</span></span>|<span data-ttu-id="38f34-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38f34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38f34-125">Accept</span><span class="sxs-lookup"><span data-stu-id="38f34-125">Accept</span></span>|<span data-ttu-id="38f34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38f34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38f34-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38f34-127">Request body</span></span>
<span data-ttu-id="38f34-128">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38f34-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="38f34-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="38f34-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="38f34-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="38f34-130">Property</span></span>|<span data-ttu-id="38f34-131">Тип</span><span class="sxs-lookup"><span data-stu-id="38f34-131">Type</span></span>|<span data-ttu-id="38f34-132">Описание</span><span class="sxs-lookup"><span data-stu-id="38f34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38f34-133">id</span><span class="sxs-lookup"><span data-stu-id="38f34-133">id</span></span>|<span data-ttu-id="38f34-134">String</span><span class="sxs-lookup"><span data-stu-id="38f34-134">String</span></span>|<span data-ttu-id="38f34-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="38f34-135">Key of the entity.</span></span> <span data-ttu-id="38f34-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="38f34-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="38f34-137">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="38f34-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="38f34-138">displayName</span><span class="sxs-lookup"><span data-stu-id="38f34-138">displayName</span></span>|<span data-ttu-id="38f34-139">Строка</span><span class="sxs-lookup"><span data-stu-id="38f34-139">String</span></span>|<span data-ttu-id="38f34-140">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="38f34-140">Display Name of the Role definition.</span></span> <span data-ttu-id="38f34-141">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="38f34-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="38f34-142">description</span><span class="sxs-lookup"><span data-stu-id="38f34-142">description</span></span>|<span data-ttu-id="38f34-143">String</span><span class="sxs-lookup"><span data-stu-id="38f34-143">String</span></span>|<span data-ttu-id="38f34-144">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="38f34-144">Description of the Role definition.</span></span> <span data-ttu-id="38f34-145">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="38f34-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="38f34-146">permissions</span><span class="sxs-lookup"><span data-stu-id="38f34-146">permissions</span></span>|<span data-ttu-id="38f34-147">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="38f34-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="38f34-148">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="38f34-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="38f34-149">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="38f34-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="38f34-150">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="38f34-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="38f34-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="38f34-151">rolePermissions</span></span>|<span data-ttu-id="38f34-152">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="38f34-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="38f34-153">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="38f34-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="38f34-154">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="38f34-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="38f34-155">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="38f34-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="38f34-156">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="38f34-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="38f34-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="38f34-157">Boolean</span></span>|<span data-ttu-id="38f34-158">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="38f34-158">Type of Role.</span></span> <span data-ttu-id="38f34-159">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="38f34-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="38f34-160">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="38f34-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="38f34-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="38f34-161">isBuiltIn</span></span>|<span data-ttu-id="38f34-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="38f34-162">Boolean</span></span>|<span data-ttu-id="38f34-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="38f34-163">Type of Role.</span></span> <span data-ttu-id="38f34-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="38f34-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="38f34-165">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="38f34-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="38f34-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38f34-166">roleScopeTagIds</span></span>|<span data-ttu-id="38f34-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="38f34-167">String collection</span></span>|<span data-ttu-id="38f34-168">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="38f34-168">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="38f34-169">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="38f34-169">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="38f34-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="38f34-170">Response</span></span>
<span data-ttu-id="38f34-171">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="38f34-171">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38f34-172">Пример</span><span class="sxs-lookup"><span data-stu-id="38f34-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="38f34-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="38f34-173">Request</span></span>
<span data-ttu-id="38f34-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38f34-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38f34-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="38f34-175">Response</span></span>
<span data-ttu-id="38f34-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38f34-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



