---
title: Обновление managedDeviceMobileAppConfigurationDeviceStatus
description: Обновление свойства объекта managedDeviceMobileAppConfigurationDeviceStatus.
ms.openlocfilehash: d81d8efac6e4b6f658fb7ebc6529ce1abfed38f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027528"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="9afcf-103">Обновление managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="9afcf-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="9afcf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9afcf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9afcf-105">Обновление свойства объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="9afcf-105">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9afcf-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9afcf-106">Prerequisites</span></span>
<span data-ttu-id="9afcf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9afcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9afcf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9afcf-109">Permission type</span></span>|<span data-ttu-id="9afcf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9afcf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9afcf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9afcf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9afcf-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9afcf-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9afcf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9afcf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9afcf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9afcf-114">Not supported.</span></span>|
|<span data-ttu-id="9afcf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9afcf-115">Application</span></span>|<span data-ttu-id="9afcf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9afcf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9afcf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9afcf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="9afcf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9afcf-118">Request headers</span></span>
|<span data-ttu-id="9afcf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9afcf-119">Header</span></span>|<span data-ttu-id="9afcf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9afcf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9afcf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9afcf-121">Authorization</span></span>|<span data-ttu-id="9afcf-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9afcf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9afcf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9afcf-123">Accept</span></span>|<span data-ttu-id="9afcf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9afcf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9afcf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9afcf-125">Request body</span></span>
<span data-ttu-id="9afcf-126">В тексте запроса укажите представление JSON для объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="9afcf-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="9afcf-127">В следующей таблице показаны свойства, которые необходимы для создания [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9afcf-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="9afcf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9afcf-128">Property</span></span>|<span data-ttu-id="9afcf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9afcf-129">Type</span></span>|<span data-ttu-id="9afcf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9afcf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9afcf-131">id</span><span class="sxs-lookup"><span data-stu-id="9afcf-131">id</span></span>|<span data-ttu-id="9afcf-132">String</span><span class="sxs-lookup"><span data-stu-id="9afcf-132">String</span></span>|<span data-ttu-id="9afcf-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9afcf-133">Key of the entity.</span></span>|
|<span data-ttu-id="9afcf-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9afcf-134">deviceDisplayName</span></span>|<span data-ttu-id="9afcf-135">String</span><span class="sxs-lookup"><span data-stu-id="9afcf-135">String</span></span>|<span data-ttu-id="9afcf-136">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="9afcf-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="9afcf-137">userName</span><span class="sxs-lookup"><span data-stu-id="9afcf-137">userName</span></span>|<span data-ttu-id="9afcf-138">String</span><span class="sxs-lookup"><span data-stu-id="9afcf-138">String</span></span>|<span data-ttu-id="9afcf-139">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="9afcf-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="9afcf-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9afcf-140">deviceModel</span></span>|<span data-ttu-id="9afcf-141">String</span><span class="sxs-lookup"><span data-stu-id="9afcf-141">String</span></span>|<span data-ttu-id="9afcf-142">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="9afcf-142">The device model that is being reported</span></span>|
|<span data-ttu-id="9afcf-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9afcf-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9afcf-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9afcf-144">DateTimeOffset</span></span>|<span data-ttu-id="9afcf-145">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9afcf-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="9afcf-146">status</span><span class="sxs-lookup"><span data-stu-id="9afcf-146">status</span></span>|[<span data-ttu-id="9afcf-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9afcf-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9afcf-148">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="9afcf-148">Compliance status of the policy report.</span></span> <span data-ttu-id="9afcf-149">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="9afcf-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9afcf-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="9afcf-150">lastReportedDateTime</span></span>|<span data-ttu-id="9afcf-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9afcf-151">DateTimeOffset</span></span>|<span data-ttu-id="9afcf-152">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="9afcf-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="9afcf-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9afcf-153">userPrincipalName</span></span>|<span data-ttu-id="9afcf-154">String</span><span class="sxs-lookup"><span data-stu-id="9afcf-154">String</span></span>|<span data-ttu-id="9afcf-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="9afcf-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="9afcf-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="9afcf-156">Response</span></span>
<span data-ttu-id="9afcf-157">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9afcf-157">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9afcf-158">Пример</span><span class="sxs-lookup"><span data-stu-id="9afcf-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="9afcf-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="9afcf-159">Request</span></span>
<span data-ttu-id="9afcf-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9afcf-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="9afcf-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="9afcf-161">Response</span></span>
<span data-ttu-id="9afcf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9afcf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



