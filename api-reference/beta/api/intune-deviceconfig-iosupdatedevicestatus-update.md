---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 402b9ba9817ee5335ac0cf5b38ffa9de5b66efb6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49220268"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="8a801-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8a801-103">Update iosUpdateDeviceStatus</span></span>

<span data-ttu-id="8a801-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a801-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a801-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a801-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a801-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a801-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a801-107">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8a801-107">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a801-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8a801-108">Prerequisites</span></span>
<span data-ttu-id="8a801-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a801-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a801-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a801-111">Permission type</span></span>|<span data-ttu-id="8a801-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a801-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a801-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a801-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a801-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a801-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8a801-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a801-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a801-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a801-116">Not supported.</span></span>|
|<span data-ttu-id="8a801-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8a801-117">Application</span></span>|<span data-ttu-id="8a801-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a801-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a801-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a801-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="8a801-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8a801-120">Request headers</span></span>
|<span data-ttu-id="8a801-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a801-121">Header</span></span>|<span data-ttu-id="8a801-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8a801-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a801-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a801-123">Authorization</span></span>|<span data-ttu-id="8a801-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a801-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a801-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8a801-125">Accept</span></span>|<span data-ttu-id="8a801-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a801-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a801-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a801-127">Request body</span></span>
<span data-ttu-id="8a801-128">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a801-128">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="8a801-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8a801-129">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="8a801-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a801-130">Property</span></span>|<span data-ttu-id="8a801-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8a801-131">Type</span></span>|<span data-ttu-id="8a801-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8a801-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a801-133">id</span><span class="sxs-lookup"><span data-stu-id="8a801-133">id</span></span>|<span data-ttu-id="8a801-134">String</span><span class="sxs-lookup"><span data-stu-id="8a801-134">String</span></span>|<span data-ttu-id="8a801-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8a801-135">Key of the entity.</span></span>|
|<span data-ttu-id="8a801-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="8a801-136">installStatus</span></span>|[<span data-ttu-id="8a801-137">иосупдатесинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="8a801-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="8a801-138">Состояние установки отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="8a801-138">The installation status of the policy report.</span></span> <span data-ttu-id="8a801-139">Возможные значения: `success` ,,,,,,,,,,,,,,,,,,,,,,,,,,, `available` `idle` `unknown` `mdmClientCrashed` `timeout` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installing` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation` `sharedDeviceUserLoggedInError` `updateError` `deviceOsHigherThanDesiredOsVersion` `updateScanFailed` .</span><span class="sxs-lookup"><span data-stu-id="8a801-139">Possible values are: `success`, `available`, `idle`, `unknown`, `mdmClientCrashed`, `timeout`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`, `updateError`, `deviceOsHigherThanDesiredOsVersion`, `updateScanFailed`.</span></span>|
|<span data-ttu-id="8a801-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="8a801-140">osVersion</span></span>|<span data-ttu-id="8a801-141">String</span><span class="sxs-lookup"><span data-stu-id="8a801-141">String</span></span>|<span data-ttu-id="8a801-142">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="8a801-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="8a801-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="8a801-143">deviceId</span></span>|<span data-ttu-id="8a801-144">String</span><span class="sxs-lookup"><span data-stu-id="8a801-144">String</span></span>|<span data-ttu-id="8a801-145">ИД устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="8a801-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="8a801-146">userId</span><span class="sxs-lookup"><span data-stu-id="8a801-146">userId</span></span>|<span data-ttu-id="8a801-147">String</span><span class="sxs-lookup"><span data-stu-id="8a801-147">String</span></span>|<span data-ttu-id="8a801-148">ИД пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="8a801-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="8a801-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8a801-149">deviceDisplayName</span></span>|<span data-ttu-id="8a801-150">String</span><span class="sxs-lookup"><span data-stu-id="8a801-150">String</span></span>|<span data-ttu-id="8a801-151">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="8a801-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="8a801-152">userName</span><span class="sxs-lookup"><span data-stu-id="8a801-152">userName</span></span>|<span data-ttu-id="8a801-153">String</span><span class="sxs-lookup"><span data-stu-id="8a801-153">String</span></span>|<span data-ttu-id="8a801-154">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="8a801-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="8a801-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8a801-155">deviceModel</span></span>|<span data-ttu-id="8a801-156">String</span><span class="sxs-lookup"><span data-stu-id="8a801-156">String</span></span>|<span data-ttu-id="8a801-157">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="8a801-157">The device model that is being reported</span></span>|
|<span data-ttu-id="8a801-158">платформа</span><span class="sxs-lookup"><span data-stu-id="8a801-158">platform</span></span>|<span data-ttu-id="8a801-159">Int32</span><span class="sxs-lookup"><span data-stu-id="8a801-159">Int32</span></span>|<span data-ttu-id="8a801-160">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="8a801-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="8a801-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8a801-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8a801-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a801-162">DateTimeOffset</span></span>|<span data-ttu-id="8a801-163">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8a801-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="8a801-164">status</span><span class="sxs-lookup"><span data-stu-id="8a801-164">status</span></span>|[<span data-ttu-id="8a801-165">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="8a801-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8a801-166">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="8a801-166">Compliance status of the policy report.</span></span> <span data-ttu-id="8a801-167">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8a801-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8a801-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a801-168">lastReportedDateTime</span></span>|<span data-ttu-id="8a801-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a801-169">DateTimeOffset</span></span>|<span data-ttu-id="8a801-170">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="8a801-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="8a801-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8a801-171">userPrincipalName</span></span>|<span data-ttu-id="8a801-172">String</span><span class="sxs-lookup"><span data-stu-id="8a801-172">String</span></span>|<span data-ttu-id="8a801-173">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="8a801-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="8a801-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a801-174">Response</span></span>
<span data-ttu-id="8a801-175">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8a801-175">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a801-176">Пример</span><span class="sxs-lookup"><span data-stu-id="8a801-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a801-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a801-177">Request</span></span>
<span data-ttu-id="8a801-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a801-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
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

### <a name="response"></a><span data-ttu-id="8a801-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a801-179">Response</span></span>
<span data-ttu-id="8a801-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a801-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

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
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




