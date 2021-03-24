---
title: Обновление объекта deviceConfigurationAssignment
description: Обновление свойств объекта deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 90f7edb2556c6f35edecc115d7056a4f7bdb2c48
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131752"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="072c7-103">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="072c7-103">Update deviceConfigurationAssignment</span></span>

<span data-ttu-id="072c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="072c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="072c7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="072c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="072c7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="072c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="072c7-107">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="072c7-107">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="072c7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="072c7-108">Prerequisites</span></span>
<span data-ttu-id="072c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="072c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="072c7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="072c7-111">Permission type</span></span>|<span data-ttu-id="072c7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="072c7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="072c7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="072c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="072c7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="072c7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="072c7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="072c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="072c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="072c7-116">Not supported.</span></span>|
|<span data-ttu-id="072c7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="072c7-117">Application</span></span>|<span data-ttu-id="072c7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="072c7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="072c7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="072c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="072c7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="072c7-120">Request headers</span></span>
|<span data-ttu-id="072c7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="072c7-121">Header</span></span>|<span data-ttu-id="072c7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="072c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="072c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="072c7-123">Authorization</span></span>|<span data-ttu-id="072c7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="072c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="072c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="072c7-125">Accept</span></span>|<span data-ttu-id="072c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="072c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="072c7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="072c7-127">Request body</span></span>
<span data-ttu-id="072c7-128">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="072c7-128">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="072c7-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="072c7-129">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="072c7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="072c7-130">Property</span></span>|<span data-ttu-id="072c7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="072c7-131">Type</span></span>|<span data-ttu-id="072c7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="072c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="072c7-133">id</span><span class="sxs-lookup"><span data-stu-id="072c7-133">id</span></span>|<span data-ttu-id="072c7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="072c7-134">String</span></span>|<span data-ttu-id="072c7-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="072c7-135">The key of the assignment.</span></span>|
|<span data-ttu-id="072c7-136">target</span><span class="sxs-lookup"><span data-stu-id="072c7-136">target</span></span>|[<span data-ttu-id="072c7-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="072c7-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="072c7-138">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="072c7-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="072c7-139">source</span><span class="sxs-lookup"><span data-stu-id="072c7-139">source</span></span>|[<span data-ttu-id="072c7-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="072c7-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="072c7-141">Источник назначения для конфигурации устройства, прямой или пакетной или политикиSet.</span><span class="sxs-lookup"><span data-stu-id="072c7-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="072c7-142">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="072c7-142">This property is read-only.</span></span> <span data-ttu-id="072c7-143">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="072c7-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="072c7-144">sourceId</span><span class="sxs-lookup"><span data-stu-id="072c7-144">sourceId</span></span>|<span data-ttu-id="072c7-145">Строка</span><span class="sxs-lookup"><span data-stu-id="072c7-145">String</span></span>|<span data-ttu-id="072c7-146">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="072c7-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="072c7-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="072c7-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="072c7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="072c7-148">Response</span></span>
<span data-ttu-id="072c7-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="072c7-149">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="072c7-150">Пример</span><span class="sxs-lookup"><span data-stu-id="072c7-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="072c7-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="072c7-151">Request</span></span>
<span data-ttu-id="072c7-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="072c7-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 449

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="072c7-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="072c7-153">Response</span></span>
<span data-ttu-id="072c7-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="072c7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 498

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




