---
title: Обновление объекта roleDefinition
description: Обновление свойств объекта roleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4e7746b5944798fd09d1565b7936c1fc5b7323cf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472357"
---
# <a name="update-roledefinition"></a><span data-ttu-id="a5f94-103">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a5f94-103">Update roleDefinition</span></span>

<span data-ttu-id="a5f94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5f94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5f94-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5f94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5f94-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5f94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5f94-107">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a5f94-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5f94-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a5f94-108">Prerequisites</span></span>
<span data-ttu-id="a5f94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5f94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5f94-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5f94-111">Permission type</span></span>|<span data-ttu-id="a5f94-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5f94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5f94-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5f94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5f94-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f94-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a5f94-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5f94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5f94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5f94-116">Not supported.</span></span>|
|<span data-ttu-id="a5f94-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5f94-117">Application</span></span>|<span data-ttu-id="a5f94-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f94-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5f94-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5f94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="a5f94-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a5f94-120">Request headers</span></span>
|<span data-ttu-id="a5f94-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5f94-121">Header</span></span>|<span data-ttu-id="a5f94-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a5f94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5f94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5f94-123">Authorization</span></span>|<span data-ttu-id="a5f94-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5f94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5f94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5f94-125">Accept</span></span>|<span data-ttu-id="a5f94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5f94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5f94-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5f94-127">Request body</span></span>
<span data-ttu-id="a5f94-128">В теле запроса добавьте представление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5f94-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="a5f94-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a5f94-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="a5f94-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5f94-130">Property</span></span>|<span data-ttu-id="a5f94-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a5f94-131">Type</span></span>|<span data-ttu-id="a5f94-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a5f94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5f94-133">id</span><span class="sxs-lookup"><span data-stu-id="a5f94-133">id</span></span>|<span data-ttu-id="a5f94-134">String</span><span class="sxs-lookup"><span data-stu-id="a5f94-134">String</span></span>|<span data-ttu-id="a5f94-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a5f94-135">Key of the entity.</span></span> <span data-ttu-id="a5f94-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="a5f94-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a5f94-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a5f94-137">displayName</span></span>|<span data-ttu-id="a5f94-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a5f94-138">String</span></span>|<span data-ttu-id="a5f94-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="a5f94-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="a5f94-140">description</span><span class="sxs-lookup"><span data-stu-id="a5f94-140">description</span></span>|<span data-ttu-id="a5f94-141">String</span><span class="sxs-lookup"><span data-stu-id="a5f94-141">String</span></span>|<span data-ttu-id="a5f94-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="a5f94-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="a5f94-143">permissions</span><span class="sxs-lookup"><span data-stu-id="a5f94-143">permissions</span></span>|<span data-ttu-id="a5f94-144">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="a5f94-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a5f94-145">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="a5f94-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a5f94-146">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="a5f94-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="a5f94-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="a5f94-147">rolePermissions</span></span>|<span data-ttu-id="a5f94-148">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="a5f94-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a5f94-149">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="a5f94-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a5f94-150">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="a5f94-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="a5f94-151">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="a5f94-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="a5f94-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5f94-152">Boolean</span></span>|<span data-ttu-id="a5f94-153">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="a5f94-153">Type of Role.</span></span> <span data-ttu-id="a5f94-154">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="a5f94-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="a5f94-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="a5f94-155">isBuiltIn</span></span>|<span data-ttu-id="a5f94-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5f94-156">Boolean</span></span>|<span data-ttu-id="a5f94-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="a5f94-157">Type of Role.</span></span> <span data-ttu-id="a5f94-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="a5f94-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="a5f94-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a5f94-159">roleScopeTagIds</span></span>|<span data-ttu-id="a5f94-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a5f94-160">String collection</span></span>|<span data-ttu-id="a5f94-161">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a5f94-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="a5f94-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5f94-162">Response</span></span>
<span data-ttu-id="a5f94-163">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a5f94-163">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5f94-164">Пример</span><span class="sxs-lookup"><span data-stu-id="a5f94-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5f94-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5f94-165">Request</span></span>
<span data-ttu-id="a5f94-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5f94-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1207

{
  "@odata.type": "#microsoft.graph.roleDefinition",
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

### <a name="response"></a><span data-ttu-id="a5f94-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5f94-167">Response</span></span>
<span data-ttu-id="a5f94-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5f94-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1256

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
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



