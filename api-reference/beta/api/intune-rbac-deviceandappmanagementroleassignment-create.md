---
title: Создание объекта deviceAndAppManagementRoleAssignment
description: Создание объекта deviceAndAppManagementRoleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2030a2133b5776081a5a3d517daec9784363b03
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940744"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="14259-103">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="14259-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="14259-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14259-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14259-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14259-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14259-106">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="14259-106">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14259-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="14259-107">Prerequisites</span></span>
<span data-ttu-id="14259-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14259-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14259-110">Permission type</span></span>|<span data-ttu-id="14259-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14259-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14259-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14259-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14259-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14259-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="14259-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14259-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14259-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14259-115">Not supported.</span></span>|
|<span data-ttu-id="14259-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14259-116">Application</span></span>|<span data-ttu-id="14259-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14259-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14259-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14259-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="14259-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="14259-119">Request headers</span></span>
|<span data-ttu-id="14259-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14259-120">Header</span></span>|<span data-ttu-id="14259-121">Значение</span><span class="sxs-lookup"><span data-stu-id="14259-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14259-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14259-122">Authorization</span></span>|<span data-ttu-id="14259-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14259-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14259-124">Accept</span><span class="sxs-lookup"><span data-stu-id="14259-124">Accept</span></span>|<span data-ttu-id="14259-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14259-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14259-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14259-126">Request body</span></span>
<span data-ttu-id="14259-127">В теле запроса добавьте представление объекта deviceAndAppManagementRoleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14259-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="14259-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="14259-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="14259-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="14259-129">Property</span></span>|<span data-ttu-id="14259-130">Тип</span><span class="sxs-lookup"><span data-stu-id="14259-130">Type</span></span>|<span data-ttu-id="14259-131">Описание</span><span class="sxs-lookup"><span data-stu-id="14259-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14259-132">id</span><span class="sxs-lookup"><span data-stu-id="14259-132">id</span></span>|<span data-ttu-id="14259-133">String</span><span class="sxs-lookup"><span data-stu-id="14259-133">String</span></span>|<span data-ttu-id="14259-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="14259-134">Key of the entity.</span></span> <span data-ttu-id="14259-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="14259-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="14259-136">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="14259-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="14259-137">displayName</span><span class="sxs-lookup"><span data-stu-id="14259-137">displayName</span></span>|<span data-ttu-id="14259-138">Строка</span><span class="sxs-lookup"><span data-stu-id="14259-138">String</span></span>|<span data-ttu-id="14259-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="14259-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="14259-140">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="14259-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="14259-141">description</span><span class="sxs-lookup"><span data-stu-id="14259-141">description</span></span>|<span data-ttu-id="14259-142">String</span><span class="sxs-lookup"><span data-stu-id="14259-142">String</span></span>|<span data-ttu-id="14259-143">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="14259-143">Description of the Role Assignment.</span></span> <span data-ttu-id="14259-144">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="14259-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="14259-145">скопемемберс</span><span class="sxs-lookup"><span data-stu-id="14259-145">scopeMembers</span></span>|<span data-ttu-id="14259-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="14259-146">String collection</span></span>|<span data-ttu-id="14259-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="14259-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="14259-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="14259-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="14259-149">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="14259-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="14259-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="14259-150">scopeType</span></span>|<span data-ttu-id="14259-151">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="14259-151">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="14259-152">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="14259-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="14259-153">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="14259-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="14259-154">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="14259-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="14259-155">Наследуется от [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="14259-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="14259-156">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="14259-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="14259-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="14259-157">resourceScopes</span></span>|<span data-ttu-id="14259-158">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="14259-158">String collection</span></span>|<span data-ttu-id="14259-159">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="14259-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="14259-160">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="14259-160">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="14259-161">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="14259-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="14259-162">members</span><span class="sxs-lookup"><span data-stu-id="14259-162">members</span></span>|<span data-ttu-id="14259-163">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="14259-163">String collection</span></span>|<span data-ttu-id="14259-164">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="14259-164">The list of ids of role member security groups.</span></span> <span data-ttu-id="14259-165">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="14259-165">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="14259-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="14259-166">Response</span></span>
<span data-ttu-id="14259-167">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="14259-167">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14259-168">Пример</span><span class="sxs-lookup"><span data-stu-id="14259-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="14259-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="14259-169">Request</span></span>
<span data-ttu-id="14259-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14259-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="14259-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="14259-171">Response</span></span>
<span data-ttu-id="14259-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14259-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```





