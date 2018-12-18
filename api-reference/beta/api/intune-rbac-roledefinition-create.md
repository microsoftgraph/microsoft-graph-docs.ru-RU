---
title: Создание roleDefinition
description: Создание объекта roleDefinition.
author: tfitzmac
ms.openlocfilehash: 03134f270d49002c5882a1e65cb0c4454684cd4a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337347"
---
# <a name="create-roledefinition"></a><span data-ttu-id="00391-103">Создание roleDefinition</span><span class="sxs-lookup"><span data-stu-id="00391-103">Create roleDefinition</span></span>

> <span data-ttu-id="00391-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="00391-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00391-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00391-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00391-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00391-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00391-107">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="00391-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00391-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="00391-108">Prerequisites</span></span>
<span data-ttu-id="00391-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00391-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00391-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00391-111">Permission type</span></span>|<span data-ttu-id="00391-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00391-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00391-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00391-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00391-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00391-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="00391-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00391-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00391-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00391-116">Not supported.</span></span>|
|<span data-ttu-id="00391-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00391-117">Application</span></span>|<span data-ttu-id="00391-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00391-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00391-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00391-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="00391-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00391-120">Request headers</span></span>
|<span data-ttu-id="00391-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00391-121">Header</span></span>|<span data-ttu-id="00391-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00391-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00391-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00391-123">Authorization</span></span>|<span data-ttu-id="00391-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="00391-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00391-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00391-125">Accept</span></span>|<span data-ttu-id="00391-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00391-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00391-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00391-127">Request body</span></span>
<span data-ttu-id="00391-128">В теле запроса добавьте представление объекта roleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00391-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="00391-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="00391-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="00391-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="00391-130">Property</span></span>|<span data-ttu-id="00391-131">Тип</span><span class="sxs-lookup"><span data-stu-id="00391-131">Type</span></span>|<span data-ttu-id="00391-132">Описание</span><span class="sxs-lookup"><span data-stu-id="00391-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00391-133">id</span><span class="sxs-lookup"><span data-stu-id="00391-133">id</span></span>|<span data-ttu-id="00391-134">Строка</span><span class="sxs-lookup"><span data-stu-id="00391-134">String</span></span>|<span data-ttu-id="00391-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="00391-135">Key of the entity.</span></span> <span data-ttu-id="00391-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="00391-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="00391-137">displayName</span><span class="sxs-lookup"><span data-stu-id="00391-137">displayName</span></span>|<span data-ttu-id="00391-138">String</span><span class="sxs-lookup"><span data-stu-id="00391-138">String</span></span>|<span data-ttu-id="00391-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="00391-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="00391-140">описание</span><span class="sxs-lookup"><span data-stu-id="00391-140">description</span></span>|<span data-ttu-id="00391-141">String</span><span class="sxs-lookup"><span data-stu-id="00391-141">String</span></span>|<span data-ttu-id="00391-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="00391-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="00391-143">permissions</span><span class="sxs-lookup"><span data-stu-id="00391-143">permissions</span></span>|<span data-ttu-id="00391-144">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="00391-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="00391-145">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="00391-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="00391-146">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="00391-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="00391-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="00391-147">rolePermissions</span></span>|<span data-ttu-id="00391-148">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="00391-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="00391-149">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="00391-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="00391-150">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="00391-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="00391-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="00391-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="00391-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="00391-152">Boolean</span></span>|<span data-ttu-id="00391-153">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="00391-153">Type of Role.</span></span> <span data-ttu-id="00391-154">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="00391-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="00391-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="00391-155">isBuiltIn</span></span>|<span data-ttu-id="00391-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="00391-156">Boolean</span></span>|<span data-ttu-id="00391-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="00391-157">Type of Role.</span></span> <span data-ttu-id="00391-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="00391-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="00391-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="00391-159">Response</span></span>
<span data-ttu-id="00391-160">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="00391-160">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00391-161">Пример</span><span class="sxs-lookup"><span data-stu-id="00391-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="00391-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="00391-162">Request</span></span>
<span data-ttu-id="00391-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00391-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="00391-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="00391-164">Response</span></span>
<span data-ttu-id="00391-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="00391-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





