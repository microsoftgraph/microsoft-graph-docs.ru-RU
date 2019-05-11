---
title: Обновление объекта deviceAndAppManagementRoleDefinition
description: Обновление свойств объекта deviceAndAppManagementRoleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 278dde3d8abb9b57a21f6672d2ebb2602683f68e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899559"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="c9f93-103">Обновление объекта deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c9f93-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="c9f93-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9f93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9f93-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9f93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9f93-106">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c9f93-106">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9f93-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c9f93-107">Prerequisites</span></span>
<span data-ttu-id="c9f93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9f93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9f93-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9f93-110">Permission type</span></span>|<span data-ttu-id="c9f93-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9f93-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9f93-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9f93-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9f93-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9f93-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c9f93-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9f93-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9f93-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9f93-115">Not supported.</span></span>|
|<span data-ttu-id="c9f93-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9f93-116">Application</span></span>|<span data-ttu-id="c9f93-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9f93-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9f93-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9f93-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="c9f93-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9f93-119">Request headers</span></span>
|<span data-ttu-id="c9f93-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9f93-120">Header</span></span>|<span data-ttu-id="c9f93-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c9f93-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9f93-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9f93-122">Authorization</span></span>|<span data-ttu-id="c9f93-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9f93-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9f93-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c9f93-124">Accept</span></span>|<span data-ttu-id="c9f93-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9f93-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9f93-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9f93-126">Request body</span></span>
<span data-ttu-id="c9f93-127">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9f93-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="c9f93-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c9f93-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="c9f93-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9f93-129">Property</span></span>|<span data-ttu-id="c9f93-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c9f93-130">Type</span></span>|<span data-ttu-id="c9f93-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c9f93-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9f93-132">id</span><span class="sxs-lookup"><span data-stu-id="c9f93-132">id</span></span>|<span data-ttu-id="c9f93-133">String</span><span class="sxs-lookup"><span data-stu-id="c9f93-133">String</span></span>|<span data-ttu-id="c9f93-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c9f93-134">Key of the entity.</span></span> <span data-ttu-id="c9f93-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="c9f93-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="c9f93-136">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c9f93-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c9f93-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c9f93-137">displayName</span></span>|<span data-ttu-id="c9f93-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c9f93-138">String</span></span>|<span data-ttu-id="c9f93-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="c9f93-139">Display Name of the Role definition.</span></span> <span data-ttu-id="c9f93-140">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c9f93-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c9f93-141">description</span><span class="sxs-lookup"><span data-stu-id="c9f93-141">description</span></span>|<span data-ttu-id="c9f93-142">String</span><span class="sxs-lookup"><span data-stu-id="c9f93-142">String</span></span>|<span data-ttu-id="c9f93-143">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="c9f93-143">Description of the Role definition.</span></span> <span data-ttu-id="c9f93-144">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c9f93-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c9f93-145">permissions</span><span class="sxs-lookup"><span data-stu-id="c9f93-145">permissions</span></span>|<span data-ttu-id="c9f93-146">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="c9f93-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c9f93-147">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="c9f93-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c9f93-148">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="c9f93-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="c9f93-149">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c9f93-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c9f93-150">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="c9f93-150">rolePermissions</span></span>|<span data-ttu-id="c9f93-151">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="c9f93-151">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c9f93-152">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="c9f93-152">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c9f93-153">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="c9f93-153">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="c9f93-154">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c9f93-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c9f93-155">Исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="c9f93-155">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="c9f93-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9f93-156">Boolean</span></span>|<span data-ttu-id="c9f93-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="c9f93-157">Type of Role.</span></span> <span data-ttu-id="c9f93-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="c9f93-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="c9f93-159">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c9f93-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c9f93-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="c9f93-160">isBuiltIn</span></span>|<span data-ttu-id="c9f93-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9f93-161">Boolean</span></span>|<span data-ttu-id="c9f93-162">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="c9f93-162">Type of Role.</span></span> <span data-ttu-id="c9f93-163">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="c9f93-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="c9f93-164">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c9f93-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c9f93-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9f93-165">roleScopeTagIds</span></span>|<span data-ttu-id="c9f93-166">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c9f93-166">String collection</span></span>|<span data-ttu-id="c9f93-167">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c9f93-167">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9f93-168">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c9f93-168">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c9f93-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9f93-169">Response</span></span>
<span data-ttu-id="c9f93-170">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9f93-170">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9f93-171">Пример</span><span class="sxs-lookup"><span data-stu-id="c9f93-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9f93-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9f93-172">Request</span></span>
<span data-ttu-id="c9f93-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9f93-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9f93-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9f93-174">Response</span></span>
<span data-ttu-id="c9f93-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9f93-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




