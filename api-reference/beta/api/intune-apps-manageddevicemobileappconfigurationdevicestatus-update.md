---
title: Обновление managedDeviceMobileAppConfigurationDeviceStatus
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 301f29fce968c45b3d907d7e8ca15f60913c1cd2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935624"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="01d0d-103">Обновление managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="01d0d-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="01d0d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01d0d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01d0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01d0d-106">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="01d0d-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01d0d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01d0d-107">Prerequisites</span></span>
<span data-ttu-id="01d0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01d0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01d0d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01d0d-110">Permission type</span></span>|<span data-ttu-id="01d0d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01d0d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01d0d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01d0d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01d0d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d0d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01d0d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01d0d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01d0d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d0d-115">Not supported.</span></span>|
|<span data-ttu-id="01d0d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01d0d-116">Application</span></span>|<span data-ttu-id="01d0d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01d0d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01d0d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01d0d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="01d0d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01d0d-119">Request headers</span></span>
|<span data-ttu-id="01d0d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01d0d-120">Header</span></span>|<span data-ttu-id="01d0d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="01d0d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01d0d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01d0d-122">Authorization</span></span>|<span data-ttu-id="01d0d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01d0d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01d0d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="01d0d-124">Accept</span></span>|<span data-ttu-id="01d0d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01d0d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01d0d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01d0d-126">Request body</span></span>
<span data-ttu-id="01d0d-127">В тексте запроса добавьте представление объекта [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01d0d-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="01d0d-128">В следующей таблице приведены свойства, необходимые при создании [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="01d0d-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="01d0d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="01d0d-129">Property</span></span>|<span data-ttu-id="01d0d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="01d0d-130">Type</span></span>|<span data-ttu-id="01d0d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="01d0d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d0d-132">id</span><span class="sxs-lookup"><span data-stu-id="01d0d-132">id</span></span>|<span data-ttu-id="01d0d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="01d0d-133">String</span></span>|<span data-ttu-id="01d0d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01d0d-134">Key of the entity.</span></span>|
|<span data-ttu-id="01d0d-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="01d0d-135">deviceDisplayName</span></span>|<span data-ttu-id="01d0d-136">Строка</span><span class="sxs-lookup"><span data-stu-id="01d0d-136">String</span></span>|<span data-ttu-id="01d0d-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="01d0d-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="01d0d-138">userName</span><span class="sxs-lookup"><span data-stu-id="01d0d-138">userName</span></span>|<span data-ttu-id="01d0d-139">Строка</span><span class="sxs-lookup"><span data-stu-id="01d0d-139">String</span></span>|<span data-ttu-id="01d0d-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="01d0d-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="01d0d-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="01d0d-141">deviceModel</span></span>|<span data-ttu-id="01d0d-142">String</span><span class="sxs-lookup"><span data-stu-id="01d0d-142">String</span></span>|<span data-ttu-id="01d0d-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="01d0d-143">The device model that is being reported</span></span>|
|<span data-ttu-id="01d0d-144">platform</span><span class="sxs-lookup"><span data-stu-id="01d0d-144">platform</span></span>|<span data-ttu-id="01d0d-145">Int32</span><span class="sxs-lookup"><span data-stu-id="01d0d-145">Int32</span></span>|<span data-ttu-id="01d0d-146">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="01d0d-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="01d0d-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="01d0d-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="01d0d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d0d-148">DateTimeOffset</span></span>|<span data-ttu-id="01d0d-149">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="01d0d-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="01d0d-150">status</span><span class="sxs-lookup"><span data-stu-id="01d0d-150">status</span></span>|[<span data-ttu-id="01d0d-151">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="01d0d-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="01d0d-152">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="01d0d-152">Compliance status of the policy report.</span></span> <span data-ttu-id="01d0d-153">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="01d0d-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="01d0d-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="01d0d-154">lastReportedDateTime</span></span>|<span data-ttu-id="01d0d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01d0d-155">DateTimeOffset</span></span>|<span data-ttu-id="01d0d-156">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="01d0d-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="01d0d-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="01d0d-157">userPrincipalName</span></span>|<span data-ttu-id="01d0d-158">String</span><span class="sxs-lookup"><span data-stu-id="01d0d-158">String</span></span>|<span data-ttu-id="01d0d-159">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="01d0d-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="01d0d-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="01d0d-160">Response</span></span>
<span data-ttu-id="01d0d-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01d0d-161">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01d0d-162">Пример</span><span class="sxs-lookup"><span data-stu-id="01d0d-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="01d0d-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="01d0d-163">Request</span></span>
<span data-ttu-id="01d0d-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01d0d-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01d0d-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="01d0d-165">Response</span></span>
<span data-ttu-id="01d0d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01d0d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




