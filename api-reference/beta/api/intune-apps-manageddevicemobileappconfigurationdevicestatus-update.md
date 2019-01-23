---
title: Обновление managedDeviceMobileAppConfigurationDeviceStatus
description: Обновление свойства объекта managedDeviceMobileAppConfigurationDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 56394f7825d180391723ffc722d58200dba9069d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397794"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="a57ac-103">Обновление managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a57ac-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="a57ac-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a57ac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a57ac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a57ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a57ac-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a57ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a57ac-107">Обновление свойства объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="a57ac-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a57ac-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="a57ac-108">Prerequisites</span></span>
<span data-ttu-id="a57ac-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a57ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a57ac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a57ac-111">Permission type</span></span>|<span data-ttu-id="a57ac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a57ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a57ac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a57ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a57ac-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a57ac-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a57ac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a57ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a57ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a57ac-116">Not supported.</span></span>|
|<span data-ttu-id="a57ac-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a57ac-117">Application</span></span>|<span data-ttu-id="a57ac-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a57ac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a57ac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a57ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="a57ac-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a57ac-120">Request headers</span></span>
|<span data-ttu-id="a57ac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a57ac-121">Header</span></span>|<span data-ttu-id="a57ac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a57ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a57ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a57ac-123">Authorization</span></span>|<span data-ttu-id="a57ac-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a57ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a57ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a57ac-125">Accept</span></span>|<span data-ttu-id="a57ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a57ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a57ac-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a57ac-127">Request body</span></span>
<span data-ttu-id="a57ac-128">В тексте запроса укажите представление JSON для объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="a57ac-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="a57ac-129">В следующей таблице показаны свойства, которые необходимы для создания [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a57ac-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="a57ac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a57ac-130">Property</span></span>|<span data-ttu-id="a57ac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a57ac-131">Type</span></span>|<span data-ttu-id="a57ac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a57ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a57ac-133">id</span><span class="sxs-lookup"><span data-stu-id="a57ac-133">id</span></span>|<span data-ttu-id="a57ac-134">String</span><span class="sxs-lookup"><span data-stu-id="a57ac-134">String</span></span>|<span data-ttu-id="a57ac-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a57ac-135">Key of the entity.</span></span>|
|<span data-ttu-id="a57ac-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a57ac-136">deviceDisplayName</span></span>|<span data-ttu-id="a57ac-137">String</span><span class="sxs-lookup"><span data-stu-id="a57ac-137">String</span></span>|<span data-ttu-id="a57ac-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="a57ac-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a57ac-139">userName</span><span class="sxs-lookup"><span data-stu-id="a57ac-139">userName</span></span>|<span data-ttu-id="a57ac-140">String</span><span class="sxs-lookup"><span data-stu-id="a57ac-140">String</span></span>|<span data-ttu-id="a57ac-141">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="a57ac-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="a57ac-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a57ac-142">deviceModel</span></span>|<span data-ttu-id="a57ac-143">String</span><span class="sxs-lookup"><span data-stu-id="a57ac-143">String</span></span>|<span data-ttu-id="a57ac-144">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="a57ac-144">The device model that is being reported</span></span>|
|<span data-ttu-id="a57ac-145">platform</span><span class="sxs-lookup"><span data-stu-id="a57ac-145">platform</span></span>|<span data-ttu-id="a57ac-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a57ac-146">Int32</span></span>|<span data-ttu-id="a57ac-147">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="a57ac-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="a57ac-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a57ac-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a57ac-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a57ac-149">DateTimeOffset</span></span>|<span data-ttu-id="a57ac-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a57ac-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a57ac-151">status</span><span class="sxs-lookup"><span data-stu-id="a57ac-151">status</span></span>|[<span data-ttu-id="a57ac-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a57ac-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a57ac-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="a57ac-153">Compliance status of the policy report.</span></span> <span data-ttu-id="a57ac-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a57ac-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a57ac-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a57ac-155">lastReportedDateTime</span></span>|<span data-ttu-id="a57ac-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a57ac-156">DateTimeOffset</span></span>|<span data-ttu-id="a57ac-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="a57ac-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a57ac-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a57ac-158">userPrincipalName</span></span>|<span data-ttu-id="a57ac-159">String</span><span class="sxs-lookup"><span data-stu-id="a57ac-159">String</span></span>|<span data-ttu-id="a57ac-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a57ac-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="a57ac-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="a57ac-161">Response</span></span>
<span data-ttu-id="a57ac-162">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a57ac-162">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a57ac-163">Пример</span><span class="sxs-lookup"><span data-stu-id="a57ac-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a57ac-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="a57ac-164">Request</span></span>
<span data-ttu-id="a57ac-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a57ac-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a57ac-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="a57ac-166">Response</span></span>
<span data-ttu-id="a57ac-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a57ac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




