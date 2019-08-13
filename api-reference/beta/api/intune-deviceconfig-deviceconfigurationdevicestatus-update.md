---
title: Обновление объекта deviceConfigurationDeviceStatus
description: Обновление свойств объекта deviceConfigurationDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 17b7b79dc09cf6edb817dcee2fa7ff154a4effda
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345913"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="6565f-103">Обновление объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="6565f-103">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="6565f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6565f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6565f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6565f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6565f-106">Обновление свойств объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="6565f-106">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6565f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6565f-107">Prerequisites</span></span>
<span data-ttu-id="6565f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6565f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6565f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6565f-110">Permission type</span></span>|<span data-ttu-id="6565f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6565f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6565f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6565f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6565f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6565f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6565f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6565f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6565f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6565f-115">Not supported.</span></span>|
|<span data-ttu-id="6565f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6565f-116">Application</span></span>|<span data-ttu-id="6565f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6565f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6565f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6565f-118">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerCertificateProfileBase/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="6565f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6565f-119">Request headers</span></span>
|<span data-ttu-id="6565f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6565f-120">Header</span></span>|<span data-ttu-id="6565f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6565f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6565f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6565f-122">Authorization</span></span>|<span data-ttu-id="6565f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6565f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6565f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6565f-124">Accept</span></span>|<span data-ttu-id="6565f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6565f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6565f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6565f-126">Request body</span></span>
<span data-ttu-id="6565f-127">В теле запроса добавьте представление объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6565f-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="6565f-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="6565f-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="6565f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6565f-129">Property</span></span>|<span data-ttu-id="6565f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6565f-130">Type</span></span>|<span data-ttu-id="6565f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6565f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6565f-132">id</span><span class="sxs-lookup"><span data-stu-id="6565f-132">id</span></span>|<span data-ttu-id="6565f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6565f-133">String</span></span>|<span data-ttu-id="6565f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6565f-134">Key of the entity.</span></span>|
|<span data-ttu-id="6565f-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6565f-135">deviceDisplayName</span></span>|<span data-ttu-id="6565f-136">String</span><span class="sxs-lookup"><span data-stu-id="6565f-136">String</span></span>|<span data-ttu-id="6565f-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="6565f-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="6565f-138">userName</span><span class="sxs-lookup"><span data-stu-id="6565f-138">userName</span></span>|<span data-ttu-id="6565f-139">String</span><span class="sxs-lookup"><span data-stu-id="6565f-139">String</span></span>|<span data-ttu-id="6565f-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="6565f-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="6565f-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6565f-141">deviceModel</span></span>|<span data-ttu-id="6565f-142">String</span><span class="sxs-lookup"><span data-stu-id="6565f-142">String</span></span>|<span data-ttu-id="6565f-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="6565f-143">The device model that is being reported</span></span>|
|<span data-ttu-id="6565f-144">platform</span><span class="sxs-lookup"><span data-stu-id="6565f-144">platform</span></span>|<span data-ttu-id="6565f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6565f-145">Int32</span></span>|<span data-ttu-id="6565f-146">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="6565f-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="6565f-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6565f-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6565f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6565f-148">DateTimeOffset</span></span>|<span data-ttu-id="6565f-149">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6565f-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="6565f-150">status</span><span class="sxs-lookup"><span data-stu-id="6565f-150">status</span></span>|[<span data-ttu-id="6565f-151">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="6565f-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6565f-152">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="6565f-152">Compliance status of the policy report.</span></span> <span data-ttu-id="6565f-153">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6565f-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6565f-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6565f-154">lastReportedDateTime</span></span>|<span data-ttu-id="6565f-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6565f-155">DateTimeOffset</span></span>|<span data-ttu-id="6565f-156">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="6565f-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="6565f-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6565f-157">userPrincipalName</span></span>|<span data-ttu-id="6565f-158">String</span><span class="sxs-lookup"><span data-stu-id="6565f-158">String</span></span>|<span data-ttu-id="6565f-159">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="6565f-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="6565f-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="6565f-160">Response</span></span>
<span data-ttu-id="6565f-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6565f-161">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6565f-162">Пример</span><span class="sxs-lookup"><span data-stu-id="6565f-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="6565f-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="6565f-163">Request</span></span>
<span data-ttu-id="6565f-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6565f-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6565f-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="6565f-165">Response</span></span>
<span data-ttu-id="6565f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6565f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






