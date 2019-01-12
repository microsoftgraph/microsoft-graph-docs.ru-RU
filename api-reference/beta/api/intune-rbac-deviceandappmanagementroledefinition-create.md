---
title: Создание deviceAndAppManagementRoleDefinition
description: Создание объекта deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bc5438b9d0d4db833949cc4ee84d9d43785b6e2a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926108"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="ea083-103">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ea083-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="ea083-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea083-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea083-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea083-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea083-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ea083-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea083-107">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ea083-107">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea083-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea083-108">Prerequisites</span></span>
<span data-ttu-id="ea083-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea083-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea083-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea083-111">Permission type</span></span>|<span data-ttu-id="ea083-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea083-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea083-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea083-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea083-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea083-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ea083-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea083-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea083-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea083-116">Not supported.</span></span>|
|<span data-ttu-id="ea083-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea083-117">Application</span></span>|<span data-ttu-id="ea083-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea083-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea083-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea083-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ea083-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea083-120">Request headers</span></span>
|<span data-ttu-id="ea083-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea083-121">Header</span></span>|<span data-ttu-id="ea083-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ea083-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea083-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea083-123">Authorization</span></span>|<span data-ttu-id="ea083-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ea083-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea083-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea083-125">Accept</span></span>|<span data-ttu-id="ea083-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea083-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea083-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea083-127">Request body</span></span>
<span data-ttu-id="ea083-128">В теле запроса добавьте представление объекта deviceAndAppManagementRoleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea083-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="ea083-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="ea083-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="ea083-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea083-130">Property</span></span>|<span data-ttu-id="ea083-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ea083-131">Type</span></span>|<span data-ttu-id="ea083-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ea083-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea083-133">id</span><span class="sxs-lookup"><span data-stu-id="ea083-133">id</span></span>|<span data-ttu-id="ea083-134">String</span><span class="sxs-lookup"><span data-stu-id="ea083-134">String</span></span>|<span data-ttu-id="ea083-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ea083-135">Key of the entity.</span></span> <span data-ttu-id="ea083-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="ea083-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="ea083-137">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ea083-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ea083-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ea083-138">displayName</span></span>|<span data-ttu-id="ea083-139">String</span><span class="sxs-lookup"><span data-stu-id="ea083-139">String</span></span>|<span data-ttu-id="ea083-140">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="ea083-140">Display Name of the Role definition.</span></span> <span data-ttu-id="ea083-141">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ea083-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ea083-142">описание</span><span class="sxs-lookup"><span data-stu-id="ea083-142">description</span></span>|<span data-ttu-id="ea083-143">String</span><span class="sxs-lookup"><span data-stu-id="ea083-143">String</span></span>|<span data-ttu-id="ea083-144">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="ea083-144">Description of the Role definition.</span></span> <span data-ttu-id="ea083-145">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ea083-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ea083-146">permissions</span><span class="sxs-lookup"><span data-stu-id="ea083-146">permissions</span></span>|<span data-ttu-id="ea083-147">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ea083-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ea083-148">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="ea083-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ea083-149">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="ea083-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ea083-150">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ea083-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ea083-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ea083-151">rolePermissions</span></span>|<span data-ttu-id="ea083-152">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ea083-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ea083-153">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="ea083-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ea083-154">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="ea083-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ea083-155">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ea083-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ea083-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ea083-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="ea083-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea083-157">Boolean</span></span>|<span data-ttu-id="ea083-158">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="ea083-158">Type of Role.</span></span> <span data-ttu-id="ea083-159">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="ea083-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ea083-160">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ea083-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ea083-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ea083-161">isBuiltIn</span></span>|<span data-ttu-id="ea083-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea083-162">Boolean</span></span>|<span data-ttu-id="ea083-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="ea083-163">Type of Role.</span></span> <span data-ttu-id="ea083-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="ea083-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ea083-165">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ea083-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ea083-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea083-166">Response</span></span>
<span data-ttu-id="ea083-167">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ea083-167">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea083-168">Пример</span><span class="sxs-lookup"><span data-stu-id="ea083-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea083-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea083-169">Request</span></span>
<span data-ttu-id="ea083-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea083-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 1167

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
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="ea083-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea083-171">Response</span></span>
<span data-ttu-id="ea083-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ea083-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





