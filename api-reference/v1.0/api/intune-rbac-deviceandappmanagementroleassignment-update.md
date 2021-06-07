---
title: Обновление объекта deviceAndAppManagementRoleAssignment
description: Обновление свойств объекта deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff303a083124b5a22ef1fc594ea824d7f5e82391
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754778"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="9f472-103">Обновление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9f472-103">Update deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="9f472-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f472-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f472-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f472-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f472-106">Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f472-106">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f472-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9f472-107">Prerequisites</span></span>
<span data-ttu-id="9f472-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f472-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f472-110">Permission type</span></span>|<span data-ttu-id="9f472-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f472-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f472-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f472-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f472-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f472-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="9f472-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f472-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f472-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f472-115">Not supported.</span></span>|
|<span data-ttu-id="9f472-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f472-116">Application</span></span>|<span data-ttu-id="9f472-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f472-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f472-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f472-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9f472-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f472-119">Request headers</span></span>
|<span data-ttu-id="9f472-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f472-120">Header</span></span>|<span data-ttu-id="9f472-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9f472-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f472-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f472-122">Authorization</span></span>|<span data-ttu-id="9f472-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f472-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f472-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9f472-124">Accept</span></span>|<span data-ttu-id="9f472-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f472-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f472-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f472-126">Request body</span></span>
<span data-ttu-id="9f472-127">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f472-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="9f472-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f472-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="9f472-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f472-129">Property</span></span>|<span data-ttu-id="9f472-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9f472-130">Type</span></span>|<span data-ttu-id="9f472-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9f472-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f472-132">id</span><span class="sxs-lookup"><span data-stu-id="9f472-132">id</span></span>|<span data-ttu-id="9f472-133">String</span><span class="sxs-lookup"><span data-stu-id="9f472-133">String</span></span>|<span data-ttu-id="9f472-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f472-134">Key of the entity.</span></span> <span data-ttu-id="9f472-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="9f472-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="9f472-136">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f472-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9f472-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9f472-137">displayName</span></span>|<span data-ttu-id="9f472-138">String</span><span class="sxs-lookup"><span data-stu-id="9f472-138">String</span></span>|<span data-ttu-id="9f472-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="9f472-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="9f472-140">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f472-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9f472-141">description</span><span class="sxs-lookup"><span data-stu-id="9f472-141">description</span></span>|<span data-ttu-id="9f472-142">String</span><span class="sxs-lookup"><span data-stu-id="9f472-142">String</span></span>|<span data-ttu-id="9f472-143">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="9f472-143">Description of the Role Assignment.</span></span> <span data-ttu-id="9f472-144">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f472-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9f472-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="9f472-145">resourceScopes</span></span>|<span data-ttu-id="9f472-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9f472-146">String collection</span></span>|<span data-ttu-id="9f472-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="9f472-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="9f472-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9f472-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="9f472-149">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f472-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="9f472-150">members</span><span class="sxs-lookup"><span data-stu-id="9f472-150">members</span></span>|<span data-ttu-id="9f472-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9f472-151">String collection</span></span>|<span data-ttu-id="9f472-152">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="9f472-152">The list of ids of role member security groups.</span></span> <span data-ttu-id="9f472-153">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9f472-153">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="9f472-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f472-154">Response</span></span>
<span data-ttu-id="9f472-155">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9f472-155">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f472-156">Пример</span><span class="sxs-lookup"><span data-stu-id="9f472-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f472-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f472-157">Request</span></span>
<span data-ttu-id="9f472-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f472-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f472-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f472-159">Response</span></span>
<span data-ttu-id="9f472-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f472-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




