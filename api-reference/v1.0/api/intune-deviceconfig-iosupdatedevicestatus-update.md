---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af4fc0ae93c501ee27d378ac98c767cf7cd11ebb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997577"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="e3700-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="e3700-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="e3700-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3700-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3700-105">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="e3700-105">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3700-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e3700-106">Prerequisites</span></span>
<span data-ttu-id="e3700-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3700-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3700-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3700-109">Permission type</span></span>|<span data-ttu-id="e3700-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3700-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3700-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3700-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3700-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3700-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3700-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3700-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3700-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3700-114">Not supported.</span></span>|
|<span data-ttu-id="e3700-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3700-115">Application</span></span>|<span data-ttu-id="e3700-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3700-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3700-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3700-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="e3700-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3700-118">Request headers</span></span>
|<span data-ttu-id="e3700-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3700-119">Header</span></span>|<span data-ttu-id="e3700-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e3700-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3700-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3700-121">Authorization</span></span>|<span data-ttu-id="e3700-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3700-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3700-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e3700-123">Accept</span></span>|<span data-ttu-id="e3700-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3700-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3700-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e3700-125">Request body</span></span>
<span data-ttu-id="e3700-126">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3700-126">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="e3700-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="e3700-127">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="e3700-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3700-128">Property</span></span>|<span data-ttu-id="e3700-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e3700-129">Type</span></span>|<span data-ttu-id="e3700-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e3700-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3700-131">id</span><span class="sxs-lookup"><span data-stu-id="e3700-131">id</span></span>|<span data-ttu-id="e3700-132">Строка</span><span class="sxs-lookup"><span data-stu-id="e3700-132">String</span></span>|<span data-ttu-id="e3700-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e3700-133">Key of the entity.</span></span>|
|<span data-ttu-id="e3700-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="e3700-134">installStatus</span></span>|[<span data-ttu-id="e3700-135">Иосупдатесинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="e3700-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="e3700-136">Состояние установки отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="e3700-136">The installation status of the policy report.</span></span> <span data-ttu-id="e3700-137">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`,. `sharedDeviceUserLoggedInError`</span><span class="sxs-lookup"><span data-stu-id="e3700-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="e3700-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="e3700-138">osVersion</span></span>|<span data-ttu-id="e3700-139">String</span><span class="sxs-lookup"><span data-stu-id="e3700-139">String</span></span>|<span data-ttu-id="e3700-140">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="e3700-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="e3700-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="e3700-141">deviceId</span></span>|<span data-ttu-id="e3700-142">String</span><span class="sxs-lookup"><span data-stu-id="e3700-142">String</span></span>|<span data-ttu-id="e3700-143">ИД устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="e3700-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="e3700-144">userId</span><span class="sxs-lookup"><span data-stu-id="e3700-144">userId</span></span>|<span data-ttu-id="e3700-145">String</span><span class="sxs-lookup"><span data-stu-id="e3700-145">String</span></span>|<span data-ttu-id="e3700-146">ИД пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="e3700-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="e3700-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e3700-147">deviceDisplayName</span></span>|<span data-ttu-id="e3700-148">String</span><span class="sxs-lookup"><span data-stu-id="e3700-148">String</span></span>|<span data-ttu-id="e3700-149">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="e3700-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="e3700-150">userName</span><span class="sxs-lookup"><span data-stu-id="e3700-150">userName</span></span>|<span data-ttu-id="e3700-151">String</span><span class="sxs-lookup"><span data-stu-id="e3700-151">String</span></span>|<span data-ttu-id="e3700-152">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="e3700-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="e3700-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="e3700-153">deviceModel</span></span>|<span data-ttu-id="e3700-154">String</span><span class="sxs-lookup"><span data-stu-id="e3700-154">String</span></span>|<span data-ttu-id="e3700-155">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="e3700-155">The device model that is being reported</span></span>|
|<span data-ttu-id="e3700-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e3700-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="e3700-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3700-157">DateTimeOffset</span></span>|<span data-ttu-id="e3700-158">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e3700-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="e3700-159">status</span><span class="sxs-lookup"><span data-stu-id="e3700-159">status</span></span>|[<span data-ttu-id="e3700-160">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="e3700-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e3700-161">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="e3700-161">Compliance status of the policy report.</span></span> <span data-ttu-id="e3700-162">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e3700-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e3700-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3700-163">lastReportedDateTime</span></span>|<span data-ttu-id="e3700-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3700-164">DateTimeOffset</span></span>|<span data-ttu-id="e3700-165">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="e3700-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="e3700-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e3700-166">userPrincipalName</span></span>|<span data-ttu-id="e3700-167">Строка</span><span class="sxs-lookup"><span data-stu-id="e3700-167">String</span></span>|<span data-ttu-id="e3700-168">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="e3700-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="e3700-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3700-169">Response</span></span>
<span data-ttu-id="e3700-170">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e3700-170">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3700-171">Пример</span><span class="sxs-lookup"><span data-stu-id="e3700-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3700-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3700-172">Request</span></span>
<span data-ttu-id="e3700-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3700-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3700-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3700-174">Response</span></span>
<span data-ttu-id="e3700-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3700-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



