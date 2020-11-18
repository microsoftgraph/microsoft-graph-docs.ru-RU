---
title: Обновление объекта targetedManagedAppPolicyAssignment
description: Обновление свойств объекта targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aae14ce7703fb4d97f1077978cd99014b0905e11
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49200815"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="58bf9-103">Обновление объекта targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="58bf9-103">Update targetedManagedAppPolicyAssignment</span></span>

<span data-ttu-id="58bf9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58bf9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58bf9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58bf9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58bf9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58bf9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58bf9-107">Обновление свойств объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="58bf9-107">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58bf9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="58bf9-108">Prerequisites</span></span>
<span data-ttu-id="58bf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58bf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58bf9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58bf9-111">Permission type</span></span>|<span data-ttu-id="58bf9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58bf9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58bf9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58bf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58bf9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bf9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="58bf9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58bf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58bf9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58bf9-116">Not supported.</span></span>|
|<span data-ttu-id="58bf9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="58bf9-117">Application</span></span>|<span data-ttu-id="58bf9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bf9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58bf9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58bf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="58bf9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58bf9-120">Request headers</span></span>
|<span data-ttu-id="58bf9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58bf9-121">Header</span></span>|<span data-ttu-id="58bf9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="58bf9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58bf9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58bf9-123">Authorization</span></span>|<span data-ttu-id="58bf9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58bf9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58bf9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58bf9-125">Accept</span></span>|<span data-ttu-id="58bf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58bf9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58bf9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58bf9-127">Request body</span></span>
<span data-ttu-id="58bf9-128">В теле запроса добавьте представление объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58bf9-128">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="58bf9-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="58bf9-129">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="58bf9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="58bf9-130">Property</span></span>|<span data-ttu-id="58bf9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="58bf9-131">Type</span></span>|<span data-ttu-id="58bf9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="58bf9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58bf9-133">id</span><span class="sxs-lookup"><span data-stu-id="58bf9-133">id</span></span>|<span data-ttu-id="58bf9-134">String</span><span class="sxs-lookup"><span data-stu-id="58bf9-134">String</span></span>|<span data-ttu-id="58bf9-135">Id</span><span class="sxs-lookup"><span data-stu-id="58bf9-135">Id</span></span>|
|<span data-ttu-id="58bf9-136">target</span><span class="sxs-lookup"><span data-stu-id="58bf9-136">target</span></span>|[<span data-ttu-id="58bf9-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="58bf9-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="58bf9-138">Идентификатор для развертывания в группе или приложении</span><span class="sxs-lookup"><span data-stu-id="58bf9-138">Identifier for deployment to a group or app</span></span>|
|<span data-ttu-id="58bf9-139">source</span><span class="sxs-lookup"><span data-stu-id="58bf9-139">source</span></span>|[<span data-ttu-id="58bf9-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="58bf9-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="58bf9-141">Тип ресурса, используемого для развертывания в группу, Direct или в упаковке/набор политик.</span><span class="sxs-lookup"><span data-stu-id="58bf9-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="58bf9-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="58bf9-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="58bf9-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="58bf9-143">sourceId</span></span>|<span data-ttu-id="58bf9-144">String</span><span class="sxs-lookup"><span data-stu-id="58bf9-144">String</span></span>|<span data-ttu-id="58bf9-145">Идентификатор ресурса, используемого для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="58bf9-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="58bf9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="58bf9-146">Response</span></span>
<span data-ttu-id="58bf9-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="58bf9-147">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58bf9-148">Пример</span><span class="sxs-lookup"><span data-stu-id="58bf9-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="58bf9-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="58bf9-149">Request</span></span>
<span data-ttu-id="58bf9-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58bf9-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 390

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="58bf9-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="58bf9-151">Response</span></span>
<span data-ttu-id="58bf9-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58bf9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




