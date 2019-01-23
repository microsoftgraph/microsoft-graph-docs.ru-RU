---
title: Обновление объекта deviceAndAppManagementRoleDefinition
description: Обновление свойств объекта deviceAndAppManagementRoleDefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a881c0242a8414b071c03de85a733ad9296200b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394014"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="3289a-103">Обновление объекта deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3289a-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="3289a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3289a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3289a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3289a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3289a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3289a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3289a-107">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3289a-107">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3289a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3289a-108">Prerequisites</span></span>
<span data-ttu-id="3289a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3289a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3289a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3289a-111">Permission type</span></span>|<span data-ttu-id="3289a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3289a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3289a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3289a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3289a-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3289a-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3289a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3289a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3289a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3289a-116">Not supported.</span></span>|
|<span data-ttu-id="3289a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3289a-117">Application</span></span>|<span data-ttu-id="3289a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3289a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3289a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3289a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="3289a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3289a-120">Request headers</span></span>
|<span data-ttu-id="3289a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3289a-121">Header</span></span>|<span data-ttu-id="3289a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3289a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3289a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3289a-123">Authorization</span></span>|<span data-ttu-id="3289a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3289a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3289a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3289a-125">Accept</span></span>|<span data-ttu-id="3289a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3289a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3289a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3289a-127">Request body</span></span>
<span data-ttu-id="3289a-128">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3289a-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="3289a-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3289a-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="3289a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3289a-130">Property</span></span>|<span data-ttu-id="3289a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3289a-131">Type</span></span>|<span data-ttu-id="3289a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3289a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3289a-133">id</span><span class="sxs-lookup"><span data-stu-id="3289a-133">id</span></span>|<span data-ttu-id="3289a-134">String</span><span class="sxs-lookup"><span data-stu-id="3289a-134">String</span></span>|<span data-ttu-id="3289a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3289a-135">Key of the entity.</span></span> <span data-ttu-id="3289a-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="3289a-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="3289a-137">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3289a-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3289a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3289a-138">displayName</span></span>|<span data-ttu-id="3289a-139">String</span><span class="sxs-lookup"><span data-stu-id="3289a-139">String</span></span>|<span data-ttu-id="3289a-140">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="3289a-140">Display Name of the Role definition.</span></span> <span data-ttu-id="3289a-141">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3289a-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3289a-142">description</span><span class="sxs-lookup"><span data-stu-id="3289a-142">description</span></span>|<span data-ttu-id="3289a-143">String</span><span class="sxs-lookup"><span data-stu-id="3289a-143">String</span></span>|<span data-ttu-id="3289a-144">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="3289a-144">Description of the Role definition.</span></span> <span data-ttu-id="3289a-145">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3289a-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3289a-146">permissions</span><span class="sxs-lookup"><span data-stu-id="3289a-146">permissions</span></span>|<span data-ttu-id="3289a-147">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3289a-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3289a-148">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="3289a-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3289a-149">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3289a-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="3289a-150">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3289a-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3289a-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="3289a-151">rolePermissions</span></span>|<span data-ttu-id="3289a-152">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3289a-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3289a-153">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="3289a-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3289a-154">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3289a-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="3289a-155">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3289a-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3289a-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3289a-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="3289a-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="3289a-157">Boolean</span></span>|<span data-ttu-id="3289a-158">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="3289a-158">Type of Role.</span></span> <span data-ttu-id="3289a-159">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="3289a-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="3289a-160">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3289a-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3289a-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="3289a-161">isBuiltIn</span></span>|<span data-ttu-id="3289a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3289a-162">Boolean</span></span>|<span data-ttu-id="3289a-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="3289a-163">Type of Role.</span></span> <span data-ttu-id="3289a-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="3289a-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="3289a-165">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3289a-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="3289a-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3289a-166">roleScopeTagIds</span></span>|<span data-ttu-id="3289a-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3289a-167">String collection</span></span>|<span data-ttu-id="3289a-168">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3289a-168">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3289a-169">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3289a-169">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3289a-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="3289a-170">Response</span></span>
<span data-ttu-id="3289a-171">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3289a-171">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3289a-172">Пример</span><span class="sxs-lookup"><span data-stu-id="3289a-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="3289a-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="3289a-173">Request</span></span>
<span data-ttu-id="3289a-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3289a-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3289a-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="3289a-175">Response</span></span>
<span data-ttu-id="3289a-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3289a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




