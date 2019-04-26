---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ede7348a948d78c2ec9f3219fa1ff072d17915f3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549869"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="46dcc-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="46dcc-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="46dcc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46dcc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46dcc-105">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="46dcc-105">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46dcc-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="46dcc-106">Prerequisites</span></span>
<span data-ttu-id="46dcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46dcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46dcc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46dcc-109">Permission type</span></span>|<span data-ttu-id="46dcc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46dcc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46dcc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46dcc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46dcc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46dcc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46dcc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46dcc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46dcc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46dcc-114">Not supported.</span></span>|
|<span data-ttu-id="46dcc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46dcc-115">Application</span></span>|<span data-ttu-id="46dcc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46dcc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46dcc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46dcc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="46dcc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46dcc-118">Request headers</span></span>
|<span data-ttu-id="46dcc-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46dcc-119">Header</span></span>|<span data-ttu-id="46dcc-120">Значение</span><span class="sxs-lookup"><span data-stu-id="46dcc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46dcc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46dcc-121">Authorization</span></span>|<span data-ttu-id="46dcc-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46dcc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46dcc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="46dcc-123">Accept</span></span>|<span data-ttu-id="46dcc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="46dcc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46dcc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46dcc-125">Request body</span></span>
<span data-ttu-id="46dcc-126">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46dcc-126">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="46dcc-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="46dcc-127">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="46dcc-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="46dcc-128">Property</span></span>|<span data-ttu-id="46dcc-129">Тип</span><span class="sxs-lookup"><span data-stu-id="46dcc-129">Type</span></span>|<span data-ttu-id="46dcc-130">Описание</span><span class="sxs-lookup"><span data-stu-id="46dcc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46dcc-131">id</span><span class="sxs-lookup"><span data-stu-id="46dcc-131">id</span></span>|<span data-ttu-id="46dcc-132">Строка</span><span class="sxs-lookup"><span data-stu-id="46dcc-132">String</span></span>|<span data-ttu-id="46dcc-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="46dcc-133">Key of the entity.</span></span>|
|<span data-ttu-id="46dcc-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="46dcc-134">installStatus</span></span>|[<span data-ttu-id="46dcc-135">Иосупдатесинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="46dcc-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="46dcc-136">Состояние установки отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="46dcc-136">The installation status of the policy report.</span></span> <span data-ttu-id="46dcc-137">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`,. `sharedDeviceUserLoggedInError`</span><span class="sxs-lookup"><span data-stu-id="46dcc-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="46dcc-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="46dcc-138">osVersion</span></span>|<span data-ttu-id="46dcc-139">String</span><span class="sxs-lookup"><span data-stu-id="46dcc-139">String</span></span>|<span data-ttu-id="46dcc-140">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="46dcc-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="46dcc-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="46dcc-141">deviceId</span></span>|<span data-ttu-id="46dcc-142">String</span><span class="sxs-lookup"><span data-stu-id="46dcc-142">String</span></span>|<span data-ttu-id="46dcc-143">ИД устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="46dcc-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="46dcc-144">userId</span><span class="sxs-lookup"><span data-stu-id="46dcc-144">userId</span></span>|<span data-ttu-id="46dcc-145">String</span><span class="sxs-lookup"><span data-stu-id="46dcc-145">String</span></span>|<span data-ttu-id="46dcc-146">ИД пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="46dcc-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="46dcc-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="46dcc-147">deviceDisplayName</span></span>|<span data-ttu-id="46dcc-148">String</span><span class="sxs-lookup"><span data-stu-id="46dcc-148">String</span></span>|<span data-ttu-id="46dcc-149">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="46dcc-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="46dcc-150">userName</span><span class="sxs-lookup"><span data-stu-id="46dcc-150">userName</span></span>|<span data-ttu-id="46dcc-151">String</span><span class="sxs-lookup"><span data-stu-id="46dcc-151">String</span></span>|<span data-ttu-id="46dcc-152">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="46dcc-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="46dcc-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="46dcc-153">deviceModel</span></span>|<span data-ttu-id="46dcc-154">String</span><span class="sxs-lookup"><span data-stu-id="46dcc-154">String</span></span>|<span data-ttu-id="46dcc-155">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="46dcc-155">The device model that is being reported</span></span>|
|<span data-ttu-id="46dcc-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="46dcc-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="46dcc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46dcc-157">DateTimeOffset</span></span>|<span data-ttu-id="46dcc-158">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="46dcc-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="46dcc-159">status</span><span class="sxs-lookup"><span data-stu-id="46dcc-159">status</span></span>|[<span data-ttu-id="46dcc-160">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="46dcc-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="46dcc-161">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="46dcc-161">Compliance status of the policy report.</span></span> <span data-ttu-id="46dcc-162">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="46dcc-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="46dcc-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="46dcc-163">lastReportedDateTime</span></span>|<span data-ttu-id="46dcc-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46dcc-164">DateTimeOffset</span></span>|<span data-ttu-id="46dcc-165">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="46dcc-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="46dcc-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46dcc-166">userPrincipalName</span></span>|<span data-ttu-id="46dcc-167">String</span><span class="sxs-lookup"><span data-stu-id="46dcc-167">String</span></span>|<span data-ttu-id="46dcc-168">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="46dcc-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="46dcc-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="46dcc-169">Response</span></span>
<span data-ttu-id="46dcc-170">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="46dcc-170">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46dcc-171">Пример</span><span class="sxs-lookup"><span data-stu-id="46dcc-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="46dcc-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="46dcc-172">Request</span></span>
<span data-ttu-id="46dcc-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46dcc-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="46dcc-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="46dcc-174">Response</span></span>
<span data-ttu-id="46dcc-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46dcc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



