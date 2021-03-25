---
title: Создание объекта deviceAndAppManagementRoleAssignment
description: Создание объекта deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30369e59547f169c010ba688e7b6655df7bc4847
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158558"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="fc002-103">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fc002-103">Create deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="fc002-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc002-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc002-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc002-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc002-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc002-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc002-107">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fc002-107">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc002-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fc002-108">Prerequisites</span></span>
<span data-ttu-id="fc002-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc002-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc002-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc002-111">Permission type</span></span>|<span data-ttu-id="fc002-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc002-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc002-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc002-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc002-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc002-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="fc002-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc002-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc002-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc002-116">Not supported.</span></span>|
|<span data-ttu-id="fc002-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fc002-117">Application</span></span>|<span data-ttu-id="fc002-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc002-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc002-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc002-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="fc002-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fc002-120">Request headers</span></span>
|<span data-ttu-id="fc002-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc002-121">Header</span></span>|<span data-ttu-id="fc002-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fc002-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc002-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc002-123">Authorization</span></span>|<span data-ttu-id="fc002-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc002-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc002-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fc002-125">Accept</span></span>|<span data-ttu-id="fc002-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc002-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc002-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc002-127">Request body</span></span>
<span data-ttu-id="fc002-128">В теле запроса добавьте представление объекта deviceAndAppManagementRoleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc002-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="fc002-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="fc002-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="fc002-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc002-130">Property</span></span>|<span data-ttu-id="fc002-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fc002-131">Type</span></span>|<span data-ttu-id="fc002-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fc002-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc002-133">id</span><span class="sxs-lookup"><span data-stu-id="fc002-133">id</span></span>|<span data-ttu-id="fc002-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fc002-134">String</span></span>|<span data-ttu-id="fc002-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc002-135">Key of the entity.</span></span> <span data-ttu-id="fc002-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="fc002-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="fc002-137">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fc002-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="fc002-138">displayName</span><span class="sxs-lookup"><span data-stu-id="fc002-138">displayName</span></span>|<span data-ttu-id="fc002-139">Строка</span><span class="sxs-lookup"><span data-stu-id="fc002-139">String</span></span>|<span data-ttu-id="fc002-140">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="fc002-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="fc002-141">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fc002-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="fc002-142">description</span><span class="sxs-lookup"><span data-stu-id="fc002-142">description</span></span>|<span data-ttu-id="fc002-143">Строка</span><span class="sxs-lookup"><span data-stu-id="fc002-143">String</span></span>|<span data-ttu-id="fc002-144">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="fc002-144">Description of the Role Assignment.</span></span> <span data-ttu-id="fc002-145">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fc002-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="fc002-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="fc002-146">scopeMembers</span></span>|<span data-ttu-id="fc002-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc002-147">String collection</span></span>|<span data-ttu-id="fc002-148">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="fc002-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fc002-149">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fc002-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="fc002-150">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fc002-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="fc002-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="fc002-151">scopeType</span></span>|<span data-ttu-id="fc002-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="fc002-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="fc002-153">Указывает тип области назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="fc002-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="fc002-154">По умолчанию тип "ResourceScope" позволяет назначение ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="fc002-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="fc002-155">Для "AllDevices", "AllLicensedUsers" и "AllDevicesAndLicensedUsers" свойство ResourceScopes следует оставить пустым.</span><span class="sxs-lookup"><span data-stu-id="fc002-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="fc002-156">Наследуется [от roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fc002-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="fc002-157">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="fc002-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="fc002-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="fc002-158">resourceScopes</span></span>|<span data-ttu-id="fc002-159">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc002-159">String collection</span></span>|<span data-ttu-id="fc002-160">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="fc002-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fc002-161">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fc002-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="fc002-162">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fc002-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="fc002-163">members</span><span class="sxs-lookup"><span data-stu-id="fc002-163">members</span></span>|<span data-ttu-id="fc002-164">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc002-164">String collection</span></span>|<span data-ttu-id="fc002-165">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="fc002-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="fc002-166">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fc002-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="fc002-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc002-167">Response</span></span>
<span data-ttu-id="fc002-168">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fc002-168">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc002-169">Пример</span><span class="sxs-lookup"><span data-stu-id="fc002-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc002-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc002-170">Request</span></span>
<span data-ttu-id="fc002-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc002-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fc002-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc002-172">Response</span></span>
<span data-ttu-id="fc002-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc002-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




