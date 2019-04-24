---
title: Обновление managedDeviceMobileAppConfigurationDeviceStatus
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0732c53a076081c35a836e7d34ed4b2427026e4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32493288"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="9c0a6-103">Обновление managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="9c0a6-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="9c0a6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c0a6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c0a6-106">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="9c0a6-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c0a6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9c0a6-107">Prerequisites</span></span>
<span data-ttu-id="9c0a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c0a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c0a6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c0a6-110">Permission type</span></span>|<span data-ttu-id="9c0a6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c0a6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c0a6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c0a6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c0a6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c0a6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9c0a6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c0a6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c0a6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-115">Not supported.</span></span>|
|<span data-ttu-id="9c0a6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c0a6-116">Application</span></span>|<span data-ttu-id="9c0a6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c0a6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c0a6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="9c0a6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c0a6-119">Request headers</span></span>
|<span data-ttu-id="9c0a6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c0a6-120">Header</span></span>|<span data-ttu-id="9c0a6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9c0a6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c0a6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c0a6-122">Authorization</span></span>|<span data-ttu-id="9c0a6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c0a6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9c0a6-124">Accept</span></span>|<span data-ttu-id="9c0a6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c0a6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c0a6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c0a6-126">Request body</span></span>
<span data-ttu-id="9c0a6-127">В тексте запроса добавьте представление объекта [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="9c0a6-128">В следующей таблице приведены свойства, необходимые при создании [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9c0a6-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="9c0a6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c0a6-129">Property</span></span>|<span data-ttu-id="9c0a6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9c0a6-130">Type</span></span>|<span data-ttu-id="9c0a6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9c0a6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c0a6-132">id</span><span class="sxs-lookup"><span data-stu-id="9c0a6-132">id</span></span>|<span data-ttu-id="9c0a6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9c0a6-133">String</span></span>|<span data-ttu-id="9c0a6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-134">Key of the entity.</span></span>|
|<span data-ttu-id="9c0a6-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9c0a6-135">deviceDisplayName</span></span>|<span data-ttu-id="9c0a6-136">String</span><span class="sxs-lookup"><span data-stu-id="9c0a6-136">String</span></span>|<span data-ttu-id="9c0a6-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="9c0a6-138">userName</span><span class="sxs-lookup"><span data-stu-id="9c0a6-138">userName</span></span>|<span data-ttu-id="9c0a6-139">String</span><span class="sxs-lookup"><span data-stu-id="9c0a6-139">String</span></span>|<span data-ttu-id="9c0a6-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="9c0a6-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="9c0a6-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9c0a6-141">deviceModel</span></span>|<span data-ttu-id="9c0a6-142">String</span><span class="sxs-lookup"><span data-stu-id="9c0a6-142">String</span></span>|<span data-ttu-id="9c0a6-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="9c0a6-143">The device model that is being reported</span></span>|
|<span data-ttu-id="9c0a6-144">platform</span><span class="sxs-lookup"><span data-stu-id="9c0a6-144">platform</span></span>|<span data-ttu-id="9c0a6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="9c0a6-145">Int32</span></span>|<span data-ttu-id="9c0a6-146">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="9c0a6-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="9c0a6-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9c0a6-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9c0a6-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c0a6-148">DateTimeOffset</span></span>|<span data-ttu-id="9c0a6-149">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="9c0a6-150">status</span><span class="sxs-lookup"><span data-stu-id="9c0a6-150">status</span></span>|[<span data-ttu-id="9c0a6-151">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="9c0a6-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9c0a6-152">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-152">Compliance status of the policy report.</span></span> <span data-ttu-id="9c0a6-153">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9c0a6-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c0a6-154">lastReportedDateTime</span></span>|<span data-ttu-id="9c0a6-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c0a6-155">DateTimeOffset</span></span>|<span data-ttu-id="9c0a6-156">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="9c0a6-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9c0a6-157">userPrincipalName</span></span>|<span data-ttu-id="9c0a6-158">String</span><span class="sxs-lookup"><span data-stu-id="9c0a6-158">String</span></span>|<span data-ttu-id="9c0a6-159">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="9c0a6-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c0a6-160">Response</span></span>
<span data-ttu-id="9c0a6-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-161">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c0a6-162">Пример</span><span class="sxs-lookup"><span data-stu-id="9c0a6-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c0a6-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c0a6-163">Request</span></span>
<span data-ttu-id="9c0a6-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c0a6-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c0a6-165">Response</span></span>
<span data-ttu-id="9c0a6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c0a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





