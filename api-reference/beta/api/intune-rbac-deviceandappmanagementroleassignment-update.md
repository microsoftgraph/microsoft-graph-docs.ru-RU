---
title: Обновление объекта deviceAndAppManagementRoleAssignment
description: Обновление свойств объекта deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20a1de5a901bb57f3bacf758de755ccb5177524e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43421334"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="f8529-103">Обновление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f8529-103">Update deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="f8529-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8529-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8529-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8529-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8529-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8529-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8529-107">Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f8529-107">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8529-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f8529-108">Prerequisites</span></span>
<span data-ttu-id="f8529-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8529-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8529-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8529-111">Permission type</span></span>|<span data-ttu-id="f8529-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8529-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8529-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8529-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8529-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8529-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f8529-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8529-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8529-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8529-116">Not supported.</span></span>|
|<span data-ttu-id="f8529-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f8529-117">Application</span></span>|<span data-ttu-id="f8529-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8529-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8529-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8529-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f8529-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f8529-120">Request headers</span></span>
|<span data-ttu-id="f8529-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8529-121">Header</span></span>|<span data-ttu-id="f8529-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f8529-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8529-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8529-123">Authorization</span></span>|<span data-ttu-id="f8529-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8529-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8529-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8529-125">Accept</span></span>|<span data-ttu-id="f8529-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8529-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8529-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8529-127">Request body</span></span>
<span data-ttu-id="f8529-128">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8529-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="f8529-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f8529-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="f8529-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8529-130">Property</span></span>|<span data-ttu-id="f8529-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f8529-131">Type</span></span>|<span data-ttu-id="f8529-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f8529-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8529-133">id</span><span class="sxs-lookup"><span data-stu-id="f8529-133">id</span></span>|<span data-ttu-id="f8529-134">String</span><span class="sxs-lookup"><span data-stu-id="f8529-134">String</span></span>|<span data-ttu-id="f8529-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f8529-135">Key of the entity.</span></span> <span data-ttu-id="f8529-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="f8529-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="f8529-137">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f8529-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f8529-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f8529-138">displayName</span></span>|<span data-ttu-id="f8529-139">Строка</span><span class="sxs-lookup"><span data-stu-id="f8529-139">String</span></span>|<span data-ttu-id="f8529-140">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="f8529-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="f8529-141">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f8529-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f8529-142">description</span><span class="sxs-lookup"><span data-stu-id="f8529-142">description</span></span>|<span data-ttu-id="f8529-143">String</span><span class="sxs-lookup"><span data-stu-id="f8529-143">String</span></span>|<span data-ttu-id="f8529-144">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="f8529-144">Description of the Role Assignment.</span></span> <span data-ttu-id="f8529-145">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f8529-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f8529-146">скопемемберс</span><span class="sxs-lookup"><span data-stu-id="f8529-146">scopeMembers</span></span>|<span data-ttu-id="f8529-147">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f8529-147">String collection</span></span>|<span data-ttu-id="f8529-148">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="f8529-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="f8529-149">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f8529-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="f8529-150">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f8529-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f8529-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="f8529-151">scopeType</span></span>|<span data-ttu-id="f8529-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="f8529-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="f8529-153">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="f8529-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="f8529-154">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="f8529-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="f8529-155">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="f8529-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="f8529-156">Наследуется от [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f8529-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="f8529-157">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="f8529-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="f8529-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="f8529-158">resourceScopes</span></span>|<span data-ttu-id="f8529-159">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f8529-159">String collection</span></span>|<span data-ttu-id="f8529-160">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="f8529-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="f8529-161">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f8529-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="f8529-162">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f8529-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f8529-163">members</span><span class="sxs-lookup"><span data-stu-id="f8529-163">members</span></span>|<span data-ttu-id="f8529-164">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f8529-164">String collection</span></span>|<span data-ttu-id="f8529-165">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="f8529-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="f8529-166">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f8529-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="f8529-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8529-167">Response</span></span>
<span data-ttu-id="f8529-168">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f8529-168">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8529-169">Пример</span><span class="sxs-lookup"><span data-stu-id="f8529-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8529-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8529-170">Request</span></span>
<span data-ttu-id="f8529-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8529-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8529-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8529-172">Response</span></span>
<span data-ttu-id="f8529-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8529-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



