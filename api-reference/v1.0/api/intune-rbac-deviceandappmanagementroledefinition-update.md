---
title: Обновление объекта deviceAndAppManagementRoleDefinition
description: Обновление свойств объекта deviceAndAppManagementRoleDefinition.
author: tfitzmac
ms.openlocfilehash: 74a66dc0480d9b856ee97f8a1c794659469d06b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309137"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="98aca-103">Обновление объекта deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="98aca-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="98aca-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="98aca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98aca-105">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="98aca-105">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98aca-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="98aca-106">Prerequisites</span></span>
<span data-ttu-id="98aca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98aca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98aca-109">Permission type</span></span>|<span data-ttu-id="98aca-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98aca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98aca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98aca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="98aca-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98aca-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="98aca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98aca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98aca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98aca-114">Not supported.</span></span>|
|<span data-ttu-id="98aca-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98aca-115">Application</span></span>|<span data-ttu-id="98aca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98aca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98aca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98aca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="98aca-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98aca-118">Request headers</span></span>
|<span data-ttu-id="98aca-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98aca-119">Header</span></span>|<span data-ttu-id="98aca-120">Значение</span><span class="sxs-lookup"><span data-stu-id="98aca-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98aca-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98aca-121">Authorization</span></span>|<span data-ttu-id="98aca-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="98aca-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98aca-123">Accept</span><span class="sxs-lookup"><span data-stu-id="98aca-123">Accept</span></span>|<span data-ttu-id="98aca-124">application/json</span><span class="sxs-lookup"><span data-stu-id="98aca-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98aca-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98aca-125">Request body</span></span>
<span data-ttu-id="98aca-126">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98aca-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="98aca-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="98aca-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="98aca-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="98aca-128">Property</span></span>|<span data-ttu-id="98aca-129">Тип</span><span class="sxs-lookup"><span data-stu-id="98aca-129">Type</span></span>|<span data-ttu-id="98aca-130">Описание</span><span class="sxs-lookup"><span data-stu-id="98aca-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98aca-131">id</span><span class="sxs-lookup"><span data-stu-id="98aca-131">id</span></span>|<span data-ttu-id="98aca-132">Строка</span><span class="sxs-lookup"><span data-stu-id="98aca-132">String</span></span>|<span data-ttu-id="98aca-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="98aca-133">Key of the entity.</span></span> <span data-ttu-id="98aca-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="98aca-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="98aca-135">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="98aca-135">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="98aca-136">displayName</span><span class="sxs-lookup"><span data-stu-id="98aca-136">displayName</span></span>|<span data-ttu-id="98aca-137">String</span><span class="sxs-lookup"><span data-stu-id="98aca-137">String</span></span>|<span data-ttu-id="98aca-138">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="98aca-138">Display Name of the Role definition.</span></span> <span data-ttu-id="98aca-139">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="98aca-139">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="98aca-140">описание</span><span class="sxs-lookup"><span data-stu-id="98aca-140">description</span></span>|<span data-ttu-id="98aca-141">String</span><span class="sxs-lookup"><span data-stu-id="98aca-141">String</span></span>|<span data-ttu-id="98aca-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="98aca-142">Description of the Role definition.</span></span> <span data-ttu-id="98aca-143">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="98aca-143">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="98aca-144">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="98aca-144">rolePermissions</span></span>|<span data-ttu-id="98aca-145">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="98aca-145">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="98aca-146">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="98aca-146">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="98aca-147">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="98aca-147">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="98aca-148">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="98aca-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="98aca-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="98aca-149">isBuiltIn</span></span>|<span data-ttu-id="98aca-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="98aca-150">Boolean</span></span>|<span data-ttu-id="98aca-151">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="98aca-151">Type of Role.</span></span> <span data-ttu-id="98aca-152">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="98aca-152">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="98aca-153">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="98aca-153">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="98aca-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="98aca-154">Response</span></span>
<span data-ttu-id="98aca-155">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="98aca-155">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98aca-156">Пример</span><span class="sxs-lookup"><span data-stu-id="98aca-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="98aca-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="98aca-157">Request</span></span>
<span data-ttu-id="98aca-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98aca-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="98aca-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="98aca-159">Response</span></span>
<span data-ttu-id="98aca-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="98aca-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



