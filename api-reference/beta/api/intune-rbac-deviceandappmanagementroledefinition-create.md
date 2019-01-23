---
title: Создание deviceAndAppManagementRoleDefinition
description: Создание объекта deviceAndAppManagementRoleDefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 11616042fd3671ca09eeb8913a15959cc3093456
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411402"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="4fd58-103">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4fd58-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="4fd58-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4fd58-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4fd58-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fd58-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fd58-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fd58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fd58-107">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4fd58-107">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fd58-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4fd58-108">Prerequisites</span></span>
<span data-ttu-id="4fd58-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4fd58-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4fd58-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fd58-111">Permission type</span></span>|<span data-ttu-id="4fd58-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fd58-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fd58-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fd58-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fd58-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fd58-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4fd58-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fd58-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fd58-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fd58-116">Not supported.</span></span>|
|<span data-ttu-id="4fd58-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fd58-117">Application</span></span>|<span data-ttu-id="4fd58-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fd58-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fd58-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fd58-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="4fd58-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fd58-120">Request headers</span></span>
|<span data-ttu-id="4fd58-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4fd58-121">Header</span></span>|<span data-ttu-id="4fd58-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4fd58-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fd58-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fd58-123">Authorization</span></span>|<span data-ttu-id="4fd58-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4fd58-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fd58-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4fd58-125">Accept</span></span>|<span data-ttu-id="4fd58-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fd58-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fd58-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4fd58-127">Request body</span></span>
<span data-ttu-id="4fd58-128">В теле запроса добавьте представление объекта deviceAndAppManagementRoleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fd58-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="4fd58-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="4fd58-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="4fd58-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fd58-130">Property</span></span>|<span data-ttu-id="4fd58-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4fd58-131">Type</span></span>|<span data-ttu-id="4fd58-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4fd58-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fd58-133">id</span><span class="sxs-lookup"><span data-stu-id="4fd58-133">id</span></span>|<span data-ttu-id="4fd58-134">String</span><span class="sxs-lookup"><span data-stu-id="4fd58-134">String</span></span>|<span data-ttu-id="4fd58-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4fd58-135">Key of the entity.</span></span> <span data-ttu-id="4fd58-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="4fd58-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="4fd58-137">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4fd58-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="4fd58-138">displayName</span><span class="sxs-lookup"><span data-stu-id="4fd58-138">displayName</span></span>|<span data-ttu-id="4fd58-139">String</span><span class="sxs-lookup"><span data-stu-id="4fd58-139">String</span></span>|<span data-ttu-id="4fd58-140">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="4fd58-140">Display Name of the Role definition.</span></span> <span data-ttu-id="4fd58-141">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4fd58-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="4fd58-142">description</span><span class="sxs-lookup"><span data-stu-id="4fd58-142">description</span></span>|<span data-ttu-id="4fd58-143">String</span><span class="sxs-lookup"><span data-stu-id="4fd58-143">String</span></span>|<span data-ttu-id="4fd58-144">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="4fd58-144">Description of the Role definition.</span></span> <span data-ttu-id="4fd58-145">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4fd58-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="4fd58-146">permissions</span><span class="sxs-lookup"><span data-stu-id="4fd58-146">permissions</span></span>|<span data-ttu-id="4fd58-147">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="4fd58-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="4fd58-148">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="4fd58-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="4fd58-149">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="4fd58-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="4fd58-150">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4fd58-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="4fd58-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="4fd58-151">rolePermissions</span></span>|<span data-ttu-id="4fd58-152">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="4fd58-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="4fd58-153">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="4fd58-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="4fd58-154">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="4fd58-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="4fd58-155">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4fd58-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="4fd58-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4fd58-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="4fd58-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fd58-157">Boolean</span></span>|<span data-ttu-id="4fd58-158">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="4fd58-158">Type of Role.</span></span> <span data-ttu-id="4fd58-159">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="4fd58-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="4fd58-160">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4fd58-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="4fd58-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="4fd58-161">isBuiltIn</span></span>|<span data-ttu-id="4fd58-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fd58-162">Boolean</span></span>|<span data-ttu-id="4fd58-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="4fd58-163">Type of Role.</span></span> <span data-ttu-id="4fd58-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="4fd58-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="4fd58-165">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4fd58-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="4fd58-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4fd58-166">roleScopeTagIds</span></span>|<span data-ttu-id="4fd58-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4fd58-167">String collection</span></span>|<span data-ttu-id="4fd58-168">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4fd58-168">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4fd58-169">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4fd58-169">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4fd58-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fd58-170">Response</span></span>
<span data-ttu-id="4fd58-171">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4fd58-171">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fd58-172">Пример</span><span class="sxs-lookup"><span data-stu-id="4fd58-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fd58-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fd58-173">Request</span></span>
<span data-ttu-id="4fd58-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fd58-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4fd58-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fd58-175">Response</span></span>
<span data-ttu-id="4fd58-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4fd58-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




