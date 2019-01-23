---
title: Обновление объекта roleDefinition
description: Обновление свойств объекта roleDefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b13f82e30e8bf67a78bd31db678de5b5a46051c3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412627"
---
# <a name="update-roledefinition"></a><span data-ttu-id="fd752-103">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="fd752-103">Update roleDefinition</span></span>

> <span data-ttu-id="fd752-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd752-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fd752-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd752-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd752-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd752-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd752-107">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fd752-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd752-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fd752-108">Prerequisites</span></span>
<span data-ttu-id="fd752-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd752-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fd752-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd752-111">Permission type</span></span>|<span data-ttu-id="fd752-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd752-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd752-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd752-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd752-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd752-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="fd752-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd752-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd752-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd752-116">Not supported.</span></span>|
|<span data-ttu-id="fd752-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd752-117">Application</span></span>|<span data-ttu-id="fd752-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd752-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd752-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd752-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="fd752-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd752-120">Request headers</span></span>
|<span data-ttu-id="fd752-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd752-121">Header</span></span>|<span data-ttu-id="fd752-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fd752-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd752-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd752-123">Authorization</span></span>|<span data-ttu-id="fd752-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fd752-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd752-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fd752-125">Accept</span></span>|<span data-ttu-id="fd752-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd752-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd752-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd752-127">Request body</span></span>
<span data-ttu-id="fd752-128">В теле запроса добавьте представление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd752-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="fd752-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fd752-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="fd752-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd752-130">Property</span></span>|<span data-ttu-id="fd752-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fd752-131">Type</span></span>|<span data-ttu-id="fd752-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fd752-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd752-133">id</span><span class="sxs-lookup"><span data-stu-id="fd752-133">id</span></span>|<span data-ttu-id="fd752-134">String</span><span class="sxs-lookup"><span data-stu-id="fd752-134">String</span></span>|<span data-ttu-id="fd752-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fd752-135">Key of the entity.</span></span> <span data-ttu-id="fd752-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="fd752-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="fd752-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fd752-137">displayName</span></span>|<span data-ttu-id="fd752-138">String</span><span class="sxs-lookup"><span data-stu-id="fd752-138">String</span></span>|<span data-ttu-id="fd752-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="fd752-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="fd752-140">description</span><span class="sxs-lookup"><span data-stu-id="fd752-140">description</span></span>|<span data-ttu-id="fd752-141">String</span><span class="sxs-lookup"><span data-stu-id="fd752-141">String</span></span>|<span data-ttu-id="fd752-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="fd752-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="fd752-143">permissions</span><span class="sxs-lookup"><span data-stu-id="fd752-143">permissions</span></span>|<span data-ttu-id="fd752-144">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="fd752-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="fd752-145">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="fd752-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="fd752-146">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="fd752-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="fd752-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="fd752-147">rolePermissions</span></span>|<span data-ttu-id="fd752-148">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="fd752-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="fd752-149">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="fd752-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="fd752-150">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="fd752-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="fd752-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="fd752-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="fd752-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd752-152">Boolean</span></span>|<span data-ttu-id="fd752-153">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="fd752-153">Type of Role.</span></span> <span data-ttu-id="fd752-154">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="fd752-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="fd752-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="fd752-155">isBuiltIn</span></span>|<span data-ttu-id="fd752-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd752-156">Boolean</span></span>|<span data-ttu-id="fd752-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="fd752-157">Type of Role.</span></span> <span data-ttu-id="fd752-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="fd752-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="fd752-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fd752-159">roleScopeTagIds</span></span>|<span data-ttu-id="fd752-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fd752-160">String collection</span></span>|<span data-ttu-id="fd752-161">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fd752-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="fd752-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd752-162">Response</span></span>
<span data-ttu-id="fd752-163">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fd752-163">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd752-164">Пример</span><span class="sxs-lookup"><span data-stu-id="fd752-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd752-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd752-165">Request</span></span>
<span data-ttu-id="fd752-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd752-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fd752-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd752-167">Response</span></span>
<span data-ttu-id="fd752-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fd752-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




