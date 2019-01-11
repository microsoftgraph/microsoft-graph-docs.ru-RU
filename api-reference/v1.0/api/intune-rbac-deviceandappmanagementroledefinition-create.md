---
title: Создание deviceAndAppManagementRoleDefinition
description: Создание объекта deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f1eb68651a32f10d2b8daaab4fe7eaac0b8b2666
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826035"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="ddd01-103">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ddd01-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="ddd01-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ddd01-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddd01-105">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ddd01-105">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ddd01-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ddd01-106">Prerequisites</span></span>
<span data-ttu-id="ddd01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddd01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddd01-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddd01-109">Permission type</span></span>|<span data-ttu-id="ddd01-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddd01-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddd01-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddd01-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ddd01-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddd01-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ddd01-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddd01-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddd01-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddd01-114">Not supported.</span></span>|
|<span data-ttu-id="ddd01-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddd01-115">Application</span></span>|<span data-ttu-id="ddd01-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddd01-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddd01-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddd01-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ddd01-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddd01-118">Request headers</span></span>
|<span data-ttu-id="ddd01-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddd01-119">Header</span></span>|<span data-ttu-id="ddd01-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ddd01-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddd01-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddd01-121">Authorization</span></span>|<span data-ttu-id="ddd01-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ddd01-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddd01-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ddd01-123">Accept</span></span>|<span data-ttu-id="ddd01-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ddd01-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddd01-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ddd01-125">Request body</span></span>
<span data-ttu-id="ddd01-126">В теле запроса добавьте представление объекта deviceAndAppManagementRoleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddd01-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="ddd01-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="ddd01-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="ddd01-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddd01-128">Property</span></span>|<span data-ttu-id="ddd01-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ddd01-129">Type</span></span>|<span data-ttu-id="ddd01-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ddd01-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddd01-131">id</span><span class="sxs-lookup"><span data-stu-id="ddd01-131">id</span></span>|<span data-ttu-id="ddd01-132">Строка</span><span class="sxs-lookup"><span data-stu-id="ddd01-132">String</span></span>|<span data-ttu-id="ddd01-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ddd01-133">Key of the entity.</span></span> <span data-ttu-id="ddd01-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="ddd01-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="ddd01-135">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ddd01-135">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ddd01-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ddd01-136">displayName</span></span>|<span data-ttu-id="ddd01-137">String</span><span class="sxs-lookup"><span data-stu-id="ddd01-137">String</span></span>|<span data-ttu-id="ddd01-138">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="ddd01-138">Display Name of the Role definition.</span></span> <span data-ttu-id="ddd01-139">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ddd01-139">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ddd01-140">описание</span><span class="sxs-lookup"><span data-stu-id="ddd01-140">description</span></span>|<span data-ttu-id="ddd01-141">String</span><span class="sxs-lookup"><span data-stu-id="ddd01-141">String</span></span>|<span data-ttu-id="ddd01-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="ddd01-142">Description of the Role definition.</span></span> <span data-ttu-id="ddd01-143">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ddd01-143">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ddd01-144">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ddd01-144">rolePermissions</span></span>|<span data-ttu-id="ddd01-145">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ddd01-145">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ddd01-146">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="ddd01-146">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ddd01-147">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="ddd01-147">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ddd01-148">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ddd01-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ddd01-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ddd01-149">isBuiltIn</span></span>|<span data-ttu-id="ddd01-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddd01-150">Boolean</span></span>|<span data-ttu-id="ddd01-151">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="ddd01-151">Type of Role.</span></span> <span data-ttu-id="ddd01-152">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="ddd01-152">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ddd01-153">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ddd01-153">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ddd01-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddd01-154">Response</span></span>
<span data-ttu-id="ddd01-155">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ddd01-155">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddd01-156">Пример</span><span class="sxs-lookup"><span data-stu-id="ddd01-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="ddd01-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddd01-157">Request</span></span>
<span data-ttu-id="ddd01-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddd01-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="ddd01-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="ddd01-159">Response</span></span>
<span data-ttu-id="ddd01-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ddd01-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



