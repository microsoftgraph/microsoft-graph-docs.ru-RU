---
title: Обновление объекта deviceAndAppManagementRoleAssignment
description: Обновление свойств объекта deviceAndAppManagementRoleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a9848c5d0a9d545444d88f41c489f54d9ba2b502
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980158"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="550be-103">Обновление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="550be-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="550be-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="550be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="550be-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="550be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="550be-106">Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="550be-106">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="550be-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="550be-107">Prerequisites</span></span>
<span data-ttu-id="550be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="550be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="550be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="550be-110">Permission type</span></span>|<span data-ttu-id="550be-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="550be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="550be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="550be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="550be-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="550be-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="550be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="550be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="550be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="550be-115">Not supported.</span></span>|
|<span data-ttu-id="550be-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="550be-116">Application</span></span>|<span data-ttu-id="550be-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="550be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="550be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="550be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="550be-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="550be-119">Request headers</span></span>
|<span data-ttu-id="550be-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="550be-120">Header</span></span>|<span data-ttu-id="550be-121">Значение</span><span class="sxs-lookup"><span data-stu-id="550be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="550be-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="550be-122">Authorization</span></span>|<span data-ttu-id="550be-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="550be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="550be-124">Accept</span><span class="sxs-lookup"><span data-stu-id="550be-124">Accept</span></span>|<span data-ttu-id="550be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="550be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="550be-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="550be-126">Request body</span></span>
<span data-ttu-id="550be-127">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="550be-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="550be-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="550be-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="550be-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="550be-129">Property</span></span>|<span data-ttu-id="550be-130">Тип</span><span class="sxs-lookup"><span data-stu-id="550be-130">Type</span></span>|<span data-ttu-id="550be-131">Описание</span><span class="sxs-lookup"><span data-stu-id="550be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="550be-132">id</span><span class="sxs-lookup"><span data-stu-id="550be-132">id</span></span>|<span data-ttu-id="550be-133">String</span><span class="sxs-lookup"><span data-stu-id="550be-133">String</span></span>|<span data-ttu-id="550be-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="550be-134">Key of the entity.</span></span> <span data-ttu-id="550be-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="550be-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="550be-136">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="550be-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="550be-137">displayName</span><span class="sxs-lookup"><span data-stu-id="550be-137">displayName</span></span>|<span data-ttu-id="550be-138">Строка</span><span class="sxs-lookup"><span data-stu-id="550be-138">String</span></span>|<span data-ttu-id="550be-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="550be-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="550be-140">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="550be-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="550be-141">description</span><span class="sxs-lookup"><span data-stu-id="550be-141">description</span></span>|<span data-ttu-id="550be-142">String</span><span class="sxs-lookup"><span data-stu-id="550be-142">String</span></span>|<span data-ttu-id="550be-143">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="550be-143">Description of the Role Assignment.</span></span> <span data-ttu-id="550be-144">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="550be-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="550be-145">Скопемемберс</span><span class="sxs-lookup"><span data-stu-id="550be-145">scopeMembers</span></span>|<span data-ttu-id="550be-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="550be-146">String collection</span></span>|<span data-ttu-id="550be-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="550be-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="550be-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="550be-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="550be-149">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="550be-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="550be-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="550be-150">scopeType</span></span>|<span data-ttu-id="550be-151">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="550be-151">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="550be-152">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="550be-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="550be-153">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="550be-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="550be-154">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="550be-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="550be-155">Наследуется от [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="550be-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="550be-156">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="550be-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="550be-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="550be-157">resourceScopes</span></span>|<span data-ttu-id="550be-158">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="550be-158">String collection</span></span>|<span data-ttu-id="550be-159">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="550be-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="550be-160">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="550be-160">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="550be-161">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="550be-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="550be-162">members</span><span class="sxs-lookup"><span data-stu-id="550be-162">members</span></span>|<span data-ttu-id="550be-163">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="550be-163">String collection</span></span>|<span data-ttu-id="550be-164">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="550be-164">The list of ids of role member security groups.</span></span> <span data-ttu-id="550be-165">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="550be-165">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="550be-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="550be-166">Response</span></span>
<span data-ttu-id="550be-167">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="550be-167">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="550be-168">Пример</span><span class="sxs-lookup"><span data-stu-id="550be-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="550be-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="550be-169">Request</span></span>
<span data-ttu-id="550be-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="550be-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
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

### <a name="response"></a><span data-ttu-id="550be-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="550be-171">Response</span></span>
<span data-ttu-id="550be-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="550be-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





