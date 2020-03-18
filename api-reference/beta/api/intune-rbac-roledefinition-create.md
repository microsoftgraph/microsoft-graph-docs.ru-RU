---
title: Создание roleDefinition
description: Создание объекта roleDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c833132bb1fcccb08b16a87d034f04d6119afcef
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801651"
---
# <a name="create-roledefinition"></a><span data-ttu-id="8b097-103">Создание roleDefinition</span><span class="sxs-lookup"><span data-stu-id="8b097-103">Create roleDefinition</span></span>

> <span data-ttu-id="8b097-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b097-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b097-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b097-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b097-106">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8b097-106">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b097-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8b097-107">Prerequisites</span></span>
<span data-ttu-id="8b097-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b097-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b097-110">Permission type</span></span>|<span data-ttu-id="8b097-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b097-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b097-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b097-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b097-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b097-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8b097-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b097-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b097-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b097-115">Not supported.</span></span>|
|<span data-ttu-id="8b097-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8b097-116">Application</span></span>|<span data-ttu-id="8b097-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b097-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b097-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b097-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="8b097-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8b097-119">Request headers</span></span>
|<span data-ttu-id="8b097-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b097-120">Header</span></span>|<span data-ttu-id="8b097-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8b097-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b097-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b097-122">Authorization</span></span>|<span data-ttu-id="8b097-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b097-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b097-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8b097-124">Accept</span></span>|<span data-ttu-id="8b097-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b097-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b097-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b097-126">Request body</span></span>
<span data-ttu-id="8b097-127">В теле запроса добавьте представление объекта roleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b097-127">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="8b097-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8b097-128">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="8b097-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b097-129">Property</span></span>|<span data-ttu-id="8b097-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8b097-130">Type</span></span>|<span data-ttu-id="8b097-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8b097-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b097-132">id</span><span class="sxs-lookup"><span data-stu-id="8b097-132">id</span></span>|<span data-ttu-id="8b097-133">String</span><span class="sxs-lookup"><span data-stu-id="8b097-133">String</span></span>|<span data-ttu-id="8b097-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8b097-134">Key of the entity.</span></span> <span data-ttu-id="8b097-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="8b097-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="8b097-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8b097-136">displayName</span></span>|<span data-ttu-id="8b097-137">Строка</span><span class="sxs-lookup"><span data-stu-id="8b097-137">String</span></span>|<span data-ttu-id="8b097-138">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="8b097-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="8b097-139">description</span><span class="sxs-lookup"><span data-stu-id="8b097-139">description</span></span>|<span data-ttu-id="8b097-140">String</span><span class="sxs-lookup"><span data-stu-id="8b097-140">String</span></span>|<span data-ttu-id="8b097-141">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="8b097-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="8b097-142">permissions</span><span class="sxs-lookup"><span data-stu-id="8b097-142">permissions</span></span>|<span data-ttu-id="8b097-143">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="8b097-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="8b097-144">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="8b097-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="8b097-145">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="8b097-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="8b097-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="8b097-146">rolePermissions</span></span>|<span data-ttu-id="8b097-147">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="8b097-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="8b097-148">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="8b097-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="8b097-149">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="8b097-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="8b097-150">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="8b097-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="8b097-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b097-151">Boolean</span></span>|<span data-ttu-id="8b097-152">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="8b097-152">Type of Role.</span></span> <span data-ttu-id="8b097-153">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="8b097-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="8b097-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="8b097-154">isBuiltIn</span></span>|<span data-ttu-id="8b097-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b097-155">Boolean</span></span>|<span data-ttu-id="8b097-156">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="8b097-156">Type of Role.</span></span> <span data-ttu-id="8b097-157">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="8b097-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="8b097-158">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8b097-158">roleScopeTagIds</span></span>|<span data-ttu-id="8b097-159">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8b097-159">String collection</span></span>|<span data-ttu-id="8b097-160">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8b097-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="8b097-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b097-161">Response</span></span>
<span data-ttu-id="8b097-162">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b097-162">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b097-163">Пример</span><span class="sxs-lookup"><span data-stu-id="8b097-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b097-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b097-164">Request</span></span>
<span data-ttu-id="8b097-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b097-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="8b097-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b097-166">Response</span></span>
<span data-ttu-id="8b097-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b097-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




