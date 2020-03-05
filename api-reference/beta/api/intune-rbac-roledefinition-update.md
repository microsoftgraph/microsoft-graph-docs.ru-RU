---
title: Обновление объекта roleDefinition
description: Обновление свойств объекта roleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e05136a24bbac8d9b646ea3b213884ca77355782
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459641"
---
# <a name="update-roledefinition"></a><span data-ttu-id="f7c4f-103">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="f7c4f-103">Update roleDefinition</span></span>

<span data-ttu-id="f7c4f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f7c4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7c4f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7c4f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7c4f-107">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f7c4f-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7c4f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7c4f-108">Prerequisites</span></span>
<span data-ttu-id="f7c4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7c4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7c4f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7c4f-111">Permission type</span></span>|<span data-ttu-id="f7c4f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7c4f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7c4f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7c4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7c4f-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c4f-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f7c4f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7c4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7c4f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-116">Not supported.</span></span>|
|<span data-ttu-id="f7c4f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7c4f-117">Application</span></span>|<span data-ttu-id="f7c4f-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c4f-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7c4f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7c4f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="f7c4f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f7c4f-120">Request headers</span></span>
|<span data-ttu-id="f7c4f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7c4f-121">Header</span></span>|<span data-ttu-id="f7c4f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7c4f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7c4f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7c4f-123">Authorization</span></span>|<span data-ttu-id="f7c4f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7c4f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7c4f-125">Accept</span></span>|<span data-ttu-id="f7c4f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7c4f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7c4f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7c4f-127">Request body</span></span>
<span data-ttu-id="f7c4f-128">В теле запроса добавьте представление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="f7c4f-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f7c4f-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="f7c4f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7c4f-130">Property</span></span>|<span data-ttu-id="f7c4f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7c4f-131">Type</span></span>|<span data-ttu-id="f7c4f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7c4f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7c4f-133">id</span><span class="sxs-lookup"><span data-stu-id="f7c4f-133">id</span></span>|<span data-ttu-id="f7c4f-134">String</span><span class="sxs-lookup"><span data-stu-id="f7c4f-134">String</span></span>|<span data-ttu-id="f7c4f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-135">Key of the entity.</span></span> <span data-ttu-id="f7c4f-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="f7c4f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f7c4f-137">displayName</span></span>|<span data-ttu-id="f7c4f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f7c4f-138">String</span></span>|<span data-ttu-id="f7c4f-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="f7c4f-140">description</span><span class="sxs-lookup"><span data-stu-id="f7c4f-140">description</span></span>|<span data-ttu-id="f7c4f-141">String</span><span class="sxs-lookup"><span data-stu-id="f7c4f-141">String</span></span>|<span data-ttu-id="f7c4f-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="f7c4f-143">permissions</span><span class="sxs-lookup"><span data-stu-id="f7c4f-143">permissions</span></span>|<span data-ttu-id="f7c4f-144">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f7c4f-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="f7c4f-145">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="f7c4f-146">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="f7c4f-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="f7c4f-147">rolePermissions</span></span>|<span data-ttu-id="f7c4f-148">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f7c4f-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="f7c4f-149">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="f7c4f-150">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="f7c4f-151">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="f7c4f-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="f7c4f-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7c4f-152">Boolean</span></span>|<span data-ttu-id="f7c4f-153">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-153">Type of Role.</span></span> <span data-ttu-id="f7c4f-154">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="f7c4f-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="f7c4f-155">isBuiltIn</span></span>|<span data-ttu-id="f7c4f-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7c4f-156">Boolean</span></span>|<span data-ttu-id="f7c4f-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-157">Type of Role.</span></span> <span data-ttu-id="f7c4f-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="f7c4f-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f7c4f-159">roleScopeTagIds</span></span>|<span data-ttu-id="f7c4f-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f7c4f-160">String collection</span></span>|<span data-ttu-id="f7c4f-161">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="f7c4f-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7c4f-162">Response</span></span>
<span data-ttu-id="f7c4f-163">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-163">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7c4f-164">Пример</span><span class="sxs-lookup"><span data-stu-id="f7c4f-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7c4f-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7c4f-165">Request</span></span>
<span data-ttu-id="f7c4f-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7c4f-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7c4f-167">Response</span></span>
<span data-ttu-id="f7c4f-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7c4f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





