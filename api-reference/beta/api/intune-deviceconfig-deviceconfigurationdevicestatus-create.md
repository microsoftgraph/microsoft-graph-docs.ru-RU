---
title: Создание объекта deviceConfigurationDeviceStatus
description: Создание объекта deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6816630400536d488d2176ad62ffefb82ab7d973
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059021"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="2dd4f-103">Создание объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2dd4f-103">Create deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="2dd4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dd4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2dd4f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dd4f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dd4f-107">Создание объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="2dd4f-107">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2dd4f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2dd4f-108">Prerequisites</span></span>
<span data-ttu-id="2dd4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dd4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dd4f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2dd4f-111">Permission type</span></span>|<span data-ttu-id="2dd4f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2dd4f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2dd4f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2dd4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2dd4f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dd4f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2dd4f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2dd4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2dd4f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-116">Not supported.</span></span>|
|<span data-ttu-id="2dd4f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2dd4f-117">Application</span></span>|<span data-ttu-id="2dd4f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dd4f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2dd4f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2dd4f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2dd4f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2dd4f-120">Request headers</span></span>
|<span data-ttu-id="2dd4f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2dd4f-121">Header</span></span>|<span data-ttu-id="2dd4f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2dd4f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2dd4f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2dd4f-123">Authorization</span></span>|<span data-ttu-id="2dd4f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2dd4f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2dd4f-125">Accept</span></span>|<span data-ttu-id="2dd4f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2dd4f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dd4f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2dd4f-127">Request body</span></span>
<span data-ttu-id="2dd4f-128">В теле запроса добавьте представление объекта deviceConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-128">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="2dd4f-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-129">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="2dd4f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dd4f-130">Property</span></span>|<span data-ttu-id="2dd4f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2dd4f-131">Type</span></span>|<span data-ttu-id="2dd4f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2dd4f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dd4f-133">id</span><span class="sxs-lookup"><span data-stu-id="2dd4f-133">id</span></span>|<span data-ttu-id="2dd4f-134">String</span><span class="sxs-lookup"><span data-stu-id="2dd4f-134">String</span></span>|<span data-ttu-id="2dd4f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-135">Key of the entity.</span></span>|
|<span data-ttu-id="2dd4f-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2dd4f-136">deviceDisplayName</span></span>|<span data-ttu-id="2dd4f-137">String</span><span class="sxs-lookup"><span data-stu-id="2dd4f-137">String</span></span>|<span data-ttu-id="2dd4f-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2dd4f-139">userName</span><span class="sxs-lookup"><span data-stu-id="2dd4f-139">userName</span></span>|<span data-ttu-id="2dd4f-140">String</span><span class="sxs-lookup"><span data-stu-id="2dd4f-140">String</span></span>|<span data-ttu-id="2dd4f-141">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="2dd4f-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="2dd4f-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2dd4f-142">deviceModel</span></span>|<span data-ttu-id="2dd4f-143">String</span><span class="sxs-lookup"><span data-stu-id="2dd4f-143">String</span></span>|<span data-ttu-id="2dd4f-144">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="2dd4f-144">The device model that is being reported</span></span>|
|<span data-ttu-id="2dd4f-145">платформа</span><span class="sxs-lookup"><span data-stu-id="2dd4f-145">platform</span></span>|<span data-ttu-id="2dd4f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2dd4f-146">Int32</span></span>|<span data-ttu-id="2dd4f-147">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="2dd4f-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="2dd4f-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2dd4f-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2dd4f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dd4f-149">DateTimeOffset</span></span>|<span data-ttu-id="2dd4f-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="2dd4f-151">status</span><span class="sxs-lookup"><span data-stu-id="2dd4f-151">status</span></span>|[<span data-ttu-id="2dd4f-152">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="2dd4f-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2dd4f-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-153">Compliance status of the policy report.</span></span> <span data-ttu-id="2dd4f-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2dd4f-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2dd4f-155">lastReportedDateTime</span></span>|<span data-ttu-id="2dd4f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dd4f-156">DateTimeOffset</span></span>|<span data-ttu-id="2dd4f-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2dd4f-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2dd4f-158">userPrincipalName</span></span>|<span data-ttu-id="2dd4f-159">String</span><span class="sxs-lookup"><span data-stu-id="2dd4f-159">String</span></span>|<span data-ttu-id="2dd4f-160">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2dd4f-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="2dd4f-161">Response</span></span>
<span data-ttu-id="2dd4f-162">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-162">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dd4f-163">Пример</span><span class="sxs-lookup"><span data-stu-id="2dd4f-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="2dd4f-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="2dd4f-164">Request</span></span>
<span data-ttu-id="2dd4f-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="2dd4f-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="2dd4f-166">Response</span></span>
<span data-ttu-id="2dd4f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2dd4f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 496

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```






