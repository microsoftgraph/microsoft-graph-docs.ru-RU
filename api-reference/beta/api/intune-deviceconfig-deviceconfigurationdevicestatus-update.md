---
title: Обновление объекта deviceConfigurationDeviceStatus
description: Обновление свойств объекта deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b35baeb458fede5ba5ee58f287a3fe0e9b58a9cf
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792928"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="ff712-103">Обновление объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="ff712-103">Update deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="ff712-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff712-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff712-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff712-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff712-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff712-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff712-107">Обновление свойств объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ff712-107">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff712-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff712-108">Prerequisites</span></span>
<span data-ttu-id="ff712-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ff712-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ff712-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff712-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff712-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff712-111">Permission type</span></span>|<span data-ttu-id="ff712-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff712-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff712-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff712-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff712-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff712-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff712-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff712-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff712-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff712-116">Not supported.</span></span>|
|<span data-ttu-id="ff712-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff712-117">Application</span></span>|<span data-ttu-id="ff712-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff712-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff712-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff712-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="ff712-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ff712-120">Request headers</span></span>
|<span data-ttu-id="ff712-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff712-121">Header</span></span>|<span data-ttu-id="ff712-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff712-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff712-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff712-123">Authorization</span></span>|<span data-ttu-id="ff712-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff712-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff712-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff712-125">Accept</span></span>|<span data-ttu-id="ff712-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff712-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff712-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff712-127">Request body</span></span>
<span data-ttu-id="ff712-128">В теле запроса добавьте представление объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff712-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="ff712-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ff712-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="ff712-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff712-130">Property</span></span>|<span data-ttu-id="ff712-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ff712-131">Type</span></span>|<span data-ttu-id="ff712-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ff712-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff712-133">id</span><span class="sxs-lookup"><span data-stu-id="ff712-133">id</span></span>|<span data-ttu-id="ff712-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ff712-134">String</span></span>|<span data-ttu-id="ff712-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ff712-135">Key of the entity.</span></span>|
|<span data-ttu-id="ff712-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ff712-136">deviceDisplayName</span></span>|<span data-ttu-id="ff712-137">String</span><span class="sxs-lookup"><span data-stu-id="ff712-137">String</span></span>|<span data-ttu-id="ff712-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="ff712-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ff712-139">userName</span><span class="sxs-lookup"><span data-stu-id="ff712-139">userName</span></span>|<span data-ttu-id="ff712-140">String</span><span class="sxs-lookup"><span data-stu-id="ff712-140">String</span></span>|<span data-ttu-id="ff712-141">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="ff712-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="ff712-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ff712-142">deviceModel</span></span>|<span data-ttu-id="ff712-143">String</span><span class="sxs-lookup"><span data-stu-id="ff712-143">String</span></span>|<span data-ttu-id="ff712-144">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="ff712-144">The device model that is being reported</span></span>|
|<span data-ttu-id="ff712-145">platform</span><span class="sxs-lookup"><span data-stu-id="ff712-145">platform</span></span>|<span data-ttu-id="ff712-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ff712-146">Int32</span></span>|<span data-ttu-id="ff712-147">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="ff712-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="ff712-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ff712-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ff712-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff712-149">DateTimeOffset</span></span>|<span data-ttu-id="ff712-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ff712-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ff712-151">status</span><span class="sxs-lookup"><span data-stu-id="ff712-151">status</span></span>|[<span data-ttu-id="ff712-152">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="ff712-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ff712-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="ff712-153">Compliance status of the policy report.</span></span> <span data-ttu-id="ff712-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ff712-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ff712-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff712-155">lastReportedDateTime</span></span>|<span data-ttu-id="ff712-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff712-156">DateTimeOffset</span></span>|<span data-ttu-id="ff712-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="ff712-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ff712-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ff712-158">userPrincipalName</span></span>|<span data-ttu-id="ff712-159">String</span><span class="sxs-lookup"><span data-stu-id="ff712-159">String</span></span>|<span data-ttu-id="ff712-160">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="ff712-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ff712-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff712-161">Response</span></span>
<span data-ttu-id="ff712-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ff712-162">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff712-163">Пример</span><span class="sxs-lookup"><span data-stu-id="ff712-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff712-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff712-164">Request</span></span>
<span data-ttu-id="ff712-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff712-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
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

### <a name="response"></a><span data-ttu-id="ff712-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff712-166">Response</span></span>
<span data-ttu-id="ff712-167">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="ff712-167">Here is an example of the response.</span></span> <span data-ttu-id="ff712-168">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="ff712-168">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ff712-169">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ff712-169">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



