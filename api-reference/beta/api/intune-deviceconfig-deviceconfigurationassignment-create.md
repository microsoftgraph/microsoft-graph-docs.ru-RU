---
title: Создание объекта deviceConfigurationAssignment
description: Создание объекта deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 44fe4ceeed762c122d6ef4915813dc23924924bd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724875"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="a18a0-103">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a18a0-103">Create deviceConfigurationAssignment</span></span>

<span data-ttu-id="a18a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a18a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a18a0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a18a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a18a0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a18a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a18a0-107">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a18a0-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a18a0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a18a0-108">Prerequisites</span></span>
<span data-ttu-id="a18a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a18a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a18a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a18a0-111">Permission type</span></span>|<span data-ttu-id="a18a0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a18a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a18a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a18a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a18a0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a18a0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a18a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a18a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a18a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a18a0-116">Not supported.</span></span>|
|<span data-ttu-id="a18a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a18a0-117">Application</span></span>|<span data-ttu-id="a18a0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a18a0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a18a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a18a0-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a18a0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a18a0-120">Request headers</span></span>
|<span data-ttu-id="a18a0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a18a0-121">Header</span></span>|<span data-ttu-id="a18a0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a18a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a18a0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a18a0-123">Authorization</span></span>|<span data-ttu-id="a18a0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a18a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a18a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a18a0-125">Accept</span></span>|<span data-ttu-id="a18a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a18a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a18a0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a18a0-127">Request body</span></span>
<span data-ttu-id="a18a0-128">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a18a0-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="a18a0-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="a18a0-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="a18a0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a18a0-130">Property</span></span>|<span data-ttu-id="a18a0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a18a0-131">Type</span></span>|<span data-ttu-id="a18a0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a18a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a18a0-133">id</span><span class="sxs-lookup"><span data-stu-id="a18a0-133">id</span></span>|<span data-ttu-id="a18a0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a18a0-134">String</span></span>|<span data-ttu-id="a18a0-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="a18a0-135">The key of the assignment.</span></span>|
|<span data-ttu-id="a18a0-136">target</span><span class="sxs-lookup"><span data-stu-id="a18a0-136">target</span></span>|[<span data-ttu-id="a18a0-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a18a0-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a18a0-138">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="a18a0-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="a18a0-139">source</span><span class="sxs-lookup"><span data-stu-id="a18a0-139">source</span></span>|[<span data-ttu-id="a18a0-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="a18a0-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="a18a0-141">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="a18a0-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="a18a0-142">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a18a0-142">This property is read-only.</span></span> <span data-ttu-id="a18a0-143">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="a18a0-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="a18a0-144">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="a18a0-144">sourceId</span></span>|<span data-ttu-id="a18a0-145">Строка</span><span class="sxs-lookup"><span data-stu-id="a18a0-145">String</span></span>|<span data-ttu-id="a18a0-146">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="a18a0-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="a18a0-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a18a0-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="a18a0-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a18a0-148">Response</span></span>
<span data-ttu-id="a18a0-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a18a0-149">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a18a0-150">Пример</span><span class="sxs-lookup"><span data-stu-id="a18a0-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="a18a0-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="a18a0-151">Request</span></span>
<span data-ttu-id="a18a0-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a18a0-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a18a0-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="a18a0-153">Response</span></span>
<span data-ttu-id="a18a0-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a18a0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





