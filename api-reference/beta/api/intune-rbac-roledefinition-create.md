---
title: Создание roleDefinition
description: Создание объекта roleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f7d31dd9dab0219af303c5d03950fd572d8ebc1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141591"
---
# <a name="create-roledefinition"></a><span data-ttu-id="cefd9-103">Создание roleDefinition</span><span class="sxs-lookup"><span data-stu-id="cefd9-103">Create roleDefinition</span></span>

<span data-ttu-id="cefd9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cefd9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cefd9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cefd9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cefd9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cefd9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cefd9-107">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cefd9-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cefd9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cefd9-108">Prerequisites</span></span>
<span data-ttu-id="cefd9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cefd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cefd9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cefd9-111">Permission type</span></span>|<span data-ttu-id="cefd9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cefd9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cefd9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cefd9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cefd9-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cefd9-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="cefd9-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cefd9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cefd9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cefd9-116">Not supported.</span></span>|
|<span data-ttu-id="cefd9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cefd9-117">Application</span></span>|<span data-ttu-id="cefd9-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cefd9-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cefd9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cefd9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="cefd9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cefd9-120">Request headers</span></span>
|<span data-ttu-id="cefd9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cefd9-121">Header</span></span>|<span data-ttu-id="cefd9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cefd9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cefd9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cefd9-123">Authorization</span></span>|<span data-ttu-id="cefd9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cefd9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cefd9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cefd9-125">Accept</span></span>|<span data-ttu-id="cefd9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cefd9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cefd9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cefd9-127">Request body</span></span>
<span data-ttu-id="cefd9-128">В теле запроса добавьте представление объекта roleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cefd9-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="cefd9-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="cefd9-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="cefd9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cefd9-130">Property</span></span>|<span data-ttu-id="cefd9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cefd9-131">Type</span></span>|<span data-ttu-id="cefd9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cefd9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cefd9-133">id</span><span class="sxs-lookup"><span data-stu-id="cefd9-133">id</span></span>|<span data-ttu-id="cefd9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cefd9-134">String</span></span>|<span data-ttu-id="cefd9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cefd9-135">Key of the entity.</span></span> <span data-ttu-id="cefd9-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="cefd9-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="cefd9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cefd9-137">displayName</span></span>|<span data-ttu-id="cefd9-138">Строка</span><span class="sxs-lookup"><span data-stu-id="cefd9-138">String</span></span>|<span data-ttu-id="cefd9-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="cefd9-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="cefd9-140">description</span><span class="sxs-lookup"><span data-stu-id="cefd9-140">description</span></span>|<span data-ttu-id="cefd9-141">Строка</span><span class="sxs-lookup"><span data-stu-id="cefd9-141">String</span></span>|<span data-ttu-id="cefd9-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="cefd9-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="cefd9-143">permissions</span><span class="sxs-lookup"><span data-stu-id="cefd9-143">permissions</span></span>|<span data-ttu-id="cefd9-144">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="cefd9-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="cefd9-145">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="cefd9-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="cefd9-146">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="cefd9-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="cefd9-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="cefd9-147">rolePermissions</span></span>|<span data-ttu-id="cefd9-148">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="cefd9-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="cefd9-149">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="cefd9-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="cefd9-150">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="cefd9-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="cefd9-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cefd9-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="cefd9-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefd9-152">Boolean</span></span>|<span data-ttu-id="cefd9-153">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="cefd9-153">Type of Role.</span></span> <span data-ttu-id="cefd9-154">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="cefd9-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="cefd9-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="cefd9-155">isBuiltIn</span></span>|<span data-ttu-id="cefd9-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefd9-156">Boolean</span></span>|<span data-ttu-id="cefd9-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="cefd9-157">Type of Role.</span></span> <span data-ttu-id="cefd9-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="cefd9-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="cefd9-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cefd9-159">roleScopeTagIds</span></span>|<span data-ttu-id="cefd9-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cefd9-160">String collection</span></span>|<span data-ttu-id="cefd9-161">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="cefd9-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="cefd9-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="cefd9-162">Response</span></span>
<span data-ttu-id="cefd9-163">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cefd9-163">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cefd9-164">Пример</span><span class="sxs-lookup"><span data-stu-id="cefd9-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="cefd9-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="cefd9-165">Request</span></span>
<span data-ttu-id="cefd9-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cefd9-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cefd9-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="cefd9-167">Response</span></span>
<span data-ttu-id="cefd9-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cefd9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




