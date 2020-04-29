---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 473cbbe1e6b18560c4a215ce6cd444024e0de185
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446093"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="040dd-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="040dd-103">Update iosUpdateDeviceStatus</span></span>

<span data-ttu-id="040dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="040dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="040dd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="040dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="040dd-106">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="040dd-106">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="040dd-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="040dd-107">Prerequisites</span></span>
<span data-ttu-id="040dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="040dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="040dd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="040dd-110">Permission type</span></span>|<span data-ttu-id="040dd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="040dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="040dd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="040dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="040dd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="040dd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="040dd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="040dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="040dd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="040dd-115">Not supported.</span></span>|
|<span data-ttu-id="040dd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="040dd-116">Application</span></span>|<span data-ttu-id="040dd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="040dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="040dd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="040dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="040dd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="040dd-119">Request headers</span></span>
|<span data-ttu-id="040dd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="040dd-120">Header</span></span>|<span data-ttu-id="040dd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="040dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="040dd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="040dd-122">Authorization</span></span>|<span data-ttu-id="040dd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="040dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="040dd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="040dd-124">Accept</span></span>|<span data-ttu-id="040dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="040dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="040dd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="040dd-126">Request body</span></span>
<span data-ttu-id="040dd-127">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="040dd-127">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="040dd-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="040dd-128">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="040dd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="040dd-129">Property</span></span>|<span data-ttu-id="040dd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="040dd-130">Type</span></span>|<span data-ttu-id="040dd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="040dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="040dd-132">id</span><span class="sxs-lookup"><span data-stu-id="040dd-132">id</span></span>|<span data-ttu-id="040dd-133">Строка</span><span class="sxs-lookup"><span data-stu-id="040dd-133">String</span></span>|<span data-ttu-id="040dd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="040dd-134">Key of the entity.</span></span>|
|<span data-ttu-id="040dd-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="040dd-135">installStatus</span></span>|[<span data-ttu-id="040dd-136">иосупдатесинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="040dd-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="040dd-137">Состояние установки отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="040dd-137">The installation status of the policy report.</span></span> <span data-ttu-id="040dd-138">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`,. `sharedDeviceUserLoggedInError`</span><span class="sxs-lookup"><span data-stu-id="040dd-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="040dd-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="040dd-139">osVersion</span></span>|<span data-ttu-id="040dd-140">String</span><span class="sxs-lookup"><span data-stu-id="040dd-140">String</span></span>|<span data-ttu-id="040dd-141">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="040dd-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="040dd-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="040dd-142">deviceId</span></span>|<span data-ttu-id="040dd-143">String</span><span class="sxs-lookup"><span data-stu-id="040dd-143">String</span></span>|<span data-ttu-id="040dd-144">ИД устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="040dd-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="040dd-145">userId</span><span class="sxs-lookup"><span data-stu-id="040dd-145">userId</span></span>|<span data-ttu-id="040dd-146">String</span><span class="sxs-lookup"><span data-stu-id="040dd-146">String</span></span>|<span data-ttu-id="040dd-147">ИД пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="040dd-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="040dd-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="040dd-148">deviceDisplayName</span></span>|<span data-ttu-id="040dd-149">String</span><span class="sxs-lookup"><span data-stu-id="040dd-149">String</span></span>|<span data-ttu-id="040dd-150">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="040dd-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="040dd-151">userName</span><span class="sxs-lookup"><span data-stu-id="040dd-151">userName</span></span>|<span data-ttu-id="040dd-152">String</span><span class="sxs-lookup"><span data-stu-id="040dd-152">String</span></span>|<span data-ttu-id="040dd-153">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="040dd-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="040dd-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="040dd-154">deviceModel</span></span>|<span data-ttu-id="040dd-155">String</span><span class="sxs-lookup"><span data-stu-id="040dd-155">String</span></span>|<span data-ttu-id="040dd-156">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="040dd-156">The device model that is being reported</span></span>|
|<span data-ttu-id="040dd-157">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="040dd-157">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="040dd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="040dd-158">DateTimeOffset</span></span>|<span data-ttu-id="040dd-159">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="040dd-159">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="040dd-160">status</span><span class="sxs-lookup"><span data-stu-id="040dd-160">status</span></span>|[<span data-ttu-id="040dd-161">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="040dd-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="040dd-162">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="040dd-162">Compliance status of the policy report.</span></span> <span data-ttu-id="040dd-163">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="040dd-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="040dd-164">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="040dd-164">lastReportedDateTime</span></span>|<span data-ttu-id="040dd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="040dd-165">DateTimeOffset</span></span>|<span data-ttu-id="040dd-166">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="040dd-166">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="040dd-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="040dd-167">userPrincipalName</span></span>|<span data-ttu-id="040dd-168">Строка</span><span class="sxs-lookup"><span data-stu-id="040dd-168">String</span></span>|<span data-ttu-id="040dd-169">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="040dd-169">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="040dd-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="040dd-170">Response</span></span>
<span data-ttu-id="040dd-171">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="040dd-171">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="040dd-172">Пример</span><span class="sxs-lookup"><span data-stu-id="040dd-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="040dd-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="040dd-173">Request</span></span>
<span data-ttu-id="040dd-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="040dd-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="040dd-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="040dd-175">Response</span></span>
<span data-ttu-id="040dd-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="040dd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






