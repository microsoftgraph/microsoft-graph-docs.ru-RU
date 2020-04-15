---
title: Обновление объекта deviceAndAppManagementRoleAssignment
description: Обновление свойств объекта deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d4e2c97a9217e011e357e87e6f1e45bbe0cefa2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452725"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="b17f4-103">Обновление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b17f4-103">Update deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="b17f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b17f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b17f4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b17f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b17f4-106">Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b17f4-106">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b17f4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b17f4-107">Prerequisites</span></span>
<span data-ttu-id="b17f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b17f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b17f4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b17f4-110">Permission type</span></span>|<span data-ttu-id="b17f4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b17f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b17f4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b17f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b17f4-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b17f4-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b17f4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b17f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b17f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b17f4-115">Not supported.</span></span>|
|<span data-ttu-id="b17f4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b17f4-116">Application</span></span>|<span data-ttu-id="b17f4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b17f4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b17f4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b17f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b17f4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b17f4-119">Request headers</span></span>
|<span data-ttu-id="b17f4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b17f4-120">Header</span></span>|<span data-ttu-id="b17f4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b17f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b17f4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b17f4-122">Authorization</span></span>|<span data-ttu-id="b17f4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b17f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b17f4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b17f4-124">Accept</span></span>|<span data-ttu-id="b17f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b17f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b17f4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b17f4-126">Request body</span></span>
<span data-ttu-id="b17f4-127">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b17f4-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="b17f4-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b17f4-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="b17f4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b17f4-129">Property</span></span>|<span data-ttu-id="b17f4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b17f4-130">Type</span></span>|<span data-ttu-id="b17f4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b17f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b17f4-132">id</span><span class="sxs-lookup"><span data-stu-id="b17f4-132">id</span></span>|<span data-ttu-id="b17f4-133">String</span><span class="sxs-lookup"><span data-stu-id="b17f4-133">String</span></span>|<span data-ttu-id="b17f4-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b17f4-134">Key of the entity.</span></span> <span data-ttu-id="b17f4-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="b17f4-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="b17f4-136">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b17f4-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b17f4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b17f4-137">displayName</span></span>|<span data-ttu-id="b17f4-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b17f4-138">String</span></span>|<span data-ttu-id="b17f4-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b17f4-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="b17f4-140">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b17f4-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b17f4-141">description</span><span class="sxs-lookup"><span data-stu-id="b17f4-141">description</span></span>|<span data-ttu-id="b17f4-142">String</span><span class="sxs-lookup"><span data-stu-id="b17f4-142">String</span></span>|<span data-ttu-id="b17f4-143">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b17f4-143">Description of the Role Assignment.</span></span> <span data-ttu-id="b17f4-144">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b17f4-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b17f4-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b17f4-145">resourceScopes</span></span>|<span data-ttu-id="b17f4-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b17f4-146">String collection</span></span>|<span data-ttu-id="b17f4-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="b17f4-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b17f4-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b17f4-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="b17f4-149">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b17f4-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b17f4-150">members</span><span class="sxs-lookup"><span data-stu-id="b17f4-150">members</span></span>|<span data-ttu-id="b17f4-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b17f4-151">String collection</span></span>|<span data-ttu-id="b17f4-152">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="b17f4-152">The list of ids of role member security groups.</span></span> <span data-ttu-id="b17f4-153">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b17f4-153">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b17f4-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="b17f4-154">Response</span></span>
<span data-ttu-id="b17f4-155">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b17f4-155">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b17f4-156">Пример</span><span class="sxs-lookup"><span data-stu-id="b17f4-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="b17f4-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="b17f4-157">Request</span></span>
<span data-ttu-id="b17f4-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b17f4-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b17f4-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b17f4-159">Response</span></span>
<span data-ttu-id="b17f4-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b17f4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```






