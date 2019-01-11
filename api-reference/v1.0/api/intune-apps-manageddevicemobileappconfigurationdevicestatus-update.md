---
title: Обновление managedDeviceMobileAppConfigurationDeviceStatus
description: Обновление свойства объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2a5d0e7a2f7bf148889b6e090a8af8a1a985cf75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855981"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="1b0d1-103">Обновление managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="1b0d1-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="1b0d1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b0d1-105">Обновление свойства объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="1b0d1-105">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b0d1-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1b0d1-106">Prerequisites</span></span>
<span data-ttu-id="1b0d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b0d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b0d1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b0d1-109">Permission type</span></span>|<span data-ttu-id="1b0d1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b0d1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b0d1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b0d1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b0d1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b0d1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b0d1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b0d1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b0d1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-114">Not supported.</span></span>|
|<span data-ttu-id="1b0d1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b0d1-115">Application</span></span>|<span data-ttu-id="1b0d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b0d1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b0d1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1b0d1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b0d1-118">Request headers</span></span>
|<span data-ttu-id="1b0d1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b0d1-119">Header</span></span>|<span data-ttu-id="1b0d1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1b0d1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b0d1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b0d1-121">Authorization</span></span>|<span data-ttu-id="1b0d1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1b0d1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b0d1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1b0d1-123">Accept</span></span>|<span data-ttu-id="1b0d1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1b0d1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b0d1-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b0d1-125">Request body</span></span>
<span data-ttu-id="1b0d1-126">В тексте запроса укажите представление JSON для объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="1b0d1-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="1b0d1-127">В следующей таблице показаны свойства, которые необходимы для создания [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="1b0d1-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="1b0d1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b0d1-128">Property</span></span>|<span data-ttu-id="1b0d1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1b0d1-129">Type</span></span>|<span data-ttu-id="1b0d1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1b0d1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b0d1-131">id</span><span class="sxs-lookup"><span data-stu-id="1b0d1-131">id</span></span>|<span data-ttu-id="1b0d1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="1b0d1-132">String</span></span>|<span data-ttu-id="1b0d1-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-133">Key of the entity.</span></span>|
|<span data-ttu-id="1b0d1-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1b0d1-134">deviceDisplayName</span></span>|<span data-ttu-id="1b0d1-135">String</span><span class="sxs-lookup"><span data-stu-id="1b0d1-135">String</span></span>|<span data-ttu-id="1b0d1-136">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="1b0d1-137">userName</span><span class="sxs-lookup"><span data-stu-id="1b0d1-137">userName</span></span>|<span data-ttu-id="1b0d1-138">String</span><span class="sxs-lookup"><span data-stu-id="1b0d1-138">String</span></span>|<span data-ttu-id="1b0d1-139">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="1b0d1-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1b0d1-140">deviceModel</span></span>|<span data-ttu-id="1b0d1-141">String</span><span class="sxs-lookup"><span data-stu-id="1b0d1-141">String</span></span>|<span data-ttu-id="1b0d1-142">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-142">The device model that is being reported</span></span>|
|<span data-ttu-id="1b0d1-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0d1-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1b0d1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0d1-144">DateTimeOffset</span></span>|<span data-ttu-id="1b0d1-145">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="1b0d1-146">status</span><span class="sxs-lookup"><span data-stu-id="1b0d1-146">status</span></span>|[<span data-ttu-id="1b0d1-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1b0d1-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1b0d1-148">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-148">Compliance status of the policy report.</span></span> <span data-ttu-id="1b0d1-149">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1b0d1-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0d1-150">lastReportedDateTime</span></span>|<span data-ttu-id="1b0d1-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0d1-151">DateTimeOffset</span></span>|<span data-ttu-id="1b0d1-152">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="1b0d1-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1b0d1-153">userPrincipalName</span></span>|<span data-ttu-id="1b0d1-154">String</span><span class="sxs-lookup"><span data-stu-id="1b0d1-154">String</span></span>|<span data-ttu-id="1b0d1-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="1b0d1-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b0d1-156">Response</span></span>
<span data-ttu-id="1b0d1-157">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-157">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b0d1-158">Пример</span><span class="sxs-lookup"><span data-stu-id="1b0d1-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b0d1-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b0d1-159">Request</span></span>
<span data-ttu-id="1b0d1-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b0d1-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b0d1-161">Response</span></span>
<span data-ttu-id="1b0d1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



