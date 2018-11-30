---
title: Обновление объекта roleDefinition
description: Обновление свойств объекта roleDefinition.
ms.openlocfilehash: 2ceb1024b45efdf47deabac3c90fe923638f42d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025497"
---
# <a name="update-roledefinition"></a><span data-ttu-id="2243e-103">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2243e-103">Update roleDefinition</span></span>

> <span data-ttu-id="2243e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2243e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2243e-105">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2243e-105">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2243e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2243e-106">Prerequisites</span></span>
<span data-ttu-id="2243e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2243e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2243e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2243e-109">Permission type</span></span>|<span data-ttu-id="2243e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2243e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2243e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2243e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2243e-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2243e-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="2243e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2243e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2243e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2243e-114">Not supported.</span></span>|
|<span data-ttu-id="2243e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2243e-115">Application</span></span>|<span data-ttu-id="2243e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2243e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2243e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2243e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="2243e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2243e-118">Request headers</span></span>
|<span data-ttu-id="2243e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2243e-119">Header</span></span>|<span data-ttu-id="2243e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2243e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2243e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2243e-121">Authorization</span></span>|<span data-ttu-id="2243e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2243e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2243e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2243e-123">Accept</span></span>|<span data-ttu-id="2243e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2243e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2243e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2243e-125">Request body</span></span>
<span data-ttu-id="2243e-126">В теле запроса добавьте представление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2243e-126">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="2243e-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2243e-127">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="2243e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2243e-128">Property</span></span>|<span data-ttu-id="2243e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2243e-129">Type</span></span>|<span data-ttu-id="2243e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2243e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2243e-131">id</span><span class="sxs-lookup"><span data-stu-id="2243e-131">id</span></span>|<span data-ttu-id="2243e-132">String</span><span class="sxs-lookup"><span data-stu-id="2243e-132">String</span></span>|<span data-ttu-id="2243e-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2243e-133">Key of the entity.</span></span> <span data-ttu-id="2243e-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="2243e-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="2243e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2243e-135">displayName</span></span>|<span data-ttu-id="2243e-136">String</span><span class="sxs-lookup"><span data-stu-id="2243e-136">String</span></span>|<span data-ttu-id="2243e-137">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="2243e-137">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="2243e-138">описание</span><span class="sxs-lookup"><span data-stu-id="2243e-138">description</span></span>|<span data-ttu-id="2243e-139">String</span><span class="sxs-lookup"><span data-stu-id="2243e-139">String</span></span>|<span data-ttu-id="2243e-140">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="2243e-140">Description of the Role definition.</span></span>|
|<span data-ttu-id="2243e-141">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="2243e-141">rolePermissions</span></span>|<span data-ttu-id="2243e-142">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="2243e-142">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="2243e-143">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="2243e-143">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="2243e-144">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="2243e-144">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="2243e-145">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="2243e-145">isBuiltIn</span></span>|<span data-ttu-id="2243e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2243e-146">Boolean</span></span>|<span data-ttu-id="2243e-147">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="2243e-147">Type of Role.</span></span> <span data-ttu-id="2243e-148">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="2243e-148">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="2243e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="2243e-149">Response</span></span>
<span data-ttu-id="2243e-150">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2243e-150">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2243e-151">Пример</span><span class="sxs-lookup"><span data-stu-id="2243e-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="2243e-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="2243e-152">Request</span></span>
<span data-ttu-id="2243e-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2243e-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2243e-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="2243e-154">Response</span></span>
<span data-ttu-id="2243e-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2243e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



