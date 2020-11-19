---
title: Создание объекта deviceConfigurationAssignment
description: Создание объекта deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f90533687916a8b796331cb4b15d4e0d5ea7ac28
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49213786"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="8ee7b-103">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8ee7b-103">Create deviceConfigurationAssignment</span></span>

<span data-ttu-id="8ee7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ee7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ee7b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ee7b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ee7b-107">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8ee7b-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ee7b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8ee7b-108">Prerequisites</span></span>
<span data-ttu-id="8ee7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ee7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ee7b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ee7b-111">Permission type</span></span>|<span data-ttu-id="8ee7b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ee7b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ee7b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ee7b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ee7b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ee7b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ee7b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ee7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ee7b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-116">Not supported.</span></span>|
|<span data-ttu-id="8ee7b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8ee7b-117">Application</span></span>|<span data-ttu-id="8ee7b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ee7b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ee7b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ee7b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8ee7b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8ee7b-120">Request headers</span></span>
|<span data-ttu-id="8ee7b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ee7b-121">Header</span></span>|<span data-ttu-id="8ee7b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ee7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ee7b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ee7b-123">Authorization</span></span>|<span data-ttu-id="8ee7b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ee7b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ee7b-125">Accept</span></span>|<span data-ttu-id="8ee7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ee7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ee7b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ee7b-127">Request body</span></span>
<span data-ttu-id="8ee7b-128">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="8ee7b-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="8ee7b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ee7b-130">Property</span></span>|<span data-ttu-id="8ee7b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8ee7b-131">Type</span></span>|<span data-ttu-id="8ee7b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8ee7b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ee7b-133">id</span><span class="sxs-lookup"><span data-stu-id="8ee7b-133">id</span></span>|<span data-ttu-id="8ee7b-134">String</span><span class="sxs-lookup"><span data-stu-id="8ee7b-134">String</span></span>|<span data-ttu-id="8ee7b-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-135">The key of the assignment.</span></span>|
|<span data-ttu-id="8ee7b-136">target</span><span class="sxs-lookup"><span data-stu-id="8ee7b-136">target</span></span>|[<span data-ttu-id="8ee7b-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8ee7b-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8ee7b-138">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="8ee7b-139">source</span><span class="sxs-lookup"><span data-stu-id="8ee7b-139">source</span></span>|[<span data-ttu-id="8ee7b-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="8ee7b-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="8ee7b-141">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="8ee7b-142">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-142">This property is read-only.</span></span> <span data-ttu-id="8ee7b-143">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="8ee7b-144">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="8ee7b-144">sourceId</span></span>|<span data-ttu-id="8ee7b-145">String</span><span class="sxs-lookup"><span data-stu-id="8ee7b-145">String</span></span>|<span data-ttu-id="8ee7b-146">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="8ee7b-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="8ee7b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ee7b-148">Response</span></span>
<span data-ttu-id="8ee7b-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-149">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ee7b-150">Пример</span><span class="sxs-lookup"><span data-stu-id="8ee7b-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ee7b-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ee7b-151">Request</span></span>
<span data-ttu-id="8ee7b-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 385

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="8ee7b-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ee7b-153">Response</span></span>
<span data-ttu-id="8ee7b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ee7b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 434

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




