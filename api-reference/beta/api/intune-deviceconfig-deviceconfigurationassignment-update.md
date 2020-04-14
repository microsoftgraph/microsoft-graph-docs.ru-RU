---
title: Обновление объекта deviceConfigurationAssignment
description: Обновление свойств объекта deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a7b4df7f80499812fde6d717fca1a383704ce98
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433586"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="6fd93-103">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6fd93-103">Update deviceConfigurationAssignment</span></span>

<span data-ttu-id="6fd93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fd93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fd93-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fd93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fd93-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fd93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fd93-107">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6fd93-107">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fd93-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6fd93-108">Prerequisites</span></span>
<span data-ttu-id="6fd93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fd93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fd93-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fd93-111">Permission type</span></span>|<span data-ttu-id="6fd93-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fd93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fd93-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fd93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fd93-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fd93-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6fd93-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fd93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fd93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fd93-116">Not supported.</span></span>|
|<span data-ttu-id="6fd93-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6fd93-117">Application</span></span>|<span data-ttu-id="6fd93-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fd93-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fd93-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fd93-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6fd93-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6fd93-120">Request headers</span></span>
|<span data-ttu-id="6fd93-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6fd93-121">Header</span></span>|<span data-ttu-id="6fd93-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6fd93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fd93-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fd93-123">Authorization</span></span>|<span data-ttu-id="6fd93-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fd93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fd93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6fd93-125">Accept</span></span>|<span data-ttu-id="6fd93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fd93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fd93-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6fd93-127">Request body</span></span>
<span data-ttu-id="6fd93-128">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fd93-128">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="6fd93-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6fd93-129">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="6fd93-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fd93-130">Property</span></span>|<span data-ttu-id="6fd93-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6fd93-131">Type</span></span>|<span data-ttu-id="6fd93-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6fd93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fd93-133">id</span><span class="sxs-lookup"><span data-stu-id="6fd93-133">id</span></span>|<span data-ttu-id="6fd93-134">String</span><span class="sxs-lookup"><span data-stu-id="6fd93-134">String</span></span>|<span data-ttu-id="6fd93-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="6fd93-135">The key of the assignment.</span></span>|
|<span data-ttu-id="6fd93-136">target</span><span class="sxs-lookup"><span data-stu-id="6fd93-136">target</span></span>|[<span data-ttu-id="6fd93-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6fd93-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6fd93-138">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="6fd93-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="6fd93-139">source</span><span class="sxs-lookup"><span data-stu-id="6fd93-139">source</span></span>|[<span data-ttu-id="6fd93-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="6fd93-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="6fd93-141">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="6fd93-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="6fd93-142">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6fd93-142">This property is read-only.</span></span> <span data-ttu-id="6fd93-143">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="6fd93-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="6fd93-144">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="6fd93-144">sourceId</span></span>|<span data-ttu-id="6fd93-145">String</span><span class="sxs-lookup"><span data-stu-id="6fd93-145">String</span></span>|<span data-ttu-id="6fd93-146">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="6fd93-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="6fd93-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6fd93-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="6fd93-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fd93-148">Response</span></span>
<span data-ttu-id="6fd93-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6fd93-149">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fd93-150">Пример</span><span class="sxs-lookup"><span data-stu-id="6fd93-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fd93-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fd93-151">Request</span></span>
<span data-ttu-id="6fd93-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6fd93-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="6fd93-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fd93-153">Response</span></span>
<span data-ttu-id="6fd93-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6fd93-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



