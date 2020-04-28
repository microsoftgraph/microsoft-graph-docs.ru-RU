---
title: Создание объекта deviceConfigurationDeviceStatus
description: Создание объекта deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ee36619a3877e5253d3e55802af8481572656666
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433444"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="b9316-103">Создание объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b9316-103">Create deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="b9316-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9316-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9316-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9316-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9316-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9316-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9316-107">Создание объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b9316-107">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9316-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b9316-108">Prerequisites</span></span>
<span data-ttu-id="b9316-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9316-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9316-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9316-111">Permission type</span></span>|<span data-ttu-id="b9316-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9316-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9316-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9316-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9316-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9316-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9316-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9316-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9316-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9316-116">Not supported.</span></span>|
|<span data-ttu-id="b9316-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9316-117">Application</span></span>|<span data-ttu-id="b9316-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9316-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9316-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9316-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b9316-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b9316-120">Request headers</span></span>
|<span data-ttu-id="b9316-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9316-121">Header</span></span>|<span data-ttu-id="b9316-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9316-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9316-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9316-123">Authorization</span></span>|<span data-ttu-id="b9316-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9316-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9316-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b9316-125">Accept</span></span>|<span data-ttu-id="b9316-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9316-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9316-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9316-127">Request body</span></span>
<span data-ttu-id="b9316-128">В теле запроса добавьте представление объекта deviceConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9316-128">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="b9316-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="b9316-129">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="b9316-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9316-130">Property</span></span>|<span data-ttu-id="b9316-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b9316-131">Type</span></span>|<span data-ttu-id="b9316-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b9316-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9316-133">id</span><span class="sxs-lookup"><span data-stu-id="b9316-133">id</span></span>|<span data-ttu-id="b9316-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b9316-134">String</span></span>|<span data-ttu-id="b9316-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b9316-135">Key of the entity.</span></span>|
|<span data-ttu-id="b9316-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b9316-136">deviceDisplayName</span></span>|<span data-ttu-id="b9316-137">String</span><span class="sxs-lookup"><span data-stu-id="b9316-137">String</span></span>|<span data-ttu-id="b9316-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="b9316-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b9316-139">userName</span><span class="sxs-lookup"><span data-stu-id="b9316-139">userName</span></span>|<span data-ttu-id="b9316-140">String</span><span class="sxs-lookup"><span data-stu-id="b9316-140">String</span></span>|<span data-ttu-id="b9316-141">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="b9316-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="b9316-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b9316-142">deviceModel</span></span>|<span data-ttu-id="b9316-143">String</span><span class="sxs-lookup"><span data-stu-id="b9316-143">String</span></span>|<span data-ttu-id="b9316-144">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="b9316-144">The device model that is being reported</span></span>|
|<span data-ttu-id="b9316-145">platform</span><span class="sxs-lookup"><span data-stu-id="b9316-145">platform</span></span>|<span data-ttu-id="b9316-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b9316-146">Int32</span></span>|<span data-ttu-id="b9316-147">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="b9316-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="b9316-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b9316-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b9316-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9316-149">DateTimeOffset</span></span>|<span data-ttu-id="b9316-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b9316-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b9316-151">status</span><span class="sxs-lookup"><span data-stu-id="b9316-151">status</span></span>|[<span data-ttu-id="b9316-152">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="b9316-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b9316-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="b9316-153">Compliance status of the policy report.</span></span> <span data-ttu-id="b9316-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b9316-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b9316-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9316-155">lastReportedDateTime</span></span>|<span data-ttu-id="b9316-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9316-156">DateTimeOffset</span></span>|<span data-ttu-id="b9316-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="b9316-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b9316-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9316-158">userPrincipalName</span></span>|<span data-ttu-id="b9316-159">String</span><span class="sxs-lookup"><span data-stu-id="b9316-159">String</span></span>|<span data-ttu-id="b9316-160">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9316-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b9316-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9316-161">Response</span></span>
<span data-ttu-id="b9316-162">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b9316-162">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9316-163">Пример</span><span class="sxs-lookup"><span data-stu-id="b9316-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9316-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9316-164">Request</span></span>
<span data-ttu-id="b9316-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9316-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b9316-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9316-166">Response</span></span>
<span data-ttu-id="b9316-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9316-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



