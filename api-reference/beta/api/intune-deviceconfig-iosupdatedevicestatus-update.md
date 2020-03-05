---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39c2d87d45c37cb1bd2024ef2167934652af540c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442574"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="aff16-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="aff16-103">Update iosUpdateDeviceStatus</span></span>

<span data-ttu-id="aff16-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aff16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aff16-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aff16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aff16-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aff16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aff16-107">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="aff16-107">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aff16-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="aff16-108">Prerequisites</span></span>
<span data-ttu-id="aff16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aff16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aff16-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aff16-111">Permission type</span></span>|<span data-ttu-id="aff16-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aff16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aff16-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aff16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aff16-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aff16-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aff16-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aff16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aff16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aff16-116">Not supported.</span></span>|
|<span data-ttu-id="aff16-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aff16-117">Application</span></span>|<span data-ttu-id="aff16-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aff16-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aff16-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aff16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="aff16-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aff16-120">Request headers</span></span>
|<span data-ttu-id="aff16-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aff16-121">Header</span></span>|<span data-ttu-id="aff16-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aff16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aff16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aff16-123">Authorization</span></span>|<span data-ttu-id="aff16-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aff16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aff16-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aff16-125">Accept</span></span>|<span data-ttu-id="aff16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aff16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aff16-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aff16-127">Request body</span></span>
<span data-ttu-id="aff16-128">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aff16-128">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="aff16-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="aff16-129">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="aff16-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aff16-130">Property</span></span>|<span data-ttu-id="aff16-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aff16-131">Type</span></span>|<span data-ttu-id="aff16-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aff16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aff16-133">id</span><span class="sxs-lookup"><span data-stu-id="aff16-133">id</span></span>|<span data-ttu-id="aff16-134">Строка</span><span class="sxs-lookup"><span data-stu-id="aff16-134">String</span></span>|<span data-ttu-id="aff16-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aff16-135">Key of the entity.</span></span>|
|<span data-ttu-id="aff16-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="aff16-136">installStatus</span></span>|[<span data-ttu-id="aff16-137">иосупдатесинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="aff16-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="aff16-138">Состояние установки отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="aff16-138">The installation status of the policy report.</span></span> <span data-ttu-id="aff16-139">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`,. `sharedDeviceUserLoggedInError`</span><span class="sxs-lookup"><span data-stu-id="aff16-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="aff16-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="aff16-140">osVersion</span></span>|<span data-ttu-id="aff16-141">String</span><span class="sxs-lookup"><span data-stu-id="aff16-141">String</span></span>|<span data-ttu-id="aff16-142">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="aff16-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="aff16-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="aff16-143">deviceId</span></span>|<span data-ttu-id="aff16-144">String</span><span class="sxs-lookup"><span data-stu-id="aff16-144">String</span></span>|<span data-ttu-id="aff16-145">ИД устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="aff16-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="aff16-146">userId</span><span class="sxs-lookup"><span data-stu-id="aff16-146">userId</span></span>|<span data-ttu-id="aff16-147">String</span><span class="sxs-lookup"><span data-stu-id="aff16-147">String</span></span>|<span data-ttu-id="aff16-148">ИД пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="aff16-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="aff16-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="aff16-149">deviceDisplayName</span></span>|<span data-ttu-id="aff16-150">String</span><span class="sxs-lookup"><span data-stu-id="aff16-150">String</span></span>|<span data-ttu-id="aff16-151">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="aff16-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="aff16-152">userName</span><span class="sxs-lookup"><span data-stu-id="aff16-152">userName</span></span>|<span data-ttu-id="aff16-153">String</span><span class="sxs-lookup"><span data-stu-id="aff16-153">String</span></span>|<span data-ttu-id="aff16-154">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="aff16-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="aff16-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="aff16-155">deviceModel</span></span>|<span data-ttu-id="aff16-156">String</span><span class="sxs-lookup"><span data-stu-id="aff16-156">String</span></span>|<span data-ttu-id="aff16-157">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="aff16-157">The device model that is being reported</span></span>|
|<span data-ttu-id="aff16-158">platform</span><span class="sxs-lookup"><span data-stu-id="aff16-158">platform</span></span>|<span data-ttu-id="aff16-159">Int32</span><span class="sxs-lookup"><span data-stu-id="aff16-159">Int32</span></span>|<span data-ttu-id="aff16-160">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="aff16-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="aff16-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="aff16-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="aff16-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aff16-162">DateTimeOffset</span></span>|<span data-ttu-id="aff16-163">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="aff16-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="aff16-164">status</span><span class="sxs-lookup"><span data-stu-id="aff16-164">status</span></span>|[<span data-ttu-id="aff16-165">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="aff16-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="aff16-166">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="aff16-166">Compliance status of the policy report.</span></span> <span data-ttu-id="aff16-167">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="aff16-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="aff16-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="aff16-168">lastReportedDateTime</span></span>|<span data-ttu-id="aff16-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aff16-169">DateTimeOffset</span></span>|<span data-ttu-id="aff16-170">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="aff16-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="aff16-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aff16-171">userPrincipalName</span></span>|<span data-ttu-id="aff16-172">Строка</span><span class="sxs-lookup"><span data-stu-id="aff16-172">String</span></span>|<span data-ttu-id="aff16-173">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="aff16-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="aff16-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="aff16-174">Response</span></span>
<span data-ttu-id="aff16-175">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="aff16-175">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aff16-176">Пример</span><span class="sxs-lookup"><span data-stu-id="aff16-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="aff16-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="aff16-177">Request</span></span>
<span data-ttu-id="aff16-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aff16-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aff16-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="aff16-179">Response</span></span>
<span data-ttu-id="aff16-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aff16-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





