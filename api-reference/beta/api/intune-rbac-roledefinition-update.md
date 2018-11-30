---
title: Обновление объекта roleDefinition
description: Обновление свойств объекта roleDefinition.
ms.openlocfilehash: debf63b5d0b7116a1e8d1f9274868d97c3cb8931
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075444"
---
# <a name="update-roledefinition"></a><span data-ttu-id="14863-103">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="14863-103">Update roleDefinition</span></span>

> <span data-ttu-id="14863-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="14863-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14863-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14863-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14863-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="14863-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14863-107">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="14863-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="14863-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="14863-108">Prerequisites</span></span>
<span data-ttu-id="14863-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14863-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14863-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14863-111">Permission type</span></span>|<span data-ttu-id="14863-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14863-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14863-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14863-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14863-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14863-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="14863-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14863-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14863-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14863-116">Not supported.</span></span>|
|<span data-ttu-id="14863-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14863-117">Application</span></span>|<span data-ttu-id="14863-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14863-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14863-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14863-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="14863-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14863-120">Request headers</span></span>
|<span data-ttu-id="14863-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14863-121">Header</span></span>|<span data-ttu-id="14863-122">Значение</span><span class="sxs-lookup"><span data-stu-id="14863-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14863-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14863-123">Authorization</span></span>|<span data-ttu-id="14863-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="14863-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14863-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14863-125">Accept</span></span>|<span data-ttu-id="14863-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14863-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14863-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14863-127">Request body</span></span>
<span data-ttu-id="14863-128">В теле запроса добавьте представление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14863-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="14863-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="14863-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="14863-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="14863-130">Property</span></span>|<span data-ttu-id="14863-131">Тип</span><span class="sxs-lookup"><span data-stu-id="14863-131">Type</span></span>|<span data-ttu-id="14863-132">Описание</span><span class="sxs-lookup"><span data-stu-id="14863-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14863-133">id</span><span class="sxs-lookup"><span data-stu-id="14863-133">id</span></span>|<span data-ttu-id="14863-134">String</span><span class="sxs-lookup"><span data-stu-id="14863-134">String</span></span>|<span data-ttu-id="14863-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="14863-135">Key of the entity.</span></span> <span data-ttu-id="14863-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="14863-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="14863-137">displayName</span><span class="sxs-lookup"><span data-stu-id="14863-137">displayName</span></span>|<span data-ttu-id="14863-138">String</span><span class="sxs-lookup"><span data-stu-id="14863-138">String</span></span>|<span data-ttu-id="14863-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="14863-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="14863-140">описание</span><span class="sxs-lookup"><span data-stu-id="14863-140">description</span></span>|<span data-ttu-id="14863-141">String</span><span class="sxs-lookup"><span data-stu-id="14863-141">String</span></span>|<span data-ttu-id="14863-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="14863-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="14863-143">permissions</span><span class="sxs-lookup"><span data-stu-id="14863-143">permissions</span></span>|<span data-ttu-id="14863-144">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="14863-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="14863-145">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="14863-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="14863-146">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="14863-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="14863-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="14863-147">rolePermissions</span></span>|<span data-ttu-id="14863-148">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="14863-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="14863-149">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="14863-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="14863-150">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="14863-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="14863-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="14863-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="14863-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="14863-152">Boolean</span></span>|<span data-ttu-id="14863-153">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="14863-153">Type of Role.</span></span> <span data-ttu-id="14863-154">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="14863-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="14863-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="14863-155">isBuiltIn</span></span>|<span data-ttu-id="14863-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="14863-156">Boolean</span></span>|<span data-ttu-id="14863-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="14863-157">Type of Role.</span></span> <span data-ttu-id="14863-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="14863-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="14863-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="14863-159">Response</span></span>
<span data-ttu-id="14863-160">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="14863-160">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14863-161">Пример</span><span class="sxs-lookup"><span data-stu-id="14863-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="14863-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="14863-162">Request</span></span>
<span data-ttu-id="14863-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14863-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14863-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="14863-164">Response</span></span>
<span data-ttu-id="14863-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="14863-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





