---
title: Создание объекта iosUpdateDeviceStatus
description: Создание объекта iosUpdateDeviceStatus.
ms.openlocfilehash: 87c1d092d87ed2279d19f8f35f717501add37389
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026772"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="8172e-103">Создание объекта iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8172e-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="8172e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8172e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8172e-105">Создание объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8172e-105">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8172e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8172e-106">Prerequisites</span></span>
<span data-ttu-id="8172e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8172e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8172e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8172e-109">Permission type</span></span>|<span data-ttu-id="8172e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8172e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8172e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8172e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8172e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8172e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8172e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8172e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8172e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8172e-114">Not supported.</span></span>|
|<span data-ttu-id="8172e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8172e-115">Application</span></span>|<span data-ttu-id="8172e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8172e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8172e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8172e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="8172e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8172e-118">Request headers</span></span>
|<span data-ttu-id="8172e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8172e-119">Header</span></span>|<span data-ttu-id="8172e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8172e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8172e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8172e-121">Authorization</span></span>|<span data-ttu-id="8172e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8172e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8172e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8172e-123">Accept</span></span>|<span data-ttu-id="8172e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8172e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8172e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8172e-125">Request body</span></span>
<span data-ttu-id="8172e-126">В теле запроса добавьте представление объекта iosUpdateDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8172e-126">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="8172e-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="8172e-127">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="8172e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8172e-128">Property</span></span>|<span data-ttu-id="8172e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8172e-129">Type</span></span>|<span data-ttu-id="8172e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8172e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8172e-131">id</span><span class="sxs-lookup"><span data-stu-id="8172e-131">id</span></span>|<span data-ttu-id="8172e-132">String</span><span class="sxs-lookup"><span data-stu-id="8172e-132">String</span></span>|<span data-ttu-id="8172e-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8172e-133">Key of the entity.</span></span>|
|<span data-ttu-id="8172e-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="8172e-134">installStatus</span></span>|[<span data-ttu-id="8172e-135">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="8172e-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="8172e-136">Состояние установки в отчете о политике.</span><span class="sxs-lookup"><span data-stu-id="8172e-136">The installation status of the policy report.</span></span> <span data-ttu-id="8172e-137">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="8172e-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="8172e-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="8172e-138">osVersion</span></span>|<span data-ttu-id="8172e-139">String</span><span class="sxs-lookup"><span data-stu-id="8172e-139">String</span></span>|<span data-ttu-id="8172e-140">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="8172e-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="8172e-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="8172e-141">deviceId</span></span>|<span data-ttu-id="8172e-142">String</span><span class="sxs-lookup"><span data-stu-id="8172e-142">String</span></span>|<span data-ttu-id="8172e-143">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="8172e-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="8172e-144">userId</span><span class="sxs-lookup"><span data-stu-id="8172e-144">userId</span></span>|<span data-ttu-id="8172e-145">String</span><span class="sxs-lookup"><span data-stu-id="8172e-145">String</span></span>|<span data-ttu-id="8172e-146">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="8172e-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="8172e-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8172e-147">deviceDisplayName</span></span>|<span data-ttu-id="8172e-148">String</span><span class="sxs-lookup"><span data-stu-id="8172e-148">String</span></span>|<span data-ttu-id="8172e-149">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="8172e-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="8172e-150">userName</span><span class="sxs-lookup"><span data-stu-id="8172e-150">userName</span></span>|<span data-ttu-id="8172e-151">String</span><span class="sxs-lookup"><span data-stu-id="8172e-151">String</span></span>|<span data-ttu-id="8172e-152">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="8172e-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="8172e-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8172e-153">deviceModel</span></span>|<span data-ttu-id="8172e-154">String</span><span class="sxs-lookup"><span data-stu-id="8172e-154">String</span></span>|<span data-ttu-id="8172e-155">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="8172e-155">The device model that is being reported</span></span>|
|<span data-ttu-id="8172e-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8172e-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8172e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8172e-157">DateTimeOffset</span></span>|<span data-ttu-id="8172e-158">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8172e-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="8172e-159">status</span><span class="sxs-lookup"><span data-stu-id="8172e-159">status</span></span>|[<span data-ttu-id="8172e-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8172e-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8172e-161">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="8172e-161">Compliance status of the policy report.</span></span> <span data-ttu-id="8172e-162">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8172e-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8172e-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8172e-163">lastReportedDateTime</span></span>|<span data-ttu-id="8172e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8172e-164">DateTimeOffset</span></span>|<span data-ttu-id="8172e-165">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="8172e-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="8172e-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8172e-166">userPrincipalName</span></span>|<span data-ttu-id="8172e-167">String</span><span class="sxs-lookup"><span data-stu-id="8172e-167">String</span></span>|<span data-ttu-id="8172e-168">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="8172e-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="8172e-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="8172e-169">Response</span></span>
<span data-ttu-id="8172e-170">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8172e-170">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8172e-171">Пример</span><span class="sxs-lookup"><span data-stu-id="8172e-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="8172e-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="8172e-172">Request</span></span>
<span data-ttu-id="8172e-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8172e-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
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

### <a name="response"></a><span data-ttu-id="8172e-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="8172e-174">Response</span></span>
<span data-ttu-id="8172e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8172e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



