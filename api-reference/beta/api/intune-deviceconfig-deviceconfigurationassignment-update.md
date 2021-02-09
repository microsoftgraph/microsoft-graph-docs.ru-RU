---
title: Обновление объекта deviceConfigurationAssignment
description: Обновление свойств объекта deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a236381c4f860e071094cfda8e8ea9567658a99
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153972"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="c8d9a-103">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c8d9a-103">Update deviceConfigurationAssignment</span></span>

<span data-ttu-id="c8d9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8d9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8d9a-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8d9a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8d9a-107">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c8d9a-107">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8d9a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c8d9a-108">Prerequisites</span></span>
<span data-ttu-id="c8d9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8d9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8d9a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8d9a-111">Permission type</span></span>|<span data-ttu-id="c8d9a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8d9a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8d9a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8d9a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8d9a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8d9a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8d9a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8d9a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8d9a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-116">Not supported.</span></span>|
|<span data-ttu-id="c8d9a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8d9a-117">Application</span></span>|<span data-ttu-id="c8d9a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8d9a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8d9a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8d9a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c8d9a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8d9a-120">Request headers</span></span>
|<span data-ttu-id="c8d9a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8d9a-121">Header</span></span>|<span data-ttu-id="c8d9a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c8d9a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8d9a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8d9a-123">Authorization</span></span>|<span data-ttu-id="c8d9a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8d9a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8d9a-125">Accept</span></span>|<span data-ttu-id="c8d9a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8d9a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8d9a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8d9a-127">Request body</span></span>
<span data-ttu-id="c8d9a-128">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-128">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="c8d9a-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c8d9a-129">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="c8d9a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8d9a-130">Property</span></span>|<span data-ttu-id="c8d9a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c8d9a-131">Type</span></span>|<span data-ttu-id="c8d9a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c8d9a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8d9a-133">id</span><span class="sxs-lookup"><span data-stu-id="c8d9a-133">id</span></span>|<span data-ttu-id="c8d9a-134">String</span><span class="sxs-lookup"><span data-stu-id="c8d9a-134">String</span></span>|<span data-ttu-id="c8d9a-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-135">The key of the assignment.</span></span>|
|<span data-ttu-id="c8d9a-136">target</span><span class="sxs-lookup"><span data-stu-id="c8d9a-136">target</span></span>|[<span data-ttu-id="c8d9a-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c8d9a-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c8d9a-138">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="c8d9a-139">source</span><span class="sxs-lookup"><span data-stu-id="c8d9a-139">source</span></span>|[<span data-ttu-id="c8d9a-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="c8d9a-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="c8d9a-141">Источник назначения для конфигурации устройства, прямой или сет политик.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="c8d9a-142">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-142">This property is read-only.</span></span> <span data-ttu-id="c8d9a-143">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="c8d9a-144">sourceId</span><span class="sxs-lookup"><span data-stu-id="c8d9a-144">sourceId</span></span>|<span data-ttu-id="c8d9a-145">String</span><span class="sxs-lookup"><span data-stu-id="c8d9a-145">String</span></span>|<span data-ttu-id="c8d9a-146">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="c8d9a-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="c8d9a-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8d9a-148">Response</span></span>
<span data-ttu-id="c8d9a-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-149">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8d9a-150">Пример</span><span class="sxs-lookup"><span data-stu-id="c8d9a-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8d9a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8d9a-151">Request</span></span>
<span data-ttu-id="c8d9a-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c8d9a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8d9a-153">Response</span></span>
<span data-ttu-id="c8d9a-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8d9a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




