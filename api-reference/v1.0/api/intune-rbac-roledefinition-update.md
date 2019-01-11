---
title: Обновление объекта roleDefinition
description: Обновление свойств объекта roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ee8e773f01aeeb6a3190b4de9c0f0b0d99e8977f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861623"
---
# <a name="update-roledefinition"></a><span data-ttu-id="11d04-103">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="11d04-103">Update roleDefinition</span></span>

> <span data-ttu-id="11d04-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="11d04-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11d04-105">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11d04-105">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11d04-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="11d04-106">Prerequisites</span></span>
<span data-ttu-id="11d04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11d04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11d04-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11d04-109">Permission type</span></span>|<span data-ttu-id="11d04-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11d04-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11d04-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11d04-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11d04-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11d04-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="11d04-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11d04-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11d04-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11d04-114">Not supported.</span></span>|
|<span data-ttu-id="11d04-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11d04-115">Application</span></span>|<span data-ttu-id="11d04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11d04-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11d04-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11d04-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="11d04-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11d04-118">Request headers</span></span>
|<span data-ttu-id="11d04-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11d04-119">Header</span></span>|<span data-ttu-id="11d04-120">Значение</span><span class="sxs-lookup"><span data-stu-id="11d04-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11d04-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="11d04-121">Authorization</span></span>|<span data-ttu-id="11d04-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="11d04-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11d04-123">Accept</span><span class="sxs-lookup"><span data-stu-id="11d04-123">Accept</span></span>|<span data-ttu-id="11d04-124">application/json</span><span class="sxs-lookup"><span data-stu-id="11d04-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11d04-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="11d04-125">Request body</span></span>
<span data-ttu-id="11d04-126">В теле запроса добавьте представление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11d04-126">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="11d04-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11d04-127">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="11d04-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="11d04-128">Property</span></span>|<span data-ttu-id="11d04-129">Тип</span><span class="sxs-lookup"><span data-stu-id="11d04-129">Type</span></span>|<span data-ttu-id="11d04-130">Описание</span><span class="sxs-lookup"><span data-stu-id="11d04-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11d04-131">id</span><span class="sxs-lookup"><span data-stu-id="11d04-131">id</span></span>|<span data-ttu-id="11d04-132">Строка</span><span class="sxs-lookup"><span data-stu-id="11d04-132">String</span></span>|<span data-ttu-id="11d04-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="11d04-133">Key of the entity.</span></span> <span data-ttu-id="11d04-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="11d04-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="11d04-135">displayName</span><span class="sxs-lookup"><span data-stu-id="11d04-135">displayName</span></span>|<span data-ttu-id="11d04-136">String</span><span class="sxs-lookup"><span data-stu-id="11d04-136">String</span></span>|<span data-ttu-id="11d04-137">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="11d04-137">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="11d04-138">описание</span><span class="sxs-lookup"><span data-stu-id="11d04-138">description</span></span>|<span data-ttu-id="11d04-139">String</span><span class="sxs-lookup"><span data-stu-id="11d04-139">String</span></span>|<span data-ttu-id="11d04-140">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="11d04-140">Description of the Role definition.</span></span>|
|<span data-ttu-id="11d04-141">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="11d04-141">rolePermissions</span></span>|<span data-ttu-id="11d04-142">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="11d04-142">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="11d04-143">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="11d04-143">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="11d04-144">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="11d04-144">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="11d04-145">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="11d04-145">isBuiltIn</span></span>|<span data-ttu-id="11d04-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="11d04-146">Boolean</span></span>|<span data-ttu-id="11d04-147">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="11d04-147">Type of Role.</span></span> <span data-ttu-id="11d04-148">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="11d04-148">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="11d04-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="11d04-149">Response</span></span>
<span data-ttu-id="11d04-150">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="11d04-150">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11d04-151">Пример</span><span class="sxs-lookup"><span data-stu-id="11d04-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="11d04-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="11d04-152">Request</span></span>
<span data-ttu-id="11d04-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11d04-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11d04-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="11d04-154">Response</span></span>
<span data-ttu-id="11d04-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="11d04-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



