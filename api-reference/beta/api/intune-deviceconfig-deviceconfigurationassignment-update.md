---
title: Обновление объекта deviceConfigurationAssignment
description: Обновление свойств объекта deviceConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fadf102764db283ad97af6905c8b0c937f7f44fb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42754463"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="2f499-103">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2f499-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="2f499-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f499-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f499-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f499-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f499-106">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2f499-106">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f499-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f499-107">Prerequisites</span></span>
<span data-ttu-id="2f499-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f499-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f499-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f499-110">Permission type</span></span>|<span data-ttu-id="2f499-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f499-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f499-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f499-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f499-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f499-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f499-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f499-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f499-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f499-115">Not supported.</span></span>|
|<span data-ttu-id="2f499-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2f499-116">Application</span></span>|<span data-ttu-id="2f499-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f499-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f499-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f499-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2f499-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2f499-119">Request headers</span></span>
|<span data-ttu-id="2f499-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f499-120">Header</span></span>|<span data-ttu-id="2f499-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2f499-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f499-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f499-122">Authorization</span></span>|<span data-ttu-id="2f499-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f499-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f499-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2f499-124">Accept</span></span>|<span data-ttu-id="2f499-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f499-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f499-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f499-126">Request body</span></span>
<span data-ttu-id="2f499-127">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f499-127">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="2f499-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2f499-128">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="2f499-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f499-129">Property</span></span>|<span data-ttu-id="2f499-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2f499-130">Type</span></span>|<span data-ttu-id="2f499-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2f499-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f499-132">id</span><span class="sxs-lookup"><span data-stu-id="2f499-132">id</span></span>|<span data-ttu-id="2f499-133">String</span><span class="sxs-lookup"><span data-stu-id="2f499-133">String</span></span>|<span data-ttu-id="2f499-134">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="2f499-134">The key of the assignment.</span></span>|
|<span data-ttu-id="2f499-135">target</span><span class="sxs-lookup"><span data-stu-id="2f499-135">target</span></span>|[<span data-ttu-id="2f499-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2f499-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2f499-137">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="2f499-137">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="2f499-138">source</span><span class="sxs-lookup"><span data-stu-id="2f499-138">source</span></span>|[<span data-ttu-id="2f499-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="2f499-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="2f499-140">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="2f499-140">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="2f499-141">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f499-141">This property is read-only.</span></span> <span data-ttu-id="2f499-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="2f499-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="2f499-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="2f499-143">sourceId</span></span>|<span data-ttu-id="2f499-144">String</span><span class="sxs-lookup"><span data-stu-id="2f499-144">String</span></span>|<span data-ttu-id="2f499-145">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="2f499-145">The identifier of the source of the assignment.</span></span> <span data-ttu-id="2f499-146">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f499-146">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="2f499-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f499-147">Response</span></span>
<span data-ttu-id="2f499-148">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f499-148">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f499-149">Пример</span><span class="sxs-lookup"><span data-stu-id="2f499-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f499-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f499-150">Request</span></span>
<span data-ttu-id="2f499-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f499-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f499-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f499-152">Response</span></span>
<span data-ttu-id="2f499-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f499-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




