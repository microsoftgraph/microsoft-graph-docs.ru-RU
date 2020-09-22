---
title: Обновление объекта deviceAndAppManagementRoleDefinition
description: Обновление свойств объекта deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae60e9c215d862fb039549fa9a3fe0df88782a4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978848"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="f311f-103">Обновление объекта deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f311f-103">Update deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="f311f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f311f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f311f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f311f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f311f-106">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f311f-106">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f311f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f311f-107">Prerequisites</span></span>
<span data-ttu-id="f311f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f311f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f311f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f311f-110">Permission type</span></span>|<span data-ttu-id="f311f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f311f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f311f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f311f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f311f-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f311f-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f311f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f311f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f311f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f311f-115">Not supported.</span></span>|
|<span data-ttu-id="f311f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f311f-116">Application</span></span>|<span data-ttu-id="f311f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f311f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f311f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f311f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="f311f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f311f-119">Request headers</span></span>
|<span data-ttu-id="f311f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f311f-120">Header</span></span>|<span data-ttu-id="f311f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f311f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f311f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f311f-122">Authorization</span></span>|<span data-ttu-id="f311f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f311f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f311f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f311f-124">Accept</span></span>|<span data-ttu-id="f311f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f311f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f311f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f311f-126">Request body</span></span>
<span data-ttu-id="f311f-127">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f311f-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="f311f-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f311f-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="f311f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f311f-129">Property</span></span>|<span data-ttu-id="f311f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f311f-130">Type</span></span>|<span data-ttu-id="f311f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f311f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f311f-132">id</span><span class="sxs-lookup"><span data-stu-id="f311f-132">id</span></span>|<span data-ttu-id="f311f-133">String</span><span class="sxs-lookup"><span data-stu-id="f311f-133">String</span></span>|<span data-ttu-id="f311f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f311f-134">Key of the entity.</span></span> <span data-ttu-id="f311f-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="f311f-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="f311f-136">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f311f-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f311f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f311f-137">displayName</span></span>|<span data-ttu-id="f311f-138">String</span><span class="sxs-lookup"><span data-stu-id="f311f-138">String</span></span>|<span data-ttu-id="f311f-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="f311f-139">Display Name of the Role definition.</span></span> <span data-ttu-id="f311f-140">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f311f-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f311f-141">description</span><span class="sxs-lookup"><span data-stu-id="f311f-141">description</span></span>|<span data-ttu-id="f311f-142">String</span><span class="sxs-lookup"><span data-stu-id="f311f-142">String</span></span>|<span data-ttu-id="f311f-143">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="f311f-143">Description of the Role definition.</span></span> <span data-ttu-id="f311f-144">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f311f-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f311f-145">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="f311f-145">rolePermissions</span></span>|<span data-ttu-id="f311f-146">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f311f-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="f311f-147">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="f311f-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="f311f-148">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="f311f-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="f311f-149">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f311f-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f311f-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="f311f-150">isBuiltIn</span></span>|<span data-ttu-id="f311f-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="f311f-151">Boolean</span></span>|<span data-ttu-id="f311f-152">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="f311f-152">Type of Role.</span></span> <span data-ttu-id="f311f-153">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="f311f-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="f311f-154">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f311f-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f311f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f311f-155">Response</span></span>
<span data-ttu-id="f311f-156">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f311f-156">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f311f-157">Пример</span><span class="sxs-lookup"><span data-stu-id="f311f-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="f311f-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="f311f-158">Request</span></span>
<span data-ttu-id="f311f-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f311f-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="f311f-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="f311f-160">Response</span></span>
<span data-ttu-id="f311f-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f311f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```









