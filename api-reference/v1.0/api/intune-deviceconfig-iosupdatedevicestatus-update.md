---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f3b6e10719ac13bb8fb483a837154cd83da553a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820365"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="3a54a-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="3a54a-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="3a54a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3a54a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a54a-105">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="3a54a-105">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a54a-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3a54a-106">Prerequisites</span></span>
<span data-ttu-id="3a54a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a54a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a54a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a54a-109">Permission type</span></span>|<span data-ttu-id="3a54a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a54a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a54a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a54a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a54a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a54a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a54a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a54a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a54a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a54a-114">Not supported.</span></span>|
|<span data-ttu-id="3a54a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a54a-115">Application</span></span>|<span data-ttu-id="3a54a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a54a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a54a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a54a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="3a54a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a54a-118">Request headers</span></span>
|<span data-ttu-id="3a54a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a54a-119">Header</span></span>|<span data-ttu-id="3a54a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3a54a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a54a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a54a-121">Authorization</span></span>|<span data-ttu-id="3a54a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3a54a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a54a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3a54a-123">Accept</span></span>|<span data-ttu-id="3a54a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3a54a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a54a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a54a-125">Request body</span></span>
<span data-ttu-id="3a54a-126">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a54a-126">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="3a54a-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="3a54a-127">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="3a54a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a54a-128">Property</span></span>|<span data-ttu-id="3a54a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3a54a-129">Type</span></span>|<span data-ttu-id="3a54a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3a54a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a54a-131">id</span><span class="sxs-lookup"><span data-stu-id="3a54a-131">id</span></span>|<span data-ttu-id="3a54a-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3a54a-132">String</span></span>|<span data-ttu-id="3a54a-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3a54a-133">Key of the entity.</span></span>|
|<span data-ttu-id="3a54a-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="3a54a-134">installStatus</span></span>|[<span data-ttu-id="3a54a-135">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="3a54a-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="3a54a-136">Состояние установки в отчете о политике.</span><span class="sxs-lookup"><span data-stu-id="3a54a-136">The installation status of the policy report.</span></span> <span data-ttu-id="3a54a-137">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="3a54a-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="3a54a-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="3a54a-138">osVersion</span></span>|<span data-ttu-id="3a54a-139">String</span><span class="sxs-lookup"><span data-stu-id="3a54a-139">String</span></span>|<span data-ttu-id="3a54a-140">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="3a54a-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="3a54a-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="3a54a-141">deviceId</span></span>|<span data-ttu-id="3a54a-142">String</span><span class="sxs-lookup"><span data-stu-id="3a54a-142">String</span></span>|<span data-ttu-id="3a54a-143">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="3a54a-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="3a54a-144">userId</span><span class="sxs-lookup"><span data-stu-id="3a54a-144">userId</span></span>|<span data-ttu-id="3a54a-145">String</span><span class="sxs-lookup"><span data-stu-id="3a54a-145">String</span></span>|<span data-ttu-id="3a54a-146">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="3a54a-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="3a54a-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3a54a-147">deviceDisplayName</span></span>|<span data-ttu-id="3a54a-148">String</span><span class="sxs-lookup"><span data-stu-id="3a54a-148">String</span></span>|<span data-ttu-id="3a54a-149">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="3a54a-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="3a54a-150">userName</span><span class="sxs-lookup"><span data-stu-id="3a54a-150">userName</span></span>|<span data-ttu-id="3a54a-151">String</span><span class="sxs-lookup"><span data-stu-id="3a54a-151">String</span></span>|<span data-ttu-id="3a54a-152">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="3a54a-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="3a54a-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="3a54a-153">deviceModel</span></span>|<span data-ttu-id="3a54a-154">String</span><span class="sxs-lookup"><span data-stu-id="3a54a-154">String</span></span>|<span data-ttu-id="3a54a-155">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="3a54a-155">The device model that is being reported</span></span>|
|<span data-ttu-id="3a54a-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3a54a-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3a54a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a54a-157">DateTimeOffset</span></span>|<span data-ttu-id="3a54a-158">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3a54a-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="3a54a-159">status</span><span class="sxs-lookup"><span data-stu-id="3a54a-159">status</span></span>|[<span data-ttu-id="3a54a-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3a54a-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3a54a-161">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="3a54a-161">Compliance status of the policy report.</span></span> <span data-ttu-id="3a54a-162">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3a54a-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3a54a-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a54a-163">lastReportedDateTime</span></span>|<span data-ttu-id="3a54a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a54a-164">DateTimeOffset</span></span>|<span data-ttu-id="3a54a-165">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="3a54a-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="3a54a-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3a54a-166">userPrincipalName</span></span>|<span data-ttu-id="3a54a-167">String</span><span class="sxs-lookup"><span data-stu-id="3a54a-167">String</span></span>|<span data-ttu-id="3a54a-168">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="3a54a-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="3a54a-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a54a-169">Response</span></span>
<span data-ttu-id="3a54a-170">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3a54a-170">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a54a-171">Пример</span><span class="sxs-lookup"><span data-stu-id="3a54a-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a54a-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a54a-172">Request</span></span>
<span data-ttu-id="3a54a-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a54a-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3a54a-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a54a-174">Response</span></span>
<span data-ttu-id="3a54a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3a54a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



