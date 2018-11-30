---
title: Обновление managedDeviceMobileAppConfigurationDeviceStatus
description: Обновление свойства объекта managedDeviceMobileAppConfigurationDeviceStatus.
ms.openlocfilehash: 92f3b2e4b119f1da552d276f4c59b8bdac2e55e3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079020"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="01f39-103">Обновление managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="01f39-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="01f39-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01f39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01f39-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01f39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01f39-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="01f39-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01f39-107">Обновление свойства объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="01f39-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01f39-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01f39-108">Prerequisites</span></span>
<span data-ttu-id="01f39-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01f39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01f39-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01f39-111">Permission type</span></span>|<span data-ttu-id="01f39-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01f39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01f39-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01f39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01f39-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f39-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01f39-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01f39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01f39-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01f39-116">Not supported.</span></span>|
|<span data-ttu-id="01f39-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01f39-117">Application</span></span>|<span data-ttu-id="01f39-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01f39-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01f39-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01f39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="01f39-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01f39-120">Request headers</span></span>
|<span data-ttu-id="01f39-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01f39-121">Header</span></span>|<span data-ttu-id="01f39-122">Значение</span><span class="sxs-lookup"><span data-stu-id="01f39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01f39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01f39-123">Authorization</span></span>|<span data-ttu-id="01f39-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="01f39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01f39-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01f39-125">Accept</span></span>|<span data-ttu-id="01f39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01f39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01f39-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01f39-127">Request body</span></span>
<span data-ttu-id="01f39-128">В тексте запроса укажите представление JSON для объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="01f39-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="01f39-129">В следующей таблице показаны свойства, которые необходимы для создания [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="01f39-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="01f39-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="01f39-130">Property</span></span>|<span data-ttu-id="01f39-131">Тип</span><span class="sxs-lookup"><span data-stu-id="01f39-131">Type</span></span>|<span data-ttu-id="01f39-132">Описание</span><span class="sxs-lookup"><span data-stu-id="01f39-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01f39-133">id</span><span class="sxs-lookup"><span data-stu-id="01f39-133">id</span></span>|<span data-ttu-id="01f39-134">String</span><span class="sxs-lookup"><span data-stu-id="01f39-134">String</span></span>|<span data-ttu-id="01f39-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01f39-135">Key of the entity.</span></span>|
|<span data-ttu-id="01f39-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="01f39-136">deviceDisplayName</span></span>|<span data-ttu-id="01f39-137">String</span><span class="sxs-lookup"><span data-stu-id="01f39-137">String</span></span>|<span data-ttu-id="01f39-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="01f39-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="01f39-139">userName</span><span class="sxs-lookup"><span data-stu-id="01f39-139">userName</span></span>|<span data-ttu-id="01f39-140">String</span><span class="sxs-lookup"><span data-stu-id="01f39-140">String</span></span>|<span data-ttu-id="01f39-141">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="01f39-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="01f39-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="01f39-142">deviceModel</span></span>|<span data-ttu-id="01f39-143">String</span><span class="sxs-lookup"><span data-stu-id="01f39-143">String</span></span>|<span data-ttu-id="01f39-144">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="01f39-144">The device model that is being reported</span></span>|
|<span data-ttu-id="01f39-145">platform</span><span class="sxs-lookup"><span data-stu-id="01f39-145">platform</span></span>|<span data-ttu-id="01f39-146">Int32</span><span class="sxs-lookup"><span data-stu-id="01f39-146">Int32</span></span>|<span data-ttu-id="01f39-147">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="01f39-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="01f39-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="01f39-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="01f39-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01f39-149">DateTimeOffset</span></span>|<span data-ttu-id="01f39-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="01f39-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="01f39-151">status</span><span class="sxs-lookup"><span data-stu-id="01f39-151">status</span></span>|[<span data-ttu-id="01f39-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="01f39-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="01f39-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="01f39-153">Compliance status of the policy report.</span></span> <span data-ttu-id="01f39-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="01f39-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="01f39-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="01f39-155">lastReportedDateTime</span></span>|<span data-ttu-id="01f39-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01f39-156">DateTimeOffset</span></span>|<span data-ttu-id="01f39-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="01f39-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="01f39-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="01f39-158">userPrincipalName</span></span>|<span data-ttu-id="01f39-159">String</span><span class="sxs-lookup"><span data-stu-id="01f39-159">String</span></span>|<span data-ttu-id="01f39-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="01f39-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="01f39-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="01f39-161">Response</span></span>
<span data-ttu-id="01f39-162">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="01f39-162">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01f39-163">Пример</span><span class="sxs-lookup"><span data-stu-id="01f39-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="01f39-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="01f39-164">Request</span></span>
<span data-ttu-id="01f39-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01f39-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 377

{
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

### <a name="response"></a><span data-ttu-id="01f39-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="01f39-166">Response</span></span>
<span data-ttu-id="01f39-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="01f39-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





