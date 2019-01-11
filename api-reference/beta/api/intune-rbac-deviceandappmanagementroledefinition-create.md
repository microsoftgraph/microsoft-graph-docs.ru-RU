---
title: Создание deviceAndAppManagementRoleDefinition
description: Создание объекта deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 69a5dee8677ae47a5055782b0ac53bc4c11d3112
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857388"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="5eb84-103">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5eb84-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="5eb84-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5eb84-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5eb84-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eb84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5eb84-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5eb84-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5eb84-107">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5eb84-107">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5eb84-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5eb84-108">Prerequisites</span></span>
<span data-ttu-id="5eb84-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eb84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eb84-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5eb84-111">Permission type</span></span>|<span data-ttu-id="5eb84-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5eb84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5eb84-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5eb84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5eb84-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eb84-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5eb84-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5eb84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5eb84-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eb84-116">Not supported.</span></span>|
|<span data-ttu-id="5eb84-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5eb84-117">Application</span></span>|<span data-ttu-id="5eb84-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eb84-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5eb84-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5eb84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="5eb84-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5eb84-120">Request headers</span></span>
|<span data-ttu-id="5eb84-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5eb84-121">Header</span></span>|<span data-ttu-id="5eb84-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5eb84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5eb84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eb84-123">Authorization</span></span>|<span data-ttu-id="5eb84-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5eb84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5eb84-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5eb84-125">Accept</span></span>|<span data-ttu-id="5eb84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5eb84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eb84-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5eb84-127">Request body</span></span>
<span data-ttu-id="5eb84-128">В теле запроса добавьте представление объекта deviceAndAppManagementRoleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5eb84-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="5eb84-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="5eb84-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="5eb84-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5eb84-130">Property</span></span>|<span data-ttu-id="5eb84-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5eb84-131">Type</span></span>|<span data-ttu-id="5eb84-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5eb84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eb84-133">id</span><span class="sxs-lookup"><span data-stu-id="5eb84-133">id</span></span>|<span data-ttu-id="5eb84-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5eb84-134">String</span></span>|<span data-ttu-id="5eb84-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5eb84-135">Key of the entity.</span></span> <span data-ttu-id="5eb84-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="5eb84-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="5eb84-137">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5eb84-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5eb84-138">displayName</span><span class="sxs-lookup"><span data-stu-id="5eb84-138">displayName</span></span>|<span data-ttu-id="5eb84-139">String</span><span class="sxs-lookup"><span data-stu-id="5eb84-139">String</span></span>|<span data-ttu-id="5eb84-140">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="5eb84-140">Display Name of the Role definition.</span></span> <span data-ttu-id="5eb84-141">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5eb84-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5eb84-142">описание</span><span class="sxs-lookup"><span data-stu-id="5eb84-142">description</span></span>|<span data-ttu-id="5eb84-143">String</span><span class="sxs-lookup"><span data-stu-id="5eb84-143">String</span></span>|<span data-ttu-id="5eb84-144">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="5eb84-144">Description of the Role definition.</span></span> <span data-ttu-id="5eb84-145">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5eb84-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5eb84-146">permissions</span><span class="sxs-lookup"><span data-stu-id="5eb84-146">permissions</span></span>|<span data-ttu-id="5eb84-147">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="5eb84-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="5eb84-148">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="5eb84-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="5eb84-149">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="5eb84-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="5eb84-150">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5eb84-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5eb84-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="5eb84-151">rolePermissions</span></span>|<span data-ttu-id="5eb84-152">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="5eb84-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="5eb84-153">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="5eb84-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="5eb84-154">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="5eb84-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="5eb84-155">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5eb84-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5eb84-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5eb84-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="5eb84-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eb84-157">Boolean</span></span>|<span data-ttu-id="5eb84-158">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="5eb84-158">Type of Role.</span></span> <span data-ttu-id="5eb84-159">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="5eb84-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="5eb84-160">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5eb84-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5eb84-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="5eb84-161">isBuiltIn</span></span>|<span data-ttu-id="5eb84-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eb84-162">Boolean</span></span>|<span data-ttu-id="5eb84-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="5eb84-163">Type of Role.</span></span> <span data-ttu-id="5eb84-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="5eb84-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="5eb84-165">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5eb84-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5eb84-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eb84-166">Response</span></span>
<span data-ttu-id="5eb84-167">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5eb84-167">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eb84-168">Пример</span><span class="sxs-lookup"><span data-stu-id="5eb84-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="5eb84-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="5eb84-169">Request</span></span>
<span data-ttu-id="5eb84-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5eb84-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5eb84-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="5eb84-171">Response</span></span>
<span data-ttu-id="5eb84-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5eb84-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





