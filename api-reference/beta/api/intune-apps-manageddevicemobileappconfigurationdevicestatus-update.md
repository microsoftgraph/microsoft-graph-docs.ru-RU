---
title: Обновление managedDeviceMobileAppConfigurationDeviceStatus
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3cf6a28de7b43bf834554291dc371eb6450be968
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445129"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="6f6c9-103">Обновление managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="6f6c9-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="6f6c9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6f6c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f6c9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f6c9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f6c9-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="6f6c9-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f6c9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6f6c9-108">Prerequisites</span></span>
<span data-ttu-id="6f6c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f6c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f6c9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f6c9-111">Permission type</span></span>|<span data-ttu-id="6f6c9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f6c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f6c9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f6c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f6c9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f6c9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6f6c9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f6c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f6c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-116">Not supported.</span></span>|
|<span data-ttu-id="6f6c9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f6c9-117">Application</span></span>|<span data-ttu-id="6f6c9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f6c9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f6c9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f6c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="6f6c9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6f6c9-120">Request headers</span></span>
|<span data-ttu-id="6f6c9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f6c9-121">Header</span></span>|<span data-ttu-id="6f6c9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6f6c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f6c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f6c9-123">Authorization</span></span>|<span data-ttu-id="6f6c9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f6c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f6c9-125">Accept</span></span>|<span data-ttu-id="6f6c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f6c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f6c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f6c9-127">Request body</span></span>
<span data-ttu-id="6f6c9-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="6f6c9-129">В следующей таблице приведены свойства, необходимые при создании [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="6f6c9-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="6f6c9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f6c9-130">Property</span></span>|<span data-ttu-id="6f6c9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6f6c9-131">Type</span></span>|<span data-ttu-id="6f6c9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6f6c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f6c9-133">id</span><span class="sxs-lookup"><span data-stu-id="6f6c9-133">id</span></span>|<span data-ttu-id="6f6c9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6f6c9-134">String</span></span>|<span data-ttu-id="6f6c9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-135">Key of the entity.</span></span>|
|<span data-ttu-id="6f6c9-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6f6c9-136">deviceDisplayName</span></span>|<span data-ttu-id="6f6c9-137">String</span><span class="sxs-lookup"><span data-stu-id="6f6c9-137">String</span></span>|<span data-ttu-id="6f6c9-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="6f6c9-139">userName</span><span class="sxs-lookup"><span data-stu-id="6f6c9-139">userName</span></span>|<span data-ttu-id="6f6c9-140">String</span><span class="sxs-lookup"><span data-stu-id="6f6c9-140">String</span></span>|<span data-ttu-id="6f6c9-141">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="6f6c9-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="6f6c9-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6f6c9-142">deviceModel</span></span>|<span data-ttu-id="6f6c9-143">String</span><span class="sxs-lookup"><span data-stu-id="6f6c9-143">String</span></span>|<span data-ttu-id="6f6c9-144">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="6f6c9-144">The device model that is being reported</span></span>|
|<span data-ttu-id="6f6c9-145">platform</span><span class="sxs-lookup"><span data-stu-id="6f6c9-145">platform</span></span>|<span data-ttu-id="6f6c9-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6f6c9-146">Int32</span></span>|<span data-ttu-id="6f6c9-147">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="6f6c9-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="6f6c9-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6f6c9-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6f6c9-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f6c9-149">DateTimeOffset</span></span>|<span data-ttu-id="6f6c9-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="6f6c9-151">status</span><span class="sxs-lookup"><span data-stu-id="6f6c9-151">status</span></span>|[<span data-ttu-id="6f6c9-152">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="6f6c9-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6f6c9-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-153">Compliance status of the policy report.</span></span> <span data-ttu-id="6f6c9-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6f6c9-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f6c9-155">lastReportedDateTime</span></span>|<span data-ttu-id="6f6c9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f6c9-156">DateTimeOffset</span></span>|<span data-ttu-id="6f6c9-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="6f6c9-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6f6c9-158">userPrincipalName</span></span>|<span data-ttu-id="6f6c9-159">String</span><span class="sxs-lookup"><span data-stu-id="6f6c9-159">String</span></span>|<span data-ttu-id="6f6c9-160">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="6f6c9-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f6c9-161">Response</span></span>
<span data-ttu-id="6f6c9-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-162">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f6c9-163">Пример</span><span class="sxs-lookup"><span data-stu-id="6f6c9-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f6c9-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f6c9-164">Request</span></span>
<span data-ttu-id="6f6c9-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 463

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
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

### <a name="response"></a><span data-ttu-id="6f6c9-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f6c9-166">Response</span></span>
<span data-ttu-id="6f6c9-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f6c9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
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





