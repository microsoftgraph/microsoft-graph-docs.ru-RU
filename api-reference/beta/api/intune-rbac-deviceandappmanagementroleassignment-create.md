---
title: Создание объекта deviceAndAppManagementRoleAssignment
description: Создание объекта deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e727838390900e065d23eb1b774f7170fafdf5b6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709133"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="49328-103">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="49328-103">Create deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="49328-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49328-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49328-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49328-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49328-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49328-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49328-107">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="49328-107">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49328-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="49328-108">Prerequisites</span></span>
<span data-ttu-id="49328-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49328-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49328-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49328-111">Permission type</span></span>|<span data-ttu-id="49328-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49328-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49328-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49328-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49328-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49328-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="49328-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49328-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49328-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49328-116">Not supported.</span></span>|
|<span data-ttu-id="49328-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49328-117">Application</span></span>|<span data-ttu-id="49328-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49328-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49328-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49328-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="49328-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="49328-120">Request headers</span></span>
|<span data-ttu-id="49328-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49328-121">Header</span></span>|<span data-ttu-id="49328-122">Значение</span><span class="sxs-lookup"><span data-stu-id="49328-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49328-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49328-123">Authorization</span></span>|<span data-ttu-id="49328-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49328-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49328-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49328-125">Accept</span></span>|<span data-ttu-id="49328-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49328-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49328-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49328-127">Request body</span></span>
<span data-ttu-id="49328-128">В теле запроса добавьте представление объекта deviceAndAppManagementRoleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49328-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="49328-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="49328-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="49328-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="49328-130">Property</span></span>|<span data-ttu-id="49328-131">Тип</span><span class="sxs-lookup"><span data-stu-id="49328-131">Type</span></span>|<span data-ttu-id="49328-132">Описание</span><span class="sxs-lookup"><span data-stu-id="49328-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49328-133">id</span><span class="sxs-lookup"><span data-stu-id="49328-133">id</span></span>|<span data-ttu-id="49328-134">Строка</span><span class="sxs-lookup"><span data-stu-id="49328-134">String</span></span>|<span data-ttu-id="49328-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="49328-135">Key of the entity.</span></span> <span data-ttu-id="49328-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="49328-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="49328-137">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="49328-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="49328-138">displayName</span><span class="sxs-lookup"><span data-stu-id="49328-138">displayName</span></span>|<span data-ttu-id="49328-139">Строка</span><span class="sxs-lookup"><span data-stu-id="49328-139">String</span></span>|<span data-ttu-id="49328-140">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="49328-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="49328-141">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="49328-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="49328-142">description</span><span class="sxs-lookup"><span data-stu-id="49328-142">description</span></span>|<span data-ttu-id="49328-143">Строка</span><span class="sxs-lookup"><span data-stu-id="49328-143">String</span></span>|<span data-ttu-id="49328-144">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="49328-144">Description of the Role Assignment.</span></span> <span data-ttu-id="49328-145">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="49328-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="49328-146">скопемемберс</span><span class="sxs-lookup"><span data-stu-id="49328-146">scopeMembers</span></span>|<span data-ttu-id="49328-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="49328-147">String collection</span></span>|<span data-ttu-id="49328-148">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="49328-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="49328-149">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="49328-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="49328-150">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="49328-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="49328-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="49328-151">scopeType</span></span>|<span data-ttu-id="49328-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="49328-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="49328-153">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="49328-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="49328-154">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="49328-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="49328-155">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="49328-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="49328-156">Наследуется от [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="49328-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="49328-157">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="49328-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="49328-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="49328-158">resourceScopes</span></span>|<span data-ttu-id="49328-159">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="49328-159">String collection</span></span>|<span data-ttu-id="49328-160">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="49328-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="49328-161">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="49328-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="49328-162">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="49328-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="49328-163">members</span><span class="sxs-lookup"><span data-stu-id="49328-163">members</span></span>|<span data-ttu-id="49328-164">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="49328-164">String collection</span></span>|<span data-ttu-id="49328-165">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="49328-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="49328-166">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="49328-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="49328-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="49328-167">Response</span></span>
<span data-ttu-id="49328-168">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="49328-168">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49328-169">Пример</span><span class="sxs-lookup"><span data-stu-id="49328-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="49328-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="49328-170">Request</span></span>
<span data-ttu-id="49328-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49328-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="49328-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="49328-172">Response</span></span>
<span data-ttu-id="49328-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49328-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





