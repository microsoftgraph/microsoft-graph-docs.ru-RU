---
title: Создание roleDefinition
description: Создание объекта roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 82f009a5dec96f6352780d8db92cf5e35277bf4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025972"
---
# <a name="create-roledefinition"></a><span data-ttu-id="275cf-103">Создание roleDefinition</span><span class="sxs-lookup"><span data-stu-id="275cf-103">Create roleDefinition</span></span>

> <span data-ttu-id="275cf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="275cf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="275cf-105">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="275cf-105">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="275cf-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="275cf-106">Prerequisites</span></span>
<span data-ttu-id="275cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="275cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="275cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="275cf-109">Permission type</span></span>|<span data-ttu-id="275cf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="275cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="275cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="275cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="275cf-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="275cf-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="275cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="275cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="275cf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="275cf-114">Not supported.</span></span>|
|<span data-ttu-id="275cf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="275cf-115">Application</span></span>|<span data-ttu-id="275cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="275cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="275cf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="275cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="275cf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="275cf-118">Request headers</span></span>
|<span data-ttu-id="275cf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="275cf-119">Header</span></span>|<span data-ttu-id="275cf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="275cf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="275cf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="275cf-121">Authorization</span></span>|<span data-ttu-id="275cf-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="275cf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="275cf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="275cf-123">Accept</span></span>|<span data-ttu-id="275cf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="275cf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="275cf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="275cf-125">Request body</span></span>
<span data-ttu-id="275cf-126">В теле запроса добавьте представление объекта roleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="275cf-126">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="275cf-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="275cf-127">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="275cf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="275cf-128">Property</span></span>|<span data-ttu-id="275cf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="275cf-129">Type</span></span>|<span data-ttu-id="275cf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="275cf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="275cf-131">id</span><span class="sxs-lookup"><span data-stu-id="275cf-131">id</span></span>|<span data-ttu-id="275cf-132">String</span><span class="sxs-lookup"><span data-stu-id="275cf-132">String</span></span>|<span data-ttu-id="275cf-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="275cf-133">Key of the entity.</span></span> <span data-ttu-id="275cf-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="275cf-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="275cf-135">displayName</span><span class="sxs-lookup"><span data-stu-id="275cf-135">displayName</span></span>|<span data-ttu-id="275cf-136">Строка</span><span class="sxs-lookup"><span data-stu-id="275cf-136">String</span></span>|<span data-ttu-id="275cf-137">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="275cf-137">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="275cf-138">description</span><span class="sxs-lookup"><span data-stu-id="275cf-138">description</span></span>|<span data-ttu-id="275cf-139">String</span><span class="sxs-lookup"><span data-stu-id="275cf-139">String</span></span>|<span data-ttu-id="275cf-140">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="275cf-140">Description of the Role definition.</span></span>|
|<span data-ttu-id="275cf-141">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="275cf-141">rolePermissions</span></span>|<span data-ttu-id="275cf-142">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="275cf-142">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="275cf-143">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="275cf-143">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="275cf-144">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="275cf-144">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="275cf-145">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="275cf-145">isBuiltIn</span></span>|<span data-ttu-id="275cf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="275cf-146">Boolean</span></span>|<span data-ttu-id="275cf-147">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="275cf-147">Type of Role.</span></span> <span data-ttu-id="275cf-148">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="275cf-148">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="275cf-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="275cf-149">Response</span></span>
<span data-ttu-id="275cf-150">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="275cf-150">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="275cf-151">Пример</span><span class="sxs-lookup"><span data-stu-id="275cf-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="275cf-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="275cf-152">Request</span></span>
<span data-ttu-id="275cf-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="275cf-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="275cf-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="275cf-154">Response</span></span>
<span data-ttu-id="275cf-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="275cf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



