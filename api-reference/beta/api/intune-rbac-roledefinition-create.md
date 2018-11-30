---
title: Создание roleDefinition
description: Создание объекта roleDefinition.
ms.openlocfilehash: 6772b065e4d4d73615540667470829b31a2de804
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082850"
---
# <a name="create-roledefinition"></a><span data-ttu-id="4ceff-103">Создание roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4ceff-103">Create roleDefinition</span></span>

> <span data-ttu-id="4ceff-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4ceff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ceff-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ceff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ceff-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4ceff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ceff-107">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4ceff-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ceff-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ceff-108">Prerequisites</span></span>
<span data-ttu-id="4ceff-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ceff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ceff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ceff-111">Permission type</span></span>|<span data-ttu-id="4ceff-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ceff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ceff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ceff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ceff-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ceff-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4ceff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ceff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ceff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ceff-116">Not supported.</span></span>|
|<span data-ttu-id="4ceff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ceff-117">Application</span></span>|<span data-ttu-id="4ceff-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ceff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ceff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ceff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="4ceff-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ceff-120">Request headers</span></span>
|<span data-ttu-id="4ceff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ceff-121">Header</span></span>|<span data-ttu-id="4ceff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4ceff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ceff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ceff-123">Authorization</span></span>|<span data-ttu-id="4ceff-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4ceff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ceff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ceff-125">Accept</span></span>|<span data-ttu-id="4ceff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ceff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ceff-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4ceff-127">Request body</span></span>
<span data-ttu-id="4ceff-128">В теле запроса добавьте представление объекта roleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ceff-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="4ceff-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="4ceff-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="4ceff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ceff-130">Property</span></span>|<span data-ttu-id="4ceff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4ceff-131">Type</span></span>|<span data-ttu-id="4ceff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4ceff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ceff-133">id</span><span class="sxs-lookup"><span data-stu-id="4ceff-133">id</span></span>|<span data-ttu-id="4ceff-134">String</span><span class="sxs-lookup"><span data-stu-id="4ceff-134">String</span></span>|<span data-ttu-id="4ceff-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4ceff-135">Key of the entity.</span></span> <span data-ttu-id="4ceff-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="4ceff-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="4ceff-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4ceff-137">displayName</span></span>|<span data-ttu-id="4ceff-138">String</span><span class="sxs-lookup"><span data-stu-id="4ceff-138">String</span></span>|<span data-ttu-id="4ceff-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="4ceff-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="4ceff-140">описание</span><span class="sxs-lookup"><span data-stu-id="4ceff-140">description</span></span>|<span data-ttu-id="4ceff-141">String</span><span class="sxs-lookup"><span data-stu-id="4ceff-141">String</span></span>|<span data-ttu-id="4ceff-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="4ceff-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="4ceff-143">permissions</span><span class="sxs-lookup"><span data-stu-id="4ceff-143">permissions</span></span>|<span data-ttu-id="4ceff-144">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="4ceff-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="4ceff-145">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="4ceff-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="4ceff-146">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="4ceff-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="4ceff-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="4ceff-147">rolePermissions</span></span>|<span data-ttu-id="4ceff-148">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="4ceff-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="4ceff-149">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="4ceff-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="4ceff-150">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="4ceff-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="4ceff-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4ceff-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="4ceff-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ceff-152">Boolean</span></span>|<span data-ttu-id="4ceff-153">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="4ceff-153">Type of Role.</span></span> <span data-ttu-id="4ceff-154">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="4ceff-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="4ceff-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="4ceff-155">isBuiltIn</span></span>|<span data-ttu-id="4ceff-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ceff-156">Boolean</span></span>|<span data-ttu-id="4ceff-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="4ceff-157">Type of Role.</span></span> <span data-ttu-id="4ceff-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="4ceff-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="4ceff-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ceff-159">Response</span></span>
<span data-ttu-id="4ceff-160">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4ceff-160">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ceff-161">Пример</span><span class="sxs-lookup"><span data-stu-id="4ceff-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ceff-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ceff-162">Request</span></span>
<span data-ttu-id="4ceff-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ceff-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 1145

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
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="4ceff-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ceff-164">Response</span></span>
<span data-ttu-id="4ceff-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4ceff-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





