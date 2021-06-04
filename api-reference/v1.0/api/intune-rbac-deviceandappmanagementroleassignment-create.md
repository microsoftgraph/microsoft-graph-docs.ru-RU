---
title: Создание объекта deviceAndAppManagementRoleAssignment
description: Создание объекта deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a0d573e2636868ee6a37e96297e096a80c3a2fa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52743226"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="89ad5-103">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="89ad5-103">Create deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="89ad5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89ad5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89ad5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89ad5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89ad5-106">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="89ad5-106">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89ad5-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="89ad5-107">Prerequisites</span></span>
<span data-ttu-id="89ad5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89ad5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ad5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89ad5-110">Permission type</span></span>|<span data-ttu-id="89ad5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89ad5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89ad5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89ad5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89ad5-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ad5-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="89ad5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89ad5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89ad5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89ad5-115">Not supported.</span></span>|
|<span data-ttu-id="89ad5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="89ad5-116">Application</span></span>|<span data-ttu-id="89ad5-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ad5-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89ad5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89ad5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="89ad5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="89ad5-119">Request headers</span></span>
|<span data-ttu-id="89ad5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89ad5-120">Header</span></span>|<span data-ttu-id="89ad5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="89ad5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89ad5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89ad5-122">Authorization</span></span>|<span data-ttu-id="89ad5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89ad5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89ad5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="89ad5-124">Accept</span></span>|<span data-ttu-id="89ad5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89ad5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89ad5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89ad5-126">Request body</span></span>
<span data-ttu-id="89ad5-127">В теле запроса добавьте представление объекта deviceAndAppManagementRoleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89ad5-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="89ad5-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="89ad5-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="89ad5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="89ad5-129">Property</span></span>|<span data-ttu-id="89ad5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="89ad5-130">Type</span></span>|<span data-ttu-id="89ad5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="89ad5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89ad5-132">id</span><span class="sxs-lookup"><span data-stu-id="89ad5-132">id</span></span>|<span data-ttu-id="89ad5-133">String</span><span class="sxs-lookup"><span data-stu-id="89ad5-133">String</span></span>|<span data-ttu-id="89ad5-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="89ad5-134">Key of the entity.</span></span> <span data-ttu-id="89ad5-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="89ad5-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="89ad5-136">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="89ad5-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="89ad5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="89ad5-137">displayName</span></span>|<span data-ttu-id="89ad5-138">String</span><span class="sxs-lookup"><span data-stu-id="89ad5-138">String</span></span>|<span data-ttu-id="89ad5-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="89ad5-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="89ad5-140">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="89ad5-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="89ad5-141">description</span><span class="sxs-lookup"><span data-stu-id="89ad5-141">description</span></span>|<span data-ttu-id="89ad5-142">String</span><span class="sxs-lookup"><span data-stu-id="89ad5-142">String</span></span>|<span data-ttu-id="89ad5-143">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="89ad5-143">Description of the Role Assignment.</span></span> <span data-ttu-id="89ad5-144">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="89ad5-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="89ad5-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="89ad5-145">resourceScopes</span></span>|<span data-ttu-id="89ad5-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="89ad5-146">String collection</span></span>|<span data-ttu-id="89ad5-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="89ad5-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="89ad5-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="89ad5-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="89ad5-149">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="89ad5-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="89ad5-150">members</span><span class="sxs-lookup"><span data-stu-id="89ad5-150">members</span></span>|<span data-ttu-id="89ad5-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="89ad5-151">String collection</span></span>|<span data-ttu-id="89ad5-152">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="89ad5-152">The list of ids of role member security groups.</span></span> <span data-ttu-id="89ad5-153">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="89ad5-153">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="89ad5-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="89ad5-154">Response</span></span>
<span data-ttu-id="89ad5-155">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="89ad5-155">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89ad5-156">Пример</span><span class="sxs-lookup"><span data-stu-id="89ad5-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="89ad5-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="89ad5-157">Request</span></span>
<span data-ttu-id="89ad5-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89ad5-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
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

### <a name="response"></a><span data-ttu-id="89ad5-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="89ad5-159">Response</span></span>
<span data-ttu-id="89ad5-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89ad5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




