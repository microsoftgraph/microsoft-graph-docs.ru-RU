---
title: Создание объекта deviceAndAppManagementRoleAssignment
description: Создание объекта deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8cf99e47d0dc42643e527ddb389f62dced191bae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452769"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="a31c3-103">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a31c3-103">Create deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="a31c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a31c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a31c3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a31c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a31c3-106">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a31c3-106">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a31c3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a31c3-107">Prerequisites</span></span>
<span data-ttu-id="a31c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a31c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a31c3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a31c3-110">Permission type</span></span>|<span data-ttu-id="a31c3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a31c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a31c3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a31c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a31c3-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a31c3-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a31c3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a31c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a31c3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a31c3-115">Not supported.</span></span>|
|<span data-ttu-id="a31c3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a31c3-116">Application</span></span>|<span data-ttu-id="a31c3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a31c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a31c3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a31c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a31c3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a31c3-119">Request headers</span></span>
|<span data-ttu-id="a31c3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a31c3-120">Header</span></span>|<span data-ttu-id="a31c3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a31c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a31c3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a31c3-122">Authorization</span></span>|<span data-ttu-id="a31c3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a31c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a31c3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a31c3-124">Accept</span></span>|<span data-ttu-id="a31c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a31c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a31c3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a31c3-126">Request body</span></span>
<span data-ttu-id="a31c3-127">В теле запроса добавьте представление объекта deviceAndAppManagementRoleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a31c3-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="a31c3-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="a31c3-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="a31c3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a31c3-129">Property</span></span>|<span data-ttu-id="a31c3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a31c3-130">Type</span></span>|<span data-ttu-id="a31c3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a31c3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a31c3-132">id</span><span class="sxs-lookup"><span data-stu-id="a31c3-132">id</span></span>|<span data-ttu-id="a31c3-133">String</span><span class="sxs-lookup"><span data-stu-id="a31c3-133">String</span></span>|<span data-ttu-id="a31c3-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a31c3-134">Key of the entity.</span></span> <span data-ttu-id="a31c3-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="a31c3-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="a31c3-136">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a31c3-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a31c3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a31c3-137">displayName</span></span>|<span data-ttu-id="a31c3-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a31c3-138">String</span></span>|<span data-ttu-id="a31c3-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="a31c3-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="a31c3-140">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a31c3-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a31c3-141">description</span><span class="sxs-lookup"><span data-stu-id="a31c3-141">description</span></span>|<span data-ttu-id="a31c3-142">String</span><span class="sxs-lookup"><span data-stu-id="a31c3-142">String</span></span>|<span data-ttu-id="a31c3-143">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="a31c3-143">Description of the Role Assignment.</span></span> <span data-ttu-id="a31c3-144">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a31c3-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a31c3-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="a31c3-145">resourceScopes</span></span>|<span data-ttu-id="a31c3-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a31c3-146">String collection</span></span>|<span data-ttu-id="a31c3-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="a31c3-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a31c3-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a31c3-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="a31c3-149">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a31c3-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="a31c3-150">members</span><span class="sxs-lookup"><span data-stu-id="a31c3-150">members</span></span>|<span data-ttu-id="a31c3-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a31c3-151">String collection</span></span>|<span data-ttu-id="a31c3-152">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="a31c3-152">The list of ids of role member security groups.</span></span> <span data-ttu-id="a31c3-153">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a31c3-153">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="a31c3-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="a31c3-154">Response</span></span>
<span data-ttu-id="a31c3-155">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a31c3-155">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a31c3-156">Пример</span><span class="sxs-lookup"><span data-stu-id="a31c3-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="a31c3-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="a31c3-157">Request</span></span>
<span data-ttu-id="a31c3-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a31c3-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a31c3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="a31c3-159">Response</span></span>
<span data-ttu-id="a31c3-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a31c3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






