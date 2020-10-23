---
title: Создание deviceAndAppManagementRoleDefinition
description: Создание объекта deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4baf3947795cf35236f5c52cb4b6c2c36b49262c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725977"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="3a65a-103">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3a65a-103">Create deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="3a65a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a65a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a65a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a65a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a65a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a65a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a65a-107">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3a65a-107">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a65a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a65a-108">Prerequisites</span></span>
<span data-ttu-id="3a65a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a65a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a65a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a65a-111">Permission type</span></span>|<span data-ttu-id="3a65a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a65a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a65a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a65a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a65a-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a65a-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3a65a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a65a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a65a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a65a-116">Not supported.</span></span>|
|<span data-ttu-id="3a65a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a65a-117">Application</span></span>|<span data-ttu-id="3a65a-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a65a-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a65a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a65a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="3a65a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a65a-120">Request headers</span></span>
|<span data-ttu-id="3a65a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a65a-121">Header</span></span>|<span data-ttu-id="3a65a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a65a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a65a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a65a-123">Authorization</span></span>|<span data-ttu-id="3a65a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a65a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a65a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a65a-125">Accept</span></span>|<span data-ttu-id="3a65a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a65a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a65a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a65a-127">Request body</span></span>
<span data-ttu-id="3a65a-128">В теле запроса добавьте представление объекта deviceAndAppManagementRoleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a65a-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="3a65a-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="3a65a-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="3a65a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a65a-130">Property</span></span>|<span data-ttu-id="3a65a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a65a-131">Type</span></span>|<span data-ttu-id="3a65a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a65a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a65a-133">id</span><span class="sxs-lookup"><span data-stu-id="3a65a-133">id</span></span>|<span data-ttu-id="3a65a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3a65a-134">String</span></span>|<span data-ttu-id="3a65a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3a65a-135">Key of the entity.</span></span> <span data-ttu-id="3a65a-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="3a65a-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="3a65a-137">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3a65a-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3a65a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3a65a-138">displayName</span></span>|<span data-ttu-id="3a65a-139">Строка</span><span class="sxs-lookup"><span data-stu-id="3a65a-139">String</span></span>|<span data-ttu-id="3a65a-140">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="3a65a-140">Display Name of the Role definition.</span></span> <span data-ttu-id="3a65a-141">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3a65a-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3a65a-142">description</span><span class="sxs-lookup"><span data-stu-id="3a65a-142">description</span></span>|<span data-ttu-id="3a65a-143">Строка</span><span class="sxs-lookup"><span data-stu-id="3a65a-143">String</span></span>|<span data-ttu-id="3a65a-144">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="3a65a-144">Description of the Role definition.</span></span> <span data-ttu-id="3a65a-145">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3a65a-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3a65a-146">permissions</span><span class="sxs-lookup"><span data-stu-id="3a65a-146">permissions</span></span>|<span data-ttu-id="3a65a-147">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3a65a-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3a65a-148">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="3a65a-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3a65a-149">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3a65a-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="3a65a-150">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3a65a-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3a65a-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="3a65a-151">rolePermissions</span></span>|<span data-ttu-id="3a65a-152">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3a65a-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3a65a-153">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="3a65a-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3a65a-154">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3a65a-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="3a65a-155">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3a65a-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3a65a-156">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="3a65a-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="3a65a-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a65a-157">Boolean</span></span>|<span data-ttu-id="3a65a-158">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="3a65a-158">Type of Role.</span></span> <span data-ttu-id="3a65a-159">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="3a65a-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="3a65a-160">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3a65a-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3a65a-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="3a65a-161">isBuiltIn</span></span>|<span data-ttu-id="3a65a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a65a-162">Boolean</span></span>|<span data-ttu-id="3a65a-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="3a65a-163">Type of Role.</span></span> <span data-ttu-id="3a65a-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="3a65a-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="3a65a-165">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3a65a-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3a65a-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a65a-166">roleScopeTagIds</span></span>|<span data-ttu-id="3a65a-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3a65a-167">String collection</span></span>|<span data-ttu-id="3a65a-168">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3a65a-168">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3a65a-169">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3a65a-169">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3a65a-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a65a-170">Response</span></span>
<span data-ttu-id="3a65a-171">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3a65a-171">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a65a-172">Пример</span><span class="sxs-lookup"><span data-stu-id="3a65a-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a65a-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a65a-173">Request</span></span>
<span data-ttu-id="3a65a-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a65a-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="3a65a-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a65a-175">Response</span></span>
<span data-ttu-id="3a65a-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a65a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





