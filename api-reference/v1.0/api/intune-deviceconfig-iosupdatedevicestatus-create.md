---
title: Создание объекта iosUpdateDeviceStatus
description: Создание объекта iosUpdateDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6f8fc2d494ded8be55413441a949074205b83f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514468"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="db2e7-103">Создание объекта iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="db2e7-103">Create iosUpdateDeviceStatus</span></span>

<span data-ttu-id="db2e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db2e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db2e7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db2e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db2e7-106">Создание объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="db2e7-106">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db2e7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="db2e7-107">Prerequisites</span></span>
<span data-ttu-id="db2e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db2e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db2e7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db2e7-110">Permission type</span></span>|<span data-ttu-id="db2e7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="db2e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db2e7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db2e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db2e7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db2e7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db2e7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db2e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db2e7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db2e7-115">Not supported.</span></span>|
|<span data-ttu-id="db2e7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db2e7-116">Application</span></span>|<span data-ttu-id="db2e7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db2e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db2e7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db2e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="db2e7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="db2e7-119">Request headers</span></span>
|<span data-ttu-id="db2e7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db2e7-120">Header</span></span>|<span data-ttu-id="db2e7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="db2e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db2e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db2e7-122">Authorization</span></span>|<span data-ttu-id="db2e7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db2e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db2e7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="db2e7-124">Accept</span></span>|<span data-ttu-id="db2e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db2e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db2e7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db2e7-126">Request body</span></span>
<span data-ttu-id="db2e7-127">В теле запроса добавьте представление объекта iosUpdateDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db2e7-127">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="db2e7-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="db2e7-128">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="db2e7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="db2e7-129">Property</span></span>|<span data-ttu-id="db2e7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="db2e7-130">Type</span></span>|<span data-ttu-id="db2e7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="db2e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db2e7-132">id</span><span class="sxs-lookup"><span data-stu-id="db2e7-132">id</span></span>|<span data-ttu-id="db2e7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="db2e7-133">String</span></span>|<span data-ttu-id="db2e7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="db2e7-134">Key of the entity.</span></span>|
|<span data-ttu-id="db2e7-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="db2e7-135">installStatus</span></span>|[<span data-ttu-id="db2e7-136">иосупдатесинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="db2e7-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="db2e7-137">Состояние установки отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="db2e7-137">The installation status of the policy report.</span></span> <span data-ttu-id="db2e7-138">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`,. `sharedDeviceUserLoggedInError`</span><span class="sxs-lookup"><span data-stu-id="db2e7-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="db2e7-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="db2e7-139">osVersion</span></span>|<span data-ttu-id="db2e7-140">Строка</span><span class="sxs-lookup"><span data-stu-id="db2e7-140">String</span></span>|<span data-ttu-id="db2e7-141">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="db2e7-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="db2e7-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="db2e7-142">deviceId</span></span>|<span data-ttu-id="db2e7-143">String</span><span class="sxs-lookup"><span data-stu-id="db2e7-143">String</span></span>|<span data-ttu-id="db2e7-144">ИД устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="db2e7-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="db2e7-145">userId</span><span class="sxs-lookup"><span data-stu-id="db2e7-145">userId</span></span>|<span data-ttu-id="db2e7-146">String</span><span class="sxs-lookup"><span data-stu-id="db2e7-146">String</span></span>|<span data-ttu-id="db2e7-147">ИД пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="db2e7-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="db2e7-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="db2e7-148">deviceDisplayName</span></span>|<span data-ttu-id="db2e7-149">Строка</span><span class="sxs-lookup"><span data-stu-id="db2e7-149">String</span></span>|<span data-ttu-id="db2e7-150">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="db2e7-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="db2e7-151">userName</span><span class="sxs-lookup"><span data-stu-id="db2e7-151">userName</span></span>|<span data-ttu-id="db2e7-152">Строка</span><span class="sxs-lookup"><span data-stu-id="db2e7-152">String</span></span>|<span data-ttu-id="db2e7-153">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="db2e7-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="db2e7-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="db2e7-154">deviceModel</span></span>|<span data-ttu-id="db2e7-155">String</span><span class="sxs-lookup"><span data-stu-id="db2e7-155">String</span></span>|<span data-ttu-id="db2e7-156">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="db2e7-156">The device model that is being reported</span></span>|
|<span data-ttu-id="db2e7-157">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="db2e7-157">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="db2e7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db2e7-158">DateTimeOffset</span></span>|<span data-ttu-id="db2e7-159">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="db2e7-159">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="db2e7-160">status</span><span class="sxs-lookup"><span data-stu-id="db2e7-160">status</span></span>|[<span data-ttu-id="db2e7-161">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="db2e7-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="db2e7-162">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="db2e7-162">Compliance status of the policy report.</span></span> <span data-ttu-id="db2e7-163">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="db2e7-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="db2e7-164">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="db2e7-164">lastReportedDateTime</span></span>|<span data-ttu-id="db2e7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db2e7-165">DateTimeOffset</span></span>|<span data-ttu-id="db2e7-166">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="db2e7-166">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="db2e7-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="db2e7-167">userPrincipalName</span></span>|<span data-ttu-id="db2e7-168">Строка</span><span class="sxs-lookup"><span data-stu-id="db2e7-168">String</span></span>|<span data-ttu-id="db2e7-169">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="db2e7-169">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="db2e7-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="db2e7-170">Response</span></span>
<span data-ttu-id="db2e7-171">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="db2e7-171">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db2e7-172">Пример</span><span class="sxs-lookup"><span data-stu-id="db2e7-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="db2e7-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="db2e7-173">Request</span></span>
<span data-ttu-id="db2e7-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db2e7-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="db2e7-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="db2e7-175">Response</span></span>
<span data-ttu-id="db2e7-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db2e7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




