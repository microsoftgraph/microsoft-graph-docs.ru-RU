---
title: Создание roleDefinition
description: Создание объекта roleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e331d5f11874408226cc946058001ad300f46dea
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752485"
---
# <a name="create-roledefinition"></a><span data-ttu-id="b76a2-103">Создание roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b76a2-103">Create roleDefinition</span></span>

<span data-ttu-id="b76a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b76a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b76a2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b76a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b76a2-106">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b76a2-106">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b76a2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b76a2-107">Prerequisites</span></span>
<span data-ttu-id="b76a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b76a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b76a2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b76a2-110">Permission type</span></span>|<span data-ttu-id="b76a2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b76a2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b76a2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b76a2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b76a2-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b76a2-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b76a2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b76a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b76a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b76a2-115">Not supported.</span></span>|
|<span data-ttu-id="b76a2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b76a2-116">Application</span></span>|<span data-ttu-id="b76a2-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b76a2-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b76a2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b76a2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="b76a2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b76a2-119">Request headers</span></span>
|<span data-ttu-id="b76a2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b76a2-120">Header</span></span>|<span data-ttu-id="b76a2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b76a2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b76a2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b76a2-122">Authorization</span></span>|<span data-ttu-id="b76a2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b76a2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b76a2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b76a2-124">Accept</span></span>|<span data-ttu-id="b76a2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b76a2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b76a2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b76a2-126">Request body</span></span>
<span data-ttu-id="b76a2-127">В теле запроса добавьте представление объекта roleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b76a2-127">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="b76a2-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="b76a2-128">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="b76a2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b76a2-129">Property</span></span>|<span data-ttu-id="b76a2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b76a2-130">Type</span></span>|<span data-ttu-id="b76a2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b76a2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b76a2-132">id</span><span class="sxs-lookup"><span data-stu-id="b76a2-132">id</span></span>|<span data-ttu-id="b76a2-133">String</span><span class="sxs-lookup"><span data-stu-id="b76a2-133">String</span></span>|<span data-ttu-id="b76a2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b76a2-134">Key of the entity.</span></span> <span data-ttu-id="b76a2-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="b76a2-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b76a2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b76a2-136">displayName</span></span>|<span data-ttu-id="b76a2-137">String</span><span class="sxs-lookup"><span data-stu-id="b76a2-137">String</span></span>|<span data-ttu-id="b76a2-138">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="b76a2-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="b76a2-139">description</span><span class="sxs-lookup"><span data-stu-id="b76a2-139">description</span></span>|<span data-ttu-id="b76a2-140">String</span><span class="sxs-lookup"><span data-stu-id="b76a2-140">String</span></span>|<span data-ttu-id="b76a2-141">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="b76a2-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="b76a2-142">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="b76a2-142">rolePermissions</span></span>|<span data-ttu-id="b76a2-143">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="b76a2-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="b76a2-144">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="b76a2-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="b76a2-145">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="b76a2-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="b76a2-146">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="b76a2-146">isBuiltIn</span></span>|<span data-ttu-id="b76a2-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="b76a2-147">Boolean</span></span>|<span data-ttu-id="b76a2-148">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="b76a2-148">Type of Role.</span></span> <span data-ttu-id="b76a2-149">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="b76a2-149">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="b76a2-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="b76a2-150">Response</span></span>
<span data-ttu-id="b76a2-151">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b76a2-151">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b76a2-152">Пример</span><span class="sxs-lookup"><span data-stu-id="b76a2-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="b76a2-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="b76a2-153">Request</span></span>
<span data-ttu-id="b76a2-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b76a2-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b76a2-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="b76a2-155">Response</span></span>
<span data-ttu-id="b76a2-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b76a2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




