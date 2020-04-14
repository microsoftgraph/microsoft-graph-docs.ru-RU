---
title: Обновление managedDeviceMobileAppConfigurationDeviceStatus
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d8cd4174557e9eab934ba6e321c3d68a8b83b29c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43405811"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="09cb7-103">Обновление managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="09cb7-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="09cb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09cb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09cb7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09cb7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09cb7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09cb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09cb7-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="09cb7-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09cb7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="09cb7-108">Prerequisites</span></span>
<span data-ttu-id="09cb7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09cb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09cb7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09cb7-111">Permission type</span></span>|<span data-ttu-id="09cb7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09cb7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09cb7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09cb7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09cb7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09cb7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="09cb7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09cb7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09cb7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09cb7-116">Not supported.</span></span>|
|<span data-ttu-id="09cb7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="09cb7-117">Application</span></span>|<span data-ttu-id="09cb7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09cb7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09cb7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09cb7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="09cb7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="09cb7-120">Request headers</span></span>
|<span data-ttu-id="09cb7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09cb7-121">Header</span></span>|<span data-ttu-id="09cb7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="09cb7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09cb7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09cb7-123">Authorization</span></span>|<span data-ttu-id="09cb7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09cb7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09cb7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="09cb7-125">Accept</span></span>|<span data-ttu-id="09cb7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09cb7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09cb7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09cb7-127">Request body</span></span>
<span data-ttu-id="09cb7-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09cb7-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="09cb7-129">В следующей таблице приведены свойства, необходимые при создании [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="09cb7-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="09cb7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="09cb7-130">Property</span></span>|<span data-ttu-id="09cb7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="09cb7-131">Type</span></span>|<span data-ttu-id="09cb7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="09cb7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09cb7-133">id</span><span class="sxs-lookup"><span data-stu-id="09cb7-133">id</span></span>|<span data-ttu-id="09cb7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="09cb7-134">String</span></span>|<span data-ttu-id="09cb7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="09cb7-135">Key of the entity.</span></span>|
|<span data-ttu-id="09cb7-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="09cb7-136">deviceDisplayName</span></span>|<span data-ttu-id="09cb7-137">String</span><span class="sxs-lookup"><span data-stu-id="09cb7-137">String</span></span>|<span data-ttu-id="09cb7-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="09cb7-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="09cb7-139">userName</span><span class="sxs-lookup"><span data-stu-id="09cb7-139">userName</span></span>|<span data-ttu-id="09cb7-140">String</span><span class="sxs-lookup"><span data-stu-id="09cb7-140">String</span></span>|<span data-ttu-id="09cb7-141">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="09cb7-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="09cb7-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="09cb7-142">deviceModel</span></span>|<span data-ttu-id="09cb7-143">String</span><span class="sxs-lookup"><span data-stu-id="09cb7-143">String</span></span>|<span data-ttu-id="09cb7-144">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="09cb7-144">The device model that is being reported</span></span>|
|<span data-ttu-id="09cb7-145">platform</span><span class="sxs-lookup"><span data-stu-id="09cb7-145">platform</span></span>|<span data-ttu-id="09cb7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="09cb7-146">Int32</span></span>|<span data-ttu-id="09cb7-147">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="09cb7-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="09cb7-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="09cb7-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="09cb7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09cb7-149">DateTimeOffset</span></span>|<span data-ttu-id="09cb7-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="09cb7-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="09cb7-151">status</span><span class="sxs-lookup"><span data-stu-id="09cb7-151">status</span></span>|[<span data-ttu-id="09cb7-152">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="09cb7-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="09cb7-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="09cb7-153">Compliance status of the policy report.</span></span> <span data-ttu-id="09cb7-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="09cb7-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="09cb7-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="09cb7-155">lastReportedDateTime</span></span>|<span data-ttu-id="09cb7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09cb7-156">DateTimeOffset</span></span>|<span data-ttu-id="09cb7-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="09cb7-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="09cb7-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="09cb7-158">userPrincipalName</span></span>|<span data-ttu-id="09cb7-159">String</span><span class="sxs-lookup"><span data-stu-id="09cb7-159">String</span></span>|<span data-ttu-id="09cb7-160">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="09cb7-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="09cb7-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="09cb7-161">Response</span></span>
<span data-ttu-id="09cb7-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09cb7-162">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09cb7-163">Пример</span><span class="sxs-lookup"><span data-stu-id="09cb7-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="09cb7-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="09cb7-164">Request</span></span>
<span data-ttu-id="09cb7-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09cb7-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="09cb7-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="09cb7-166">Response</span></span>
<span data-ttu-id="09cb7-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09cb7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



