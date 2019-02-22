---
title: Создание deviceAndAppManagementRoleDefinition
description: Создание объекта deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9017d2cd02fa7ef9594efb62b168ce70fc4dd259
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139580"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="5a24c-103">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5a24c-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="5a24c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a24c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a24c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a24c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a24c-106">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5a24c-106">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a24c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a24c-107">Prerequisites</span></span>
<span data-ttu-id="5a24c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5a24c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5a24c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a24c-110">Permission type</span></span>|<span data-ttu-id="5a24c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a24c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a24c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a24c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a24c-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a24c-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5a24c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a24c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a24c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a24c-115">Not supported.</span></span>|
|<span data-ttu-id="5a24c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a24c-116">Application</span></span>|<span data-ttu-id="5a24c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a24c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a24c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a24c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="5a24c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a24c-119">Request headers</span></span>
|<span data-ttu-id="5a24c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a24c-120">Header</span></span>|<span data-ttu-id="5a24c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5a24c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a24c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a24c-122">Authorization</span></span>|<span data-ttu-id="5a24c-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5a24c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a24c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5a24c-124">Accept</span></span>|<span data-ttu-id="5a24c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a24c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a24c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5a24c-126">Request body</span></span>
<span data-ttu-id="5a24c-127">В теле запроса добавьте представление объекта deviceAndAppManagementRoleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a24c-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="5a24c-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="5a24c-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="5a24c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a24c-129">Property</span></span>|<span data-ttu-id="5a24c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5a24c-130">Type</span></span>|<span data-ttu-id="5a24c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5a24c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a24c-132">id</span><span class="sxs-lookup"><span data-stu-id="5a24c-132">id</span></span>|<span data-ttu-id="5a24c-133">String</span><span class="sxs-lookup"><span data-stu-id="5a24c-133">String</span></span>|<span data-ttu-id="5a24c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5a24c-134">Key of the entity.</span></span> <span data-ttu-id="5a24c-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="5a24c-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="5a24c-136">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5a24c-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5a24c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5a24c-137">displayName</span></span>|<span data-ttu-id="5a24c-138">String</span><span class="sxs-lookup"><span data-stu-id="5a24c-138">String</span></span>|<span data-ttu-id="5a24c-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="5a24c-139">Display Name of the Role definition.</span></span> <span data-ttu-id="5a24c-140">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5a24c-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5a24c-141">description</span><span class="sxs-lookup"><span data-stu-id="5a24c-141">description</span></span>|<span data-ttu-id="5a24c-142">String</span><span class="sxs-lookup"><span data-stu-id="5a24c-142">String</span></span>|<span data-ttu-id="5a24c-143">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="5a24c-143">Description of the Role definition.</span></span> <span data-ttu-id="5a24c-144">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5a24c-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5a24c-145">permissions</span><span class="sxs-lookup"><span data-stu-id="5a24c-145">permissions</span></span>|<span data-ttu-id="5a24c-146">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="5a24c-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="5a24c-147">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="5a24c-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="5a24c-148">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="5a24c-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="5a24c-149">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5a24c-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5a24c-150">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="5a24c-150">rolePermissions</span></span>|<span data-ttu-id="5a24c-151">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="5a24c-151">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="5a24c-152">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="5a24c-152">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="5a24c-153">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="5a24c-153">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="5a24c-154">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5a24c-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5a24c-155">Исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="5a24c-155">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="5a24c-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a24c-156">Boolean</span></span>|<span data-ttu-id="5a24c-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="5a24c-157">Type of Role.</span></span> <span data-ttu-id="5a24c-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="5a24c-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="5a24c-159">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5a24c-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5a24c-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="5a24c-160">isBuiltIn</span></span>|<span data-ttu-id="5a24c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a24c-161">Boolean</span></span>|<span data-ttu-id="5a24c-162">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="5a24c-162">Type of Role.</span></span> <span data-ttu-id="5a24c-163">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="5a24c-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="5a24c-164">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5a24c-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5a24c-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5a24c-165">roleScopeTagIds</span></span>|<span data-ttu-id="5a24c-166">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5a24c-166">String collection</span></span>|<span data-ttu-id="5a24c-167">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5a24c-167">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5a24c-168">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5a24c-168">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5a24c-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a24c-169">Response</span></span>
<span data-ttu-id="5a24c-170">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5a24c-170">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a24c-171">Пример</span><span class="sxs-lookup"><span data-stu-id="5a24c-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a24c-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a24c-172">Request</span></span>
<span data-ttu-id="5a24c-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a24c-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5a24c-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a24c-174">Response</span></span>
<span data-ttu-id="5a24c-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a24c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




