---
title: Обновление объекта roleDefinition
description: Обновление свойств объекта roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3afe285537bc6ff3476b2aadf70d104801baa793
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934186"
---
# <a name="update-roledefinition"></a><span data-ttu-id="f95c6-103">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="f95c6-103">Update roleDefinition</span></span>

> <span data-ttu-id="f95c6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f95c6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f95c6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f95c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f95c6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f95c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f95c6-107">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f95c6-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f95c6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f95c6-108">Prerequisites</span></span>
<span data-ttu-id="f95c6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f95c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f95c6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f95c6-111">Permission type</span></span>|<span data-ttu-id="f95c6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f95c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f95c6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f95c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f95c6-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f95c6-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f95c6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f95c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f95c6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f95c6-116">Not supported.</span></span>|
|<span data-ttu-id="f95c6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f95c6-117">Application</span></span>|<span data-ttu-id="f95c6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f95c6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f95c6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f95c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="f95c6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f95c6-120">Request headers</span></span>
|<span data-ttu-id="f95c6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f95c6-121">Header</span></span>|<span data-ttu-id="f95c6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f95c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f95c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f95c6-123">Authorization</span></span>|<span data-ttu-id="f95c6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f95c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f95c6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f95c6-125">Accept</span></span>|<span data-ttu-id="f95c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f95c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f95c6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f95c6-127">Request body</span></span>
<span data-ttu-id="f95c6-128">В теле запроса добавьте представление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f95c6-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="f95c6-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f95c6-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="f95c6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f95c6-130">Property</span></span>|<span data-ttu-id="f95c6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f95c6-131">Type</span></span>|<span data-ttu-id="f95c6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f95c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f95c6-133">id</span><span class="sxs-lookup"><span data-stu-id="f95c6-133">id</span></span>|<span data-ttu-id="f95c6-134">String</span><span class="sxs-lookup"><span data-stu-id="f95c6-134">String</span></span>|<span data-ttu-id="f95c6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f95c6-135">Key of the entity.</span></span> <span data-ttu-id="f95c6-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="f95c6-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="f95c6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f95c6-137">displayName</span></span>|<span data-ttu-id="f95c6-138">String</span><span class="sxs-lookup"><span data-stu-id="f95c6-138">String</span></span>|<span data-ttu-id="f95c6-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="f95c6-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="f95c6-140">описание</span><span class="sxs-lookup"><span data-stu-id="f95c6-140">description</span></span>|<span data-ttu-id="f95c6-141">String</span><span class="sxs-lookup"><span data-stu-id="f95c6-141">String</span></span>|<span data-ttu-id="f95c6-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="f95c6-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="f95c6-143">permissions</span><span class="sxs-lookup"><span data-stu-id="f95c6-143">permissions</span></span>|<span data-ttu-id="f95c6-144">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f95c6-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="f95c6-145">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="f95c6-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="f95c6-146">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="f95c6-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="f95c6-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="f95c6-147">rolePermissions</span></span>|<span data-ttu-id="f95c6-148">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f95c6-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="f95c6-149">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="f95c6-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="f95c6-150">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="f95c6-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="f95c6-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f95c6-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="f95c6-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95c6-152">Boolean</span></span>|<span data-ttu-id="f95c6-153">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="f95c6-153">Type of Role.</span></span> <span data-ttu-id="f95c6-154">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="f95c6-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="f95c6-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="f95c6-155">isBuiltIn</span></span>|<span data-ttu-id="f95c6-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95c6-156">Boolean</span></span>|<span data-ttu-id="f95c6-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="f95c6-157">Type of Role.</span></span> <span data-ttu-id="f95c6-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="f95c6-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="f95c6-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="f95c6-159">Response</span></span>
<span data-ttu-id="f95c6-160">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f95c6-160">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f95c6-161">Пример</span><span class="sxs-lookup"><span data-stu-id="f95c6-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="f95c6-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="f95c6-162">Request</span></span>
<span data-ttu-id="f95c6-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f95c6-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f95c6-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="f95c6-164">Response</span></span>
<span data-ttu-id="f95c6-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f95c6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1194

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
  "isBuiltIn": true
}
```





