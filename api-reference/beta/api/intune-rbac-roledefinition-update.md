---
title: Обновление объекта roleDefinition
description: Обновление свойств объекта roleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 481e86b590cbc1ffddcddb0b2593d5b6fc08b335
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36351191"
---
# <a name="update-roledefinition"></a><span data-ttu-id="0e382-103">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="0e382-103">Update roleDefinition</span></span>

> <span data-ttu-id="0e382-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e382-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e382-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e382-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e382-106">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0e382-106">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e382-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0e382-107">Prerequisites</span></span>
<span data-ttu-id="0e382-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e382-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e382-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e382-110">Permission type</span></span>|<span data-ttu-id="0e382-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e382-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e382-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e382-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e382-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e382-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0e382-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e382-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e382-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e382-115">Not supported.</span></span>|
|<span data-ttu-id="0e382-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e382-116">Application</span></span>|<span data-ttu-id="0e382-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e382-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e382-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e382-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="0e382-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e382-119">Request headers</span></span>
|<span data-ttu-id="0e382-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e382-120">Header</span></span>|<span data-ttu-id="0e382-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0e382-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e382-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e382-122">Authorization</span></span>|<span data-ttu-id="0e382-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e382-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e382-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0e382-124">Accept</span></span>|<span data-ttu-id="0e382-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e382-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e382-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0e382-126">Request body</span></span>
<span data-ttu-id="0e382-127">В теле запроса добавьте представление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e382-127">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="0e382-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0e382-128">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="0e382-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e382-129">Property</span></span>|<span data-ttu-id="0e382-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0e382-130">Type</span></span>|<span data-ttu-id="0e382-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0e382-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e382-132">id</span><span class="sxs-lookup"><span data-stu-id="0e382-132">id</span></span>|<span data-ttu-id="0e382-133">String</span><span class="sxs-lookup"><span data-stu-id="0e382-133">String</span></span>|<span data-ttu-id="0e382-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0e382-134">Key of the entity.</span></span> <span data-ttu-id="0e382-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="0e382-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="0e382-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0e382-136">displayName</span></span>|<span data-ttu-id="0e382-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0e382-137">String</span></span>|<span data-ttu-id="0e382-138">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="0e382-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="0e382-139">description</span><span class="sxs-lookup"><span data-stu-id="0e382-139">description</span></span>|<span data-ttu-id="0e382-140">String</span><span class="sxs-lookup"><span data-stu-id="0e382-140">String</span></span>|<span data-ttu-id="0e382-141">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="0e382-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="0e382-142">permissions</span><span class="sxs-lookup"><span data-stu-id="0e382-142">permissions</span></span>|<span data-ttu-id="0e382-143">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="0e382-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="0e382-144">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="0e382-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="0e382-145">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="0e382-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="0e382-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="0e382-146">rolePermissions</span></span>|<span data-ttu-id="0e382-147">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="0e382-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="0e382-148">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="0e382-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="0e382-149">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="0e382-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="0e382-150">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="0e382-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="0e382-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e382-151">Boolean</span></span>|<span data-ttu-id="0e382-152">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="0e382-152">Type of Role.</span></span> <span data-ttu-id="0e382-153">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="0e382-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="0e382-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="0e382-154">isBuiltIn</span></span>|<span data-ttu-id="0e382-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e382-155">Boolean</span></span>|<span data-ttu-id="0e382-156">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="0e382-156">Type of Role.</span></span> <span data-ttu-id="0e382-157">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="0e382-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="0e382-158">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e382-158">roleScopeTagIds</span></span>|<span data-ttu-id="0e382-159">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0e382-159">String collection</span></span>|<span data-ttu-id="0e382-160">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0e382-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="0e382-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e382-161">Response</span></span>
<span data-ttu-id="0e382-162">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0e382-162">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e382-163">Пример</span><span class="sxs-lookup"><span data-stu-id="0e382-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e382-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e382-164">Request</span></span>
<span data-ttu-id="0e382-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e382-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e382-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e382-166">Response</span></span>
<span data-ttu-id="0e382-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e382-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






