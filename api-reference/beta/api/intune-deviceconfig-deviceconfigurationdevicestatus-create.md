---
title: Создание объекта deviceConfigurationDeviceStatus
description: Создание объекта deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2e3ee8c4d2d29139cba0d094f6a755f026b652a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32469518"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="6d947-103">Создание объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="6d947-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="6d947-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d947-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d947-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d947-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d947-106">Создание объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="6d947-106">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d947-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6d947-107">Prerequisites</span></span>
<span data-ttu-id="6d947-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d947-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d947-110">Permission type</span></span>|<span data-ttu-id="6d947-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d947-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d947-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d947-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d947-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d947-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d947-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d947-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d947-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d947-115">Not supported.</span></span>|
|<span data-ttu-id="6d947-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d947-116">Application</span></span>|<span data-ttu-id="6d947-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d947-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d947-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d947-118">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6d947-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d947-119">Request headers</span></span>
|<span data-ttu-id="6d947-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d947-120">Header</span></span>|<span data-ttu-id="6d947-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6d947-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d947-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d947-122">Authorization</span></span>|<span data-ttu-id="6d947-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d947-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d947-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6d947-124">Accept</span></span>|<span data-ttu-id="6d947-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d947-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d947-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d947-126">Request body</span></span>
<span data-ttu-id="6d947-127">В теле запроса добавьте представление объекта deviceConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d947-127">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="6d947-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="6d947-128">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="6d947-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d947-129">Property</span></span>|<span data-ttu-id="6d947-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6d947-130">Type</span></span>|<span data-ttu-id="6d947-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6d947-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d947-132">id</span><span class="sxs-lookup"><span data-stu-id="6d947-132">id</span></span>|<span data-ttu-id="6d947-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6d947-133">String</span></span>|<span data-ttu-id="6d947-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6d947-134">Key of the entity.</span></span>|
|<span data-ttu-id="6d947-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6d947-135">deviceDisplayName</span></span>|<span data-ttu-id="6d947-136">String</span><span class="sxs-lookup"><span data-stu-id="6d947-136">String</span></span>|<span data-ttu-id="6d947-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="6d947-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="6d947-138">userName</span><span class="sxs-lookup"><span data-stu-id="6d947-138">userName</span></span>|<span data-ttu-id="6d947-139">String</span><span class="sxs-lookup"><span data-stu-id="6d947-139">String</span></span>|<span data-ttu-id="6d947-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="6d947-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="6d947-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6d947-141">deviceModel</span></span>|<span data-ttu-id="6d947-142">String</span><span class="sxs-lookup"><span data-stu-id="6d947-142">String</span></span>|<span data-ttu-id="6d947-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="6d947-143">The device model that is being reported</span></span>|
|<span data-ttu-id="6d947-144">platform</span><span class="sxs-lookup"><span data-stu-id="6d947-144">platform</span></span>|<span data-ttu-id="6d947-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6d947-145">Int32</span></span>|<span data-ttu-id="6d947-146">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="6d947-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="6d947-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6d947-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6d947-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d947-148">DateTimeOffset</span></span>|<span data-ttu-id="6d947-149">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6d947-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="6d947-150">status</span><span class="sxs-lookup"><span data-stu-id="6d947-150">status</span></span>|[<span data-ttu-id="6d947-151">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="6d947-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6d947-152">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="6d947-152">Compliance status of the policy report.</span></span> <span data-ttu-id="6d947-153">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6d947-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6d947-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d947-154">lastReportedDateTime</span></span>|<span data-ttu-id="6d947-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d947-155">DateTimeOffset</span></span>|<span data-ttu-id="6d947-156">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="6d947-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="6d947-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6d947-157">userPrincipalName</span></span>|<span data-ttu-id="6d947-158">String</span><span class="sxs-lookup"><span data-stu-id="6d947-158">String</span></span>|<span data-ttu-id="6d947-159">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="6d947-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="6d947-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d947-160">Response</span></span>
<span data-ttu-id="6d947-161">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6d947-161">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d947-162">Пример</span><span class="sxs-lookup"><span data-stu-id="6d947-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d947-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d947-163">Request</span></span>
<span data-ttu-id="6d947-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d947-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6d947-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d947-165">Response</span></span>
<span data-ttu-id="6d947-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d947-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





