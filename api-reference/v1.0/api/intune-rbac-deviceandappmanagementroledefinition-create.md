---
title: Создание deviceAndAppManagementRoleDefinition
description: Создание объекта deviceAndAppManagementRoleDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 281c965de97876812510b04a5f131f1354720df8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512323"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="370cd-103">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="370cd-103">Create deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="370cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="370cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="370cd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="370cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="370cd-106">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="370cd-106">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="370cd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="370cd-107">Prerequisites</span></span>
<span data-ttu-id="370cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="370cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="370cd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="370cd-110">Permission type</span></span>|<span data-ttu-id="370cd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="370cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="370cd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="370cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="370cd-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="370cd-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="370cd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="370cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="370cd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="370cd-115">Not supported.</span></span>|
|<span data-ttu-id="370cd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="370cd-116">Application</span></span>|<span data-ttu-id="370cd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="370cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="370cd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="370cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="370cd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="370cd-119">Request headers</span></span>
|<span data-ttu-id="370cd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="370cd-120">Header</span></span>|<span data-ttu-id="370cd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="370cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="370cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="370cd-122">Authorization</span></span>|<span data-ttu-id="370cd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="370cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="370cd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="370cd-124">Accept</span></span>|<span data-ttu-id="370cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="370cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="370cd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="370cd-126">Request body</span></span>
<span data-ttu-id="370cd-127">В теле запроса добавьте представление объекта deviceAndAppManagementRoleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="370cd-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="370cd-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="370cd-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="370cd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="370cd-129">Property</span></span>|<span data-ttu-id="370cd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="370cd-130">Type</span></span>|<span data-ttu-id="370cd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="370cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="370cd-132">id</span><span class="sxs-lookup"><span data-stu-id="370cd-132">id</span></span>|<span data-ttu-id="370cd-133">String</span><span class="sxs-lookup"><span data-stu-id="370cd-133">String</span></span>|<span data-ttu-id="370cd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="370cd-134">Key of the entity.</span></span> <span data-ttu-id="370cd-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="370cd-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="370cd-136">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="370cd-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="370cd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="370cd-137">displayName</span></span>|<span data-ttu-id="370cd-138">Строка</span><span class="sxs-lookup"><span data-stu-id="370cd-138">String</span></span>|<span data-ttu-id="370cd-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="370cd-139">Display Name of the Role definition.</span></span> <span data-ttu-id="370cd-140">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="370cd-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="370cd-141">description</span><span class="sxs-lookup"><span data-stu-id="370cd-141">description</span></span>|<span data-ttu-id="370cd-142">String</span><span class="sxs-lookup"><span data-stu-id="370cd-142">String</span></span>|<span data-ttu-id="370cd-143">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="370cd-143">Description of the Role definition.</span></span> <span data-ttu-id="370cd-144">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="370cd-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="370cd-145">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="370cd-145">rolePermissions</span></span>|<span data-ttu-id="370cd-146">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="370cd-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="370cd-147">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="370cd-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="370cd-148">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="370cd-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="370cd-149">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="370cd-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="370cd-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="370cd-150">isBuiltIn</span></span>|<span data-ttu-id="370cd-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="370cd-151">Boolean</span></span>|<span data-ttu-id="370cd-152">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="370cd-152">Type of Role.</span></span> <span data-ttu-id="370cd-153">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="370cd-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="370cd-154">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="370cd-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="370cd-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="370cd-155">Response</span></span>
<span data-ttu-id="370cd-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="370cd-156">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="370cd-157">Пример</span><span class="sxs-lookup"><span data-stu-id="370cd-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="370cd-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="370cd-158">Request</span></span>
<span data-ttu-id="370cd-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="370cd-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="370cd-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="370cd-160">Response</span></span>
<span data-ttu-id="370cd-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="370cd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




