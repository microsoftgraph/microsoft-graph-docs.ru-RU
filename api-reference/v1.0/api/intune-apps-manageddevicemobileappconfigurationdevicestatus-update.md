---
title: Обновление managedDeviceMobileAppConfigurationDeviceStatus
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: efb70f7a7dfc0be9d0c1f1a0bf882b52d15fd4bd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "37355325"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="d474d-103">Обновление managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d474d-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="d474d-104">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d474d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d474d-105">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="d474d-105">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d474d-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d474d-106">Prerequisites</span></span>
<span data-ttu-id="d474d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d474d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d474d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d474d-109">Permission type</span></span>|<span data-ttu-id="d474d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d474d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d474d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d474d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d474d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d474d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d474d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d474d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d474d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d474d-114">Not supported.</span></span>|
|<span data-ttu-id="d474d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d474d-115">Application</span></span>|<span data-ttu-id="d474d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d474d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d474d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d474d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="d474d-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d474d-118">Request headers</span></span>
|<span data-ttu-id="d474d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d474d-119">Header</span></span>|<span data-ttu-id="d474d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d474d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d474d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d474d-121">Authorization</span></span>|<span data-ttu-id="d474d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d474d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d474d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d474d-123">Accept</span></span>|<span data-ttu-id="d474d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d474d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d474d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d474d-125">Request body</span></span>
<span data-ttu-id="d474d-126">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d474d-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="d474d-127">В следующей таблице приведены свойства, необходимые при создании [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d474d-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="d474d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d474d-128">Property</span></span>|<span data-ttu-id="d474d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d474d-129">Type</span></span>|<span data-ttu-id="d474d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d474d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d474d-131">id</span><span class="sxs-lookup"><span data-stu-id="d474d-131">id</span></span>|<span data-ttu-id="d474d-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d474d-132">String</span></span>|<span data-ttu-id="d474d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d474d-133">Key of the entity.</span></span>|
|<span data-ttu-id="d474d-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d474d-134">deviceDisplayName</span></span>|<span data-ttu-id="d474d-135">String</span><span class="sxs-lookup"><span data-stu-id="d474d-135">String</span></span>|<span data-ttu-id="d474d-136">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="d474d-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="d474d-137">userName</span><span class="sxs-lookup"><span data-stu-id="d474d-137">userName</span></span>|<span data-ttu-id="d474d-138">String</span><span class="sxs-lookup"><span data-stu-id="d474d-138">String</span></span>|<span data-ttu-id="d474d-139">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="d474d-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="d474d-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d474d-140">deviceModel</span></span>|<span data-ttu-id="d474d-141">String</span><span class="sxs-lookup"><span data-stu-id="d474d-141">String</span></span>|<span data-ttu-id="d474d-142">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="d474d-142">The device model that is being reported</span></span>|
|<span data-ttu-id="d474d-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d474d-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d474d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d474d-144">DateTimeOffset</span></span>|<span data-ttu-id="d474d-145">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d474d-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="d474d-146">status</span><span class="sxs-lookup"><span data-stu-id="d474d-146">status</span></span>|[<span data-ttu-id="d474d-147">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="d474d-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d474d-148">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="d474d-148">Compliance status of the policy report.</span></span> <span data-ttu-id="d474d-149">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d474d-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d474d-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d474d-150">lastReportedDateTime</span></span>|<span data-ttu-id="d474d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d474d-151">DateTimeOffset</span></span>|<span data-ttu-id="d474d-152">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="d474d-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="d474d-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d474d-153">userPrincipalName</span></span>|<span data-ttu-id="d474d-154">String</span><span class="sxs-lookup"><span data-stu-id="d474d-154">String</span></span>|<span data-ttu-id="d474d-155">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="d474d-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="d474d-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="d474d-156">Response</span></span>
<span data-ttu-id="d474d-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d474d-157">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d474d-158">Пример</span><span class="sxs-lookup"><span data-stu-id="d474d-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="d474d-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="d474d-159">Request</span></span>
<span data-ttu-id="d474d-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d474d-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d474d-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="d474d-161">Response</span></span>
<span data-ttu-id="d474d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d474d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




