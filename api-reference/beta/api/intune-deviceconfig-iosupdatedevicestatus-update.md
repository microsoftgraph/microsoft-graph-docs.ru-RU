---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e25aeea1ccb384387c5004b8ef4a0837b38dbec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519173"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="13c91-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="13c91-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="13c91-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13c91-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13c91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13c91-106">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="13c91-106">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13c91-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="13c91-107">Prerequisites</span></span>
<span data-ttu-id="13c91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13c91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13c91-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13c91-110">Permission type</span></span>|<span data-ttu-id="13c91-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13c91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13c91-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13c91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13c91-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c91-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13c91-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13c91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13c91-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c91-115">Not supported.</span></span>|
|<span data-ttu-id="13c91-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13c91-116">Application</span></span>|<span data-ttu-id="13c91-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c91-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13c91-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13c91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="13c91-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13c91-119">Request headers</span></span>
|<span data-ttu-id="13c91-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13c91-120">Header</span></span>|<span data-ttu-id="13c91-121">Значение</span><span class="sxs-lookup"><span data-stu-id="13c91-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13c91-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13c91-122">Authorization</span></span>|<span data-ttu-id="13c91-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13c91-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13c91-124">Accept</span><span class="sxs-lookup"><span data-stu-id="13c91-124">Accept</span></span>|<span data-ttu-id="13c91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13c91-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13c91-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13c91-126">Request body</span></span>
<span data-ttu-id="13c91-127">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13c91-127">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="13c91-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="13c91-128">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="13c91-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="13c91-129">Property</span></span>|<span data-ttu-id="13c91-130">Тип</span><span class="sxs-lookup"><span data-stu-id="13c91-130">Type</span></span>|<span data-ttu-id="13c91-131">Описание</span><span class="sxs-lookup"><span data-stu-id="13c91-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13c91-132">id</span><span class="sxs-lookup"><span data-stu-id="13c91-132">id</span></span>|<span data-ttu-id="13c91-133">Строка</span><span class="sxs-lookup"><span data-stu-id="13c91-133">String</span></span>|<span data-ttu-id="13c91-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="13c91-134">Key of the entity.</span></span>|
|<span data-ttu-id="13c91-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="13c91-135">installStatus</span></span>|[<span data-ttu-id="13c91-136">Иосупдатесинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="13c91-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="13c91-137">Состояние установки отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="13c91-137">The installation status of the policy report.</span></span> <span data-ttu-id="13c91-138">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`,. `sharedDeviceUserLoggedInError`</span><span class="sxs-lookup"><span data-stu-id="13c91-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="13c91-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="13c91-139">osVersion</span></span>|<span data-ttu-id="13c91-140">String</span><span class="sxs-lookup"><span data-stu-id="13c91-140">String</span></span>|<span data-ttu-id="13c91-141">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="13c91-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="13c91-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="13c91-142">deviceId</span></span>|<span data-ttu-id="13c91-143">String</span><span class="sxs-lookup"><span data-stu-id="13c91-143">String</span></span>|<span data-ttu-id="13c91-144">ИД устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="13c91-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="13c91-145">userId</span><span class="sxs-lookup"><span data-stu-id="13c91-145">userId</span></span>|<span data-ttu-id="13c91-146">String</span><span class="sxs-lookup"><span data-stu-id="13c91-146">String</span></span>|<span data-ttu-id="13c91-147">ИД пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="13c91-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="13c91-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="13c91-148">deviceDisplayName</span></span>|<span data-ttu-id="13c91-149">String</span><span class="sxs-lookup"><span data-stu-id="13c91-149">String</span></span>|<span data-ttu-id="13c91-150">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="13c91-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="13c91-151">userName</span><span class="sxs-lookup"><span data-stu-id="13c91-151">userName</span></span>|<span data-ttu-id="13c91-152">String</span><span class="sxs-lookup"><span data-stu-id="13c91-152">String</span></span>|<span data-ttu-id="13c91-153">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="13c91-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="13c91-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="13c91-154">deviceModel</span></span>|<span data-ttu-id="13c91-155">String</span><span class="sxs-lookup"><span data-stu-id="13c91-155">String</span></span>|<span data-ttu-id="13c91-156">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="13c91-156">The device model that is being reported</span></span>|
|<span data-ttu-id="13c91-157">platform</span><span class="sxs-lookup"><span data-stu-id="13c91-157">platform</span></span>|<span data-ttu-id="13c91-158">Int32</span><span class="sxs-lookup"><span data-stu-id="13c91-158">Int32</span></span>|<span data-ttu-id="13c91-159">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="13c91-159">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="13c91-160">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="13c91-160">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="13c91-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13c91-161">DateTimeOffset</span></span>|<span data-ttu-id="13c91-162">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="13c91-162">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="13c91-163">status</span><span class="sxs-lookup"><span data-stu-id="13c91-163">status</span></span>|[<span data-ttu-id="13c91-164">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="13c91-164">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="13c91-165">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="13c91-165">Compliance status of the policy report.</span></span> <span data-ttu-id="13c91-166">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="13c91-166">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="13c91-167">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="13c91-167">lastReportedDateTime</span></span>|<span data-ttu-id="13c91-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13c91-168">DateTimeOffset</span></span>|<span data-ttu-id="13c91-169">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="13c91-169">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="13c91-170">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="13c91-170">userPrincipalName</span></span>|<span data-ttu-id="13c91-171">String</span><span class="sxs-lookup"><span data-stu-id="13c91-171">String</span></span>|<span data-ttu-id="13c91-172">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="13c91-172">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="13c91-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="13c91-173">Response</span></span>
<span data-ttu-id="13c91-174">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="13c91-174">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13c91-175">Пример</span><span class="sxs-lookup"><span data-stu-id="13c91-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="13c91-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="13c91-176">Request</span></span>
<span data-ttu-id="13c91-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13c91-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="13c91-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="13c91-178">Response</span></span>
<span data-ttu-id="13c91-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13c91-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





