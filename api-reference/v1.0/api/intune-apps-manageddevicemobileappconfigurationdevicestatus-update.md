---
title: Обновление managedDeviceMobileAppConfigurationDeviceStatus
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad38a993f9cc216d61f2eeaed38c20625cd094d7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422253"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="772f7-103">Обновление managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="772f7-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="772f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="772f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="772f7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="772f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="772f7-106">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="772f7-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="772f7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="772f7-107">Prerequisites</span></span>
<span data-ttu-id="772f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="772f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="772f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="772f7-110">Permission type</span></span>|<span data-ttu-id="772f7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="772f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="772f7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="772f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="772f7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="772f7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="772f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="772f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="772f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="772f7-115">Not supported.</span></span>|
|<span data-ttu-id="772f7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="772f7-116">Application</span></span>|<span data-ttu-id="772f7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="772f7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="772f7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="772f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="772f7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="772f7-119">Request headers</span></span>
|<span data-ttu-id="772f7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="772f7-120">Header</span></span>|<span data-ttu-id="772f7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="772f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="772f7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="772f7-122">Authorization</span></span>|<span data-ttu-id="772f7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="772f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="772f7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="772f7-124">Accept</span></span>|<span data-ttu-id="772f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="772f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="772f7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="772f7-126">Request body</span></span>
<span data-ttu-id="772f7-127">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="772f7-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="772f7-128">В следующей таблице приведены свойства, необходимые при создании [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="772f7-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="772f7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="772f7-129">Property</span></span>|<span data-ttu-id="772f7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="772f7-130">Type</span></span>|<span data-ttu-id="772f7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="772f7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="772f7-132">id</span><span class="sxs-lookup"><span data-stu-id="772f7-132">id</span></span>|<span data-ttu-id="772f7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="772f7-133">String</span></span>|<span data-ttu-id="772f7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="772f7-134">Key of the entity.</span></span>|
|<span data-ttu-id="772f7-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="772f7-135">deviceDisplayName</span></span>|<span data-ttu-id="772f7-136">String</span><span class="sxs-lookup"><span data-stu-id="772f7-136">String</span></span>|<span data-ttu-id="772f7-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="772f7-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="772f7-138">userName</span><span class="sxs-lookup"><span data-stu-id="772f7-138">userName</span></span>|<span data-ttu-id="772f7-139">String</span><span class="sxs-lookup"><span data-stu-id="772f7-139">String</span></span>|<span data-ttu-id="772f7-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="772f7-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="772f7-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="772f7-141">deviceModel</span></span>|<span data-ttu-id="772f7-142">String</span><span class="sxs-lookup"><span data-stu-id="772f7-142">String</span></span>|<span data-ttu-id="772f7-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="772f7-143">The device model that is being reported</span></span>|
|<span data-ttu-id="772f7-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="772f7-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="772f7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="772f7-145">DateTimeOffset</span></span>|<span data-ttu-id="772f7-146">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="772f7-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="772f7-147">status</span><span class="sxs-lookup"><span data-stu-id="772f7-147">status</span></span>|[<span data-ttu-id="772f7-148">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="772f7-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="772f7-149">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="772f7-149">Compliance status of the policy report.</span></span> <span data-ttu-id="772f7-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="772f7-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="772f7-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="772f7-151">lastReportedDateTime</span></span>|<span data-ttu-id="772f7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="772f7-152">DateTimeOffset</span></span>|<span data-ttu-id="772f7-153">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="772f7-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="772f7-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="772f7-154">userPrincipalName</span></span>|<span data-ttu-id="772f7-155">String</span><span class="sxs-lookup"><span data-stu-id="772f7-155">String</span></span>|<span data-ttu-id="772f7-156">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="772f7-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="772f7-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="772f7-157">Response</span></span>
<span data-ttu-id="772f7-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="772f7-158">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="772f7-159">Пример</span><span class="sxs-lookup"><span data-stu-id="772f7-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="772f7-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="772f7-160">Request</span></span>
<span data-ttu-id="772f7-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="772f7-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="772f7-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="772f7-162">Response</span></span>
<span data-ttu-id="772f7-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="772f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






