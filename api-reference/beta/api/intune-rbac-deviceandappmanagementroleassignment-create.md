---
title: Создание объекта deviceAndAppManagementRoleAssignment
description: Создание объекта deviceAndAppManagementRoleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 689221b6f965668d76e23176d78c6439ef74e17f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460019"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="bcc9b-103">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bcc9b-103">Create deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="bcc9b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bcc9b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bcc9b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcc9b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcc9b-107">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bcc9b-107">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcc9b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bcc9b-108">Prerequisites</span></span>
<span data-ttu-id="bcc9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcc9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcc9b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcc9b-111">Permission type</span></span>|<span data-ttu-id="bcc9b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcc9b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcc9b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcc9b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bcc9b-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcc9b-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="bcc9b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcc9b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcc9b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-116">Not supported.</span></span>|
|<span data-ttu-id="bcc9b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcc9b-117">Application</span></span>|<span data-ttu-id="bcc9b-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcc9b-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcc9b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcc9b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="bcc9b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bcc9b-120">Request headers</span></span>
|<span data-ttu-id="bcc9b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcc9b-121">Header</span></span>|<span data-ttu-id="bcc9b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bcc9b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcc9b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcc9b-123">Authorization</span></span>|<span data-ttu-id="bcc9b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcc9b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bcc9b-125">Accept</span></span>|<span data-ttu-id="bcc9b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bcc9b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcc9b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcc9b-127">Request body</span></span>
<span data-ttu-id="bcc9b-128">В теле запроса добавьте представление объекта deviceAndAppManagementRoleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="bcc9b-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="bcc9b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcc9b-130">Property</span></span>|<span data-ttu-id="bcc9b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bcc9b-131">Type</span></span>|<span data-ttu-id="bcc9b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bcc9b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcc9b-133">id</span><span class="sxs-lookup"><span data-stu-id="bcc9b-133">id</span></span>|<span data-ttu-id="bcc9b-134">String</span><span class="sxs-lookup"><span data-stu-id="bcc9b-134">String</span></span>|<span data-ttu-id="bcc9b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-135">Key of the entity.</span></span> <span data-ttu-id="bcc9b-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="bcc9b-137">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bcc9b-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="bcc9b-138">displayName</span><span class="sxs-lookup"><span data-stu-id="bcc9b-138">displayName</span></span>|<span data-ttu-id="bcc9b-139">Строка</span><span class="sxs-lookup"><span data-stu-id="bcc9b-139">String</span></span>|<span data-ttu-id="bcc9b-140">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="bcc9b-141">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bcc9b-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="bcc9b-142">description</span><span class="sxs-lookup"><span data-stu-id="bcc9b-142">description</span></span>|<span data-ttu-id="bcc9b-143">String</span><span class="sxs-lookup"><span data-stu-id="bcc9b-143">String</span></span>|<span data-ttu-id="bcc9b-144">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-144">Description of the Role Assignment.</span></span> <span data-ttu-id="bcc9b-145">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bcc9b-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="bcc9b-146">скопемемберс</span><span class="sxs-lookup"><span data-stu-id="bcc9b-146">scopeMembers</span></span>|<span data-ttu-id="bcc9b-147">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bcc9b-147">String collection</span></span>|<span data-ttu-id="bcc9b-148">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="bcc9b-149">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="bcc9b-150">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bcc9b-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="bcc9b-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="bcc9b-151">scopeType</span></span>|<span data-ttu-id="bcc9b-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="bcc9b-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="bcc9b-153">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="bcc9b-154">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="bcc9b-155">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="bcc9b-156">Наследуется от [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bcc9b-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="bcc9b-157">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="bcc9b-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="bcc9b-158">resourceScopes</span></span>|<span data-ttu-id="bcc9b-159">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bcc9b-159">String collection</span></span>|<span data-ttu-id="bcc9b-160">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="bcc9b-161">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="bcc9b-162">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bcc9b-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="bcc9b-163">members</span><span class="sxs-lookup"><span data-stu-id="bcc9b-163">members</span></span>|<span data-ttu-id="bcc9b-164">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bcc9b-164">String collection</span></span>|<span data-ttu-id="bcc9b-165">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="bcc9b-166">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="bcc9b-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc9b-167">Response</span></span>
<span data-ttu-id="bcc9b-168">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-168">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcc9b-169">Пример</span><span class="sxs-lookup"><span data-stu-id="bcc9b-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcc9b-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcc9b-170">Request</span></span>
<span data-ttu-id="bcc9b-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bcc9b-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc9b-172">Response</span></span>
<span data-ttu-id="bcc9b-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcc9b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





