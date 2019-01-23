---
title: Создание объекта deviceConfigurationDeviceStatus
description: Создание объекта deviceConfigurationDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f75b9a74d7d199e490d9ebcf3fb17aa79e5d1cdb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423505"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="46ea1-103">Создание объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="46ea1-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="46ea1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46ea1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="46ea1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ea1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46ea1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46ea1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46ea1-107">Создание объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="46ea1-107">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46ea1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="46ea1-108">Prerequisites</span></span>
<span data-ttu-id="46ea1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="46ea1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="46ea1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46ea1-111">Permission type</span></span>|<span data-ttu-id="46ea1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46ea1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46ea1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46ea1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46ea1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46ea1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46ea1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46ea1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46ea1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ea1-116">Not supported.</span></span>|
|<span data-ttu-id="46ea1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46ea1-117">Application</span></span>|<span data-ttu-id="46ea1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ea1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46ea1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46ea1-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="46ea1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46ea1-120">Request headers</span></span>
|<span data-ttu-id="46ea1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46ea1-121">Header</span></span>|<span data-ttu-id="46ea1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="46ea1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46ea1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46ea1-123">Authorization</span></span>|<span data-ttu-id="46ea1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="46ea1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46ea1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46ea1-125">Accept</span></span>|<span data-ttu-id="46ea1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46ea1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46ea1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46ea1-127">Request body</span></span>
<span data-ttu-id="46ea1-128">В теле запроса добавьте представление объекта deviceConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46ea1-128">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="46ea1-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="46ea1-129">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="46ea1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="46ea1-130">Property</span></span>|<span data-ttu-id="46ea1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="46ea1-131">Type</span></span>|<span data-ttu-id="46ea1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="46ea1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46ea1-133">id</span><span class="sxs-lookup"><span data-stu-id="46ea1-133">id</span></span>|<span data-ttu-id="46ea1-134">String</span><span class="sxs-lookup"><span data-stu-id="46ea1-134">String</span></span>|<span data-ttu-id="46ea1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="46ea1-135">Key of the entity.</span></span>|
|<span data-ttu-id="46ea1-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="46ea1-136">deviceDisplayName</span></span>|<span data-ttu-id="46ea1-137">String</span><span class="sxs-lookup"><span data-stu-id="46ea1-137">String</span></span>|<span data-ttu-id="46ea1-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="46ea1-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="46ea1-139">userName</span><span class="sxs-lookup"><span data-stu-id="46ea1-139">userName</span></span>|<span data-ttu-id="46ea1-140">String</span><span class="sxs-lookup"><span data-stu-id="46ea1-140">String</span></span>|<span data-ttu-id="46ea1-141">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="46ea1-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="46ea1-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="46ea1-142">deviceModel</span></span>|<span data-ttu-id="46ea1-143">String</span><span class="sxs-lookup"><span data-stu-id="46ea1-143">String</span></span>|<span data-ttu-id="46ea1-144">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="46ea1-144">The device model that is being reported</span></span>|
|<span data-ttu-id="46ea1-145">platform</span><span class="sxs-lookup"><span data-stu-id="46ea1-145">platform</span></span>|<span data-ttu-id="46ea1-146">Int32</span><span class="sxs-lookup"><span data-stu-id="46ea1-146">Int32</span></span>|<span data-ttu-id="46ea1-147">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="46ea1-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="46ea1-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="46ea1-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="46ea1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46ea1-149">DateTimeOffset</span></span>|<span data-ttu-id="46ea1-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="46ea1-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="46ea1-151">status</span><span class="sxs-lookup"><span data-stu-id="46ea1-151">status</span></span>|[<span data-ttu-id="46ea1-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="46ea1-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="46ea1-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="46ea1-153">Compliance status of the policy report.</span></span> <span data-ttu-id="46ea1-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="46ea1-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="46ea1-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="46ea1-155">lastReportedDateTime</span></span>|<span data-ttu-id="46ea1-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46ea1-156">DateTimeOffset</span></span>|<span data-ttu-id="46ea1-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="46ea1-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="46ea1-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46ea1-158">userPrincipalName</span></span>|<span data-ttu-id="46ea1-159">String</span><span class="sxs-lookup"><span data-stu-id="46ea1-159">String</span></span>|<span data-ttu-id="46ea1-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="46ea1-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="46ea1-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="46ea1-161">Response</span></span>
<span data-ttu-id="46ea1-162">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="46ea1-162">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46ea1-163">Пример</span><span class="sxs-lookup"><span data-stu-id="46ea1-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="46ea1-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="46ea1-164">Request</span></span>
<span data-ttu-id="46ea1-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46ea1-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="46ea1-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="46ea1-166">Response</span></span>
<span data-ttu-id="46ea1-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="46ea1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




