---
title: Создание объекта deviceAndAppManagementRoleAssignment
description: Создание объекта deviceAndAppManagementRoleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: defac24202a66fff7980d4bb383ecdce38e9d823
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512358"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="7cb80-103">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7cb80-103">Create deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="7cb80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cb80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7cb80-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7cb80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cb80-106">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7cb80-106">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cb80-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7cb80-107">Prerequisites</span></span>
<span data-ttu-id="7cb80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cb80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cb80-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cb80-110">Permission type</span></span>|<span data-ttu-id="7cb80-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cb80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cb80-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cb80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7cb80-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cb80-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="7cb80-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cb80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cb80-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cb80-115">Not supported.</span></span>|
|<span data-ttu-id="7cb80-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cb80-116">Application</span></span>|<span data-ttu-id="7cb80-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cb80-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cb80-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cb80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="7cb80-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7cb80-119">Request headers</span></span>
|<span data-ttu-id="7cb80-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7cb80-120">Header</span></span>|<span data-ttu-id="7cb80-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7cb80-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cb80-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cb80-122">Authorization</span></span>|<span data-ttu-id="7cb80-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cb80-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cb80-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7cb80-124">Accept</span></span>|<span data-ttu-id="7cb80-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7cb80-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cb80-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cb80-126">Request body</span></span>
<span data-ttu-id="7cb80-127">В теле запроса добавьте представление объекта deviceAndAppManagementRoleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cb80-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="7cb80-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="7cb80-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="7cb80-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cb80-129">Property</span></span>|<span data-ttu-id="7cb80-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7cb80-130">Type</span></span>|<span data-ttu-id="7cb80-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7cb80-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cb80-132">id</span><span class="sxs-lookup"><span data-stu-id="7cb80-132">id</span></span>|<span data-ttu-id="7cb80-133">String</span><span class="sxs-lookup"><span data-stu-id="7cb80-133">String</span></span>|<span data-ttu-id="7cb80-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7cb80-134">Key of the entity.</span></span> <span data-ttu-id="7cb80-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="7cb80-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="7cb80-136">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7cb80-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="7cb80-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7cb80-137">displayName</span></span>|<span data-ttu-id="7cb80-138">Строка</span><span class="sxs-lookup"><span data-stu-id="7cb80-138">String</span></span>|<span data-ttu-id="7cb80-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="7cb80-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="7cb80-140">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7cb80-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="7cb80-141">description</span><span class="sxs-lookup"><span data-stu-id="7cb80-141">description</span></span>|<span data-ttu-id="7cb80-142">String</span><span class="sxs-lookup"><span data-stu-id="7cb80-142">String</span></span>|<span data-ttu-id="7cb80-143">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="7cb80-143">Description of the Role Assignment.</span></span> <span data-ttu-id="7cb80-144">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7cb80-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="7cb80-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="7cb80-145">resourceScopes</span></span>|<span data-ttu-id="7cb80-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7cb80-146">String collection</span></span>|<span data-ttu-id="7cb80-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="7cb80-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="7cb80-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7cb80-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="7cb80-149">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7cb80-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="7cb80-150">members</span><span class="sxs-lookup"><span data-stu-id="7cb80-150">members</span></span>|<span data-ttu-id="7cb80-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7cb80-151">String collection</span></span>|<span data-ttu-id="7cb80-152">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="7cb80-152">The list of ids of role member security groups.</span></span> <span data-ttu-id="7cb80-153">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7cb80-153">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="7cb80-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cb80-154">Response</span></span>
<span data-ttu-id="7cb80-155">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7cb80-155">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cb80-156">Пример</span><span class="sxs-lookup"><span data-stu-id="7cb80-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cb80-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cb80-157">Request</span></span>
<span data-ttu-id="7cb80-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cb80-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7cb80-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cb80-159">Response</span></span>
<span data-ttu-id="7cb80-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7cb80-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




