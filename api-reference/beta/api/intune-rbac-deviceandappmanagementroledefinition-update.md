---
title: Обновление объекта deviceAndAppManagementRoleDefinition
description: Обновление свойств объекта deviceAndAppManagementRoleDefinition.
ms.openlocfilehash: 81cf688228f37c9b762e6b572d98ae693c33266d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074771"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="de53c-103">Обновление объекта deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="de53c-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="de53c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="de53c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de53c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de53c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de53c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="de53c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de53c-107">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="de53c-107">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de53c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="de53c-108">Prerequisites</span></span>
<span data-ttu-id="de53c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de53c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de53c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de53c-111">Permission type</span></span>|<span data-ttu-id="de53c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de53c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de53c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de53c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de53c-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de53c-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="de53c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de53c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de53c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de53c-116">Not supported.</span></span>|
|<span data-ttu-id="de53c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de53c-117">Application</span></span>|<span data-ttu-id="de53c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de53c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de53c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de53c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="de53c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de53c-120">Request headers</span></span>
|<span data-ttu-id="de53c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de53c-121">Header</span></span>|<span data-ttu-id="de53c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de53c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de53c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de53c-123">Authorization</span></span>|<span data-ttu-id="de53c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="de53c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de53c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de53c-125">Accept</span></span>|<span data-ttu-id="de53c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de53c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de53c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de53c-127">Request body</span></span>
<span data-ttu-id="de53c-128">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de53c-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="de53c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="de53c-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="de53c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="de53c-130">Property</span></span>|<span data-ttu-id="de53c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="de53c-131">Type</span></span>|<span data-ttu-id="de53c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="de53c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de53c-133">id</span><span class="sxs-lookup"><span data-stu-id="de53c-133">id</span></span>|<span data-ttu-id="de53c-134">String</span><span class="sxs-lookup"><span data-stu-id="de53c-134">String</span></span>|<span data-ttu-id="de53c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="de53c-135">Key of the entity.</span></span> <span data-ttu-id="de53c-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="de53c-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="de53c-137">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="de53c-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="de53c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="de53c-138">displayName</span></span>|<span data-ttu-id="de53c-139">String</span><span class="sxs-lookup"><span data-stu-id="de53c-139">String</span></span>|<span data-ttu-id="de53c-140">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="de53c-140">Display Name of the Role definition.</span></span> <span data-ttu-id="de53c-141">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="de53c-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="de53c-142">описание</span><span class="sxs-lookup"><span data-stu-id="de53c-142">description</span></span>|<span data-ttu-id="de53c-143">String</span><span class="sxs-lookup"><span data-stu-id="de53c-143">String</span></span>|<span data-ttu-id="de53c-144">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="de53c-144">Description of the Role definition.</span></span> <span data-ttu-id="de53c-145">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="de53c-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="de53c-146">permissions</span><span class="sxs-lookup"><span data-stu-id="de53c-146">permissions</span></span>|<span data-ttu-id="de53c-147">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="de53c-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="de53c-148">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="de53c-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="de53c-149">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="de53c-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="de53c-150">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="de53c-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="de53c-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="de53c-151">rolePermissions</span></span>|<span data-ttu-id="de53c-152">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="de53c-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="de53c-153">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="de53c-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="de53c-154">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="de53c-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="de53c-155">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="de53c-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="de53c-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="de53c-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="de53c-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="de53c-157">Boolean</span></span>|<span data-ttu-id="de53c-158">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="de53c-158">Type of Role.</span></span> <span data-ttu-id="de53c-159">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="de53c-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="de53c-160">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="de53c-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="de53c-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="de53c-161">isBuiltIn</span></span>|<span data-ttu-id="de53c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="de53c-162">Boolean</span></span>|<span data-ttu-id="de53c-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="de53c-163">Type of Role.</span></span> <span data-ttu-id="de53c-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="de53c-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="de53c-165">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="de53c-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="de53c-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="de53c-166">Response</span></span>
<span data-ttu-id="de53c-167">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="de53c-167">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de53c-168">Пример</span><span class="sxs-lookup"><span data-stu-id="de53c-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="de53c-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="de53c-169">Request</span></span>
<span data-ttu-id="de53c-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de53c-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1092

{
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
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="de53c-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="de53c-171">Response</span></span>
<span data-ttu-id="de53c-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="de53c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1216

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
  "isBuiltIn": true
}
```





