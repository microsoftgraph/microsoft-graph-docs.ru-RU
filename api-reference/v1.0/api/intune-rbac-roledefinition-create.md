---
title: Создание roleDefinition
description: Создание объекта roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 27dc878346645c5b7d2e35ebc7fc468afa043a7c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966750"
---
# <a name="create-roledefinition"></a><span data-ttu-id="ed91d-103">Создание roleDefinition</span><span class="sxs-lookup"><span data-stu-id="ed91d-103">Create roleDefinition</span></span>

> <span data-ttu-id="ed91d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed91d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed91d-105">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ed91d-105">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed91d-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ed91d-106">Prerequisites</span></span>
<span data-ttu-id="ed91d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed91d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed91d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed91d-109">Permission type</span></span>|<span data-ttu-id="ed91d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed91d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed91d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed91d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed91d-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed91d-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ed91d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed91d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed91d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed91d-114">Not supported.</span></span>|
|<span data-ttu-id="ed91d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed91d-115">Application</span></span>|<span data-ttu-id="ed91d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed91d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed91d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed91d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ed91d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed91d-118">Request headers</span></span>
|<span data-ttu-id="ed91d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed91d-119">Header</span></span>|<span data-ttu-id="ed91d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ed91d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed91d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed91d-121">Authorization</span></span>|<span data-ttu-id="ed91d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ed91d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed91d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ed91d-123">Accept</span></span>|<span data-ttu-id="ed91d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ed91d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed91d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed91d-125">Request body</span></span>
<span data-ttu-id="ed91d-126">В теле запроса добавьте представление объекта roleDefinition в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed91d-126">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="ed91d-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="ed91d-127">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="ed91d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed91d-128">Property</span></span>|<span data-ttu-id="ed91d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ed91d-129">Type</span></span>|<span data-ttu-id="ed91d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ed91d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed91d-131">id</span><span class="sxs-lookup"><span data-stu-id="ed91d-131">id</span></span>|<span data-ttu-id="ed91d-132">String</span><span class="sxs-lookup"><span data-stu-id="ed91d-132">String</span></span>|<span data-ttu-id="ed91d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ed91d-133">Key of the entity.</span></span> <span data-ttu-id="ed91d-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="ed91d-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="ed91d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ed91d-135">displayName</span></span>|<span data-ttu-id="ed91d-136">String</span><span class="sxs-lookup"><span data-stu-id="ed91d-136">String</span></span>|<span data-ttu-id="ed91d-137">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="ed91d-137">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="ed91d-138">описание</span><span class="sxs-lookup"><span data-stu-id="ed91d-138">description</span></span>|<span data-ttu-id="ed91d-139">String</span><span class="sxs-lookup"><span data-stu-id="ed91d-139">String</span></span>|<span data-ttu-id="ed91d-140">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="ed91d-140">Description of the Role definition.</span></span>|
|<span data-ttu-id="ed91d-141">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ed91d-141">rolePermissions</span></span>|<span data-ttu-id="ed91d-142">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ed91d-142">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ed91d-143">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="ed91d-143">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ed91d-144">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="ed91d-144">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="ed91d-145">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ed91d-145">isBuiltIn</span></span>|<span data-ttu-id="ed91d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed91d-146">Boolean</span></span>|<span data-ttu-id="ed91d-147">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="ed91d-147">Type of Role.</span></span> <span data-ttu-id="ed91d-148">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="ed91d-148">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="ed91d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed91d-149">Response</span></span>
<span data-ttu-id="ed91d-150">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ed91d-150">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed91d-151">Пример</span><span class="sxs-lookup"><span data-stu-id="ed91d-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed91d-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed91d-152">Request</span></span>
<span data-ttu-id="ed91d-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed91d-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ed91d-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed91d-154">Response</span></span>
<span data-ttu-id="ed91d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ed91d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



