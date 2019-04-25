---
title: Обновление объекта deviceAndAppManagementRoleDefinition
description: Обновление свойств объекта deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2279a89aa47802b94f58f92851014d1e0b0eb312
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527597"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="f4271-103">Обновление объекта deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f4271-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="f4271-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4271-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4271-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4271-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4271-106">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f4271-106">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4271-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f4271-107">Prerequisites</span></span>
<span data-ttu-id="f4271-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4271-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4271-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4271-110">Permission type</span></span>|<span data-ttu-id="f4271-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4271-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4271-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4271-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4271-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4271-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f4271-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4271-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4271-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4271-115">Not supported.</span></span>|
|<span data-ttu-id="f4271-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4271-116">Application</span></span>|<span data-ttu-id="f4271-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4271-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4271-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4271-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="f4271-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4271-119">Request headers</span></span>
|<span data-ttu-id="f4271-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4271-120">Header</span></span>|<span data-ttu-id="f4271-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f4271-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4271-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4271-122">Authorization</span></span>|<span data-ttu-id="f4271-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4271-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4271-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f4271-124">Accept</span></span>|<span data-ttu-id="f4271-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4271-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4271-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4271-126">Request body</span></span>
<span data-ttu-id="f4271-127">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4271-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="f4271-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f4271-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="f4271-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4271-129">Property</span></span>|<span data-ttu-id="f4271-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f4271-130">Type</span></span>|<span data-ttu-id="f4271-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f4271-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4271-132">id</span><span class="sxs-lookup"><span data-stu-id="f4271-132">id</span></span>|<span data-ttu-id="f4271-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f4271-133">String</span></span>|<span data-ttu-id="f4271-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f4271-134">Key of the entity.</span></span> <span data-ttu-id="f4271-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="f4271-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="f4271-136">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f4271-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f4271-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f4271-137">displayName</span></span>|<span data-ttu-id="f4271-138">String</span><span class="sxs-lookup"><span data-stu-id="f4271-138">String</span></span>|<span data-ttu-id="f4271-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="f4271-139">Display Name of the Role definition.</span></span> <span data-ttu-id="f4271-140">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f4271-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f4271-141">description</span><span class="sxs-lookup"><span data-stu-id="f4271-141">description</span></span>|<span data-ttu-id="f4271-142">String</span><span class="sxs-lookup"><span data-stu-id="f4271-142">String</span></span>|<span data-ttu-id="f4271-143">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="f4271-143">Description of the Role definition.</span></span> <span data-ttu-id="f4271-144">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f4271-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f4271-145">permissions</span><span class="sxs-lookup"><span data-stu-id="f4271-145">permissions</span></span>|<span data-ttu-id="f4271-146">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f4271-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="f4271-147">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="f4271-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="f4271-148">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="f4271-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="f4271-149">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f4271-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f4271-150">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="f4271-150">rolePermissions</span></span>|<span data-ttu-id="f4271-151">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f4271-151">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="f4271-152">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="f4271-152">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="f4271-153">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="f4271-153">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="f4271-154">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f4271-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f4271-155">Исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="f4271-155">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="f4271-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4271-156">Boolean</span></span>|<span data-ttu-id="f4271-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="f4271-157">Type of Role.</span></span> <span data-ttu-id="f4271-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="f4271-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="f4271-159">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f4271-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f4271-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="f4271-160">isBuiltIn</span></span>|<span data-ttu-id="f4271-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4271-161">Boolean</span></span>|<span data-ttu-id="f4271-162">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="f4271-162">Type of Role.</span></span> <span data-ttu-id="f4271-163">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="f4271-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="f4271-164">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f4271-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f4271-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4271-165">roleScopeTagIds</span></span>|<span data-ttu-id="f4271-166">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f4271-166">String collection</span></span>|<span data-ttu-id="f4271-167">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f4271-167">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4271-168">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f4271-168">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f4271-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4271-169">Response</span></span>
<span data-ttu-id="f4271-170">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f4271-170">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4271-171">Пример</span><span class="sxs-lookup"><span data-stu-id="f4271-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4271-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4271-172">Request</span></span>
<span data-ttu-id="f4271-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4271-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4271-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4271-174">Response</span></span>
<span data-ttu-id="f4271-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4271-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





