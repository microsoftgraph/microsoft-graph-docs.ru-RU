---
title: Обновление объекта roleDefinition
description: Обновление свойств объекта roleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7669e4b4a5ca791ab071a673f8609e409111599
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965766"
---
# <a name="update-roledefinition"></a><span data-ttu-id="37a06-103">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="37a06-103">Update roleDefinition</span></span>

<span data-ttu-id="37a06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37a06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37a06-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37a06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37a06-106">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="37a06-106">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37a06-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="37a06-107">Prerequisites</span></span>
<span data-ttu-id="37a06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37a06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37a06-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37a06-110">Permission type</span></span>|<span data-ttu-id="37a06-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37a06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37a06-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37a06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37a06-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a06-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="37a06-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37a06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37a06-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37a06-115">Not supported.</span></span>|
|<span data-ttu-id="37a06-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37a06-116">Application</span></span>|<span data-ttu-id="37a06-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37a06-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37a06-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37a06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="37a06-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="37a06-119">Request headers</span></span>
|<span data-ttu-id="37a06-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37a06-120">Header</span></span>|<span data-ttu-id="37a06-121">Значение</span><span class="sxs-lookup"><span data-stu-id="37a06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37a06-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="37a06-122">Authorization</span></span>|<span data-ttu-id="37a06-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37a06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37a06-124">Accept</span><span class="sxs-lookup"><span data-stu-id="37a06-124">Accept</span></span>|<span data-ttu-id="37a06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37a06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37a06-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="37a06-126">Request body</span></span>
<span data-ttu-id="37a06-127">В теле запроса добавьте представление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37a06-127">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="37a06-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="37a06-128">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="37a06-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="37a06-129">Property</span></span>|<span data-ttu-id="37a06-130">Тип</span><span class="sxs-lookup"><span data-stu-id="37a06-130">Type</span></span>|<span data-ttu-id="37a06-131">Описание</span><span class="sxs-lookup"><span data-stu-id="37a06-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37a06-132">id</span><span class="sxs-lookup"><span data-stu-id="37a06-132">id</span></span>|<span data-ttu-id="37a06-133">String</span><span class="sxs-lookup"><span data-stu-id="37a06-133">String</span></span>|<span data-ttu-id="37a06-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="37a06-134">Key of the entity.</span></span> <span data-ttu-id="37a06-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="37a06-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="37a06-136">displayName</span><span class="sxs-lookup"><span data-stu-id="37a06-136">displayName</span></span>|<span data-ttu-id="37a06-137">String</span><span class="sxs-lookup"><span data-stu-id="37a06-137">String</span></span>|<span data-ttu-id="37a06-138">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="37a06-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="37a06-139">description</span><span class="sxs-lookup"><span data-stu-id="37a06-139">description</span></span>|<span data-ttu-id="37a06-140">String</span><span class="sxs-lookup"><span data-stu-id="37a06-140">String</span></span>|<span data-ttu-id="37a06-141">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="37a06-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="37a06-142">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="37a06-142">rolePermissions</span></span>|<span data-ttu-id="37a06-143">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="37a06-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="37a06-144">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="37a06-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="37a06-145">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="37a06-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="37a06-146">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="37a06-146">isBuiltIn</span></span>|<span data-ttu-id="37a06-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="37a06-147">Boolean</span></span>|<span data-ttu-id="37a06-148">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="37a06-148">Type of Role.</span></span> <span data-ttu-id="37a06-149">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="37a06-149">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="37a06-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="37a06-150">Response</span></span>
<span data-ttu-id="37a06-151">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="37a06-151">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37a06-152">Пример</span><span class="sxs-lookup"><span data-stu-id="37a06-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="37a06-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="37a06-153">Request</span></span>
<span data-ttu-id="37a06-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37a06-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 580

{
  "@odata.type": "#microsoft.graph.roleDefinition",
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

### <a name="response"></a><span data-ttu-id="37a06-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="37a06-155">Response</span></span>
<span data-ttu-id="37a06-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37a06-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 629

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
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









