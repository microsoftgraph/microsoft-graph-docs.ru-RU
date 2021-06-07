---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c41b8f777784ce7d10f591456b0511bea903a8c6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747944"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="6aa17-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="6aa17-103">Update iosUpdateDeviceStatus</span></span>

<span data-ttu-id="6aa17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aa17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6aa17-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6aa17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aa17-106">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="6aa17-106">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6aa17-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa17-107">Prerequisites</span></span>
<span data-ttu-id="6aa17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aa17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aa17-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa17-110">Permission type</span></span>|<span data-ttu-id="6aa17-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aa17-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aa17-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aa17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6aa17-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aa17-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6aa17-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aa17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aa17-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa17-115">Not supported.</span></span>|
|<span data-ttu-id="6aa17-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6aa17-116">Application</span></span>|<span data-ttu-id="6aa17-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aa17-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aa17-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6aa17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="6aa17-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6aa17-119">Request headers</span></span>
|<span data-ttu-id="6aa17-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6aa17-120">Header</span></span>|<span data-ttu-id="6aa17-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6aa17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aa17-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aa17-122">Authorization</span></span>|<span data-ttu-id="6aa17-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6aa17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aa17-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6aa17-124">Accept</span></span>|<span data-ttu-id="6aa17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6aa17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aa17-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6aa17-126">Request body</span></span>
<span data-ttu-id="6aa17-127">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6aa17-127">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="6aa17-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="6aa17-128">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="6aa17-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6aa17-129">Property</span></span>|<span data-ttu-id="6aa17-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6aa17-130">Type</span></span>|<span data-ttu-id="6aa17-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6aa17-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aa17-132">id</span><span class="sxs-lookup"><span data-stu-id="6aa17-132">id</span></span>|<span data-ttu-id="6aa17-133">String</span><span class="sxs-lookup"><span data-stu-id="6aa17-133">String</span></span>|<span data-ttu-id="6aa17-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6aa17-134">Key of the entity.</span></span>|
|<span data-ttu-id="6aa17-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="6aa17-135">installStatus</span></span>|[<span data-ttu-id="6aa17-136">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="6aa17-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="6aa17-137">Состояние установки отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="6aa17-137">The installation status of the policy report.</span></span> <span data-ttu-id="6aa17-138">Возможные значения: `success` `available` , , , , `idle` , `unknown` , `downloading` `downloadFailed` `downloadRequiresComputer` , `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installing` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation` `sharedDeviceUserLoggedInError` `deviceOsHigherThanDesiredOsVersion` .</span><span class="sxs-lookup"><span data-stu-id="6aa17-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`, `deviceOsHigherThanDesiredOsVersion`.</span></span>|
|<span data-ttu-id="6aa17-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="6aa17-139">osVersion</span></span>|<span data-ttu-id="6aa17-140">String</span><span class="sxs-lookup"><span data-stu-id="6aa17-140">String</span></span>|<span data-ttu-id="6aa17-141">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="6aa17-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="6aa17-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="6aa17-142">deviceId</span></span>|<span data-ttu-id="6aa17-143">String</span><span class="sxs-lookup"><span data-stu-id="6aa17-143">String</span></span>|<span data-ttu-id="6aa17-144">ИД устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="6aa17-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="6aa17-145">userId</span><span class="sxs-lookup"><span data-stu-id="6aa17-145">userId</span></span>|<span data-ttu-id="6aa17-146">String</span><span class="sxs-lookup"><span data-stu-id="6aa17-146">String</span></span>|<span data-ttu-id="6aa17-147">ИД пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="6aa17-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="6aa17-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6aa17-148">deviceDisplayName</span></span>|<span data-ttu-id="6aa17-149">String</span><span class="sxs-lookup"><span data-stu-id="6aa17-149">String</span></span>|<span data-ttu-id="6aa17-150">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="6aa17-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="6aa17-151">userName</span><span class="sxs-lookup"><span data-stu-id="6aa17-151">userName</span></span>|<span data-ttu-id="6aa17-152">String</span><span class="sxs-lookup"><span data-stu-id="6aa17-152">String</span></span>|<span data-ttu-id="6aa17-153">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="6aa17-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="6aa17-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6aa17-154">deviceModel</span></span>|<span data-ttu-id="6aa17-155">String</span><span class="sxs-lookup"><span data-stu-id="6aa17-155">String</span></span>|<span data-ttu-id="6aa17-156">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="6aa17-156">The device model that is being reported</span></span>|
|<span data-ttu-id="6aa17-157">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6aa17-157">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6aa17-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aa17-158">DateTimeOffset</span></span>|<span data-ttu-id="6aa17-159">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6aa17-159">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="6aa17-160">status</span><span class="sxs-lookup"><span data-stu-id="6aa17-160">status</span></span>|[<span data-ttu-id="6aa17-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6aa17-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6aa17-162">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="6aa17-162">Compliance status of the policy report.</span></span> <span data-ttu-id="6aa17-163">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6aa17-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6aa17-164">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6aa17-164">lastReportedDateTime</span></span>|<span data-ttu-id="6aa17-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aa17-165">DateTimeOffset</span></span>|<span data-ttu-id="6aa17-166">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="6aa17-166">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="6aa17-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6aa17-167">userPrincipalName</span></span>|<span data-ttu-id="6aa17-168">String</span><span class="sxs-lookup"><span data-stu-id="6aa17-168">String</span></span>|<span data-ttu-id="6aa17-169">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="6aa17-169">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="6aa17-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="6aa17-170">Response</span></span>
<span data-ttu-id="6aa17-171">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6aa17-171">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aa17-172">Пример</span><span class="sxs-lookup"><span data-stu-id="6aa17-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aa17-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="6aa17-173">Request</span></span>
<span data-ttu-id="6aa17-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6aa17-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
Content-type: application/json
Content-length: 552

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="6aa17-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="6aa17-175">Response</span></span>
<span data-ttu-id="6aa17-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6aa17-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "63a79499-9499-63a7-9994-a7639994a763",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




