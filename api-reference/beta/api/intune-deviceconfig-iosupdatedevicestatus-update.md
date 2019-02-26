---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5917e256357305b1967789507dbcfaf69fd98a0c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162806"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="acbd3-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="acbd3-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="acbd3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acbd3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acbd3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="acbd3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acbd3-106">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="acbd3-106">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acbd3-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="acbd3-107">Prerequisites</span></span>
<span data-ttu-id="acbd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="acbd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="acbd3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acbd3-110">Permission type</span></span>|<span data-ttu-id="acbd3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="acbd3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acbd3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acbd3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="acbd3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acbd3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="acbd3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acbd3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acbd3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acbd3-115">Not supported.</span></span>|
|<span data-ttu-id="acbd3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="acbd3-116">Application</span></span>|<span data-ttu-id="acbd3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acbd3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acbd3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acbd3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="acbd3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="acbd3-119">Request headers</span></span>
|<span data-ttu-id="acbd3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="acbd3-120">Header</span></span>|<span data-ttu-id="acbd3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="acbd3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acbd3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="acbd3-122">Authorization</span></span>|<span data-ttu-id="acbd3-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="acbd3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acbd3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="acbd3-124">Accept</span></span>|<span data-ttu-id="acbd3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="acbd3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acbd3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="acbd3-126">Request body</span></span>
<span data-ttu-id="acbd3-127">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acbd3-127">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="acbd3-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="acbd3-128">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="acbd3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="acbd3-129">Property</span></span>|<span data-ttu-id="acbd3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="acbd3-130">Type</span></span>|<span data-ttu-id="acbd3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="acbd3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acbd3-132">id</span><span class="sxs-lookup"><span data-stu-id="acbd3-132">id</span></span>|<span data-ttu-id="acbd3-133">Строка</span><span class="sxs-lookup"><span data-stu-id="acbd3-133">String</span></span>|<span data-ttu-id="acbd3-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="acbd3-134">Key of the entity.</span></span>|
|<span data-ttu-id="acbd3-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="acbd3-135">installStatus</span></span>|[<span data-ttu-id="acbd3-136">Иосупдатесинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="acbd3-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="acbd3-137">Состояние установки в отчете о политике.</span><span class="sxs-lookup"><span data-stu-id="acbd3-137">The installation status of the policy report.</span></span> <span data-ttu-id="acbd3-138">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`,. `sharedDeviceUserLoggedInError`</span><span class="sxs-lookup"><span data-stu-id="acbd3-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="acbd3-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="acbd3-139">osVersion</span></span>|<span data-ttu-id="acbd3-140">String</span><span class="sxs-lookup"><span data-stu-id="acbd3-140">String</span></span>|<span data-ttu-id="acbd3-141">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="acbd3-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="acbd3-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="acbd3-142">deviceId</span></span>|<span data-ttu-id="acbd3-143">String</span><span class="sxs-lookup"><span data-stu-id="acbd3-143">String</span></span>|<span data-ttu-id="acbd3-144">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="acbd3-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="acbd3-145">userId</span><span class="sxs-lookup"><span data-stu-id="acbd3-145">userId</span></span>|<span data-ttu-id="acbd3-146">String</span><span class="sxs-lookup"><span data-stu-id="acbd3-146">String</span></span>|<span data-ttu-id="acbd3-147">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="acbd3-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="acbd3-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="acbd3-148">deviceDisplayName</span></span>|<span data-ttu-id="acbd3-149">String</span><span class="sxs-lookup"><span data-stu-id="acbd3-149">String</span></span>|<span data-ttu-id="acbd3-150">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="acbd3-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="acbd3-151">userName</span><span class="sxs-lookup"><span data-stu-id="acbd3-151">userName</span></span>|<span data-ttu-id="acbd3-152">String</span><span class="sxs-lookup"><span data-stu-id="acbd3-152">String</span></span>|<span data-ttu-id="acbd3-153">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="acbd3-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="acbd3-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="acbd3-154">deviceModel</span></span>|<span data-ttu-id="acbd3-155">String</span><span class="sxs-lookup"><span data-stu-id="acbd3-155">String</span></span>|<span data-ttu-id="acbd3-156">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="acbd3-156">The device model that is being reported</span></span>|
|<span data-ttu-id="acbd3-157">platform</span><span class="sxs-lookup"><span data-stu-id="acbd3-157">platform</span></span>|<span data-ttu-id="acbd3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="acbd3-158">Int32</span></span>|<span data-ttu-id="acbd3-159">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="acbd3-159">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="acbd3-160">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="acbd3-160">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="acbd3-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acbd3-161">DateTimeOffset</span></span>|<span data-ttu-id="acbd3-162">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="acbd3-162">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="acbd3-163">status</span><span class="sxs-lookup"><span data-stu-id="acbd3-163">status</span></span>|[<span data-ttu-id="acbd3-164">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="acbd3-164">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="acbd3-165">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="acbd3-165">Compliance status of the policy report.</span></span> <span data-ttu-id="acbd3-166">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="acbd3-166">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="acbd3-167">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="acbd3-167">lastReportedDateTime</span></span>|<span data-ttu-id="acbd3-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acbd3-168">DateTimeOffset</span></span>|<span data-ttu-id="acbd3-169">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="acbd3-169">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="acbd3-170">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="acbd3-170">userPrincipalName</span></span>|<span data-ttu-id="acbd3-171">Строка</span><span class="sxs-lookup"><span data-stu-id="acbd3-171">String</span></span>|<span data-ttu-id="acbd3-172">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="acbd3-172">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="acbd3-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="acbd3-173">Response</span></span>
<span data-ttu-id="acbd3-174">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="acbd3-174">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acbd3-175">Пример</span><span class="sxs-lookup"><span data-stu-id="acbd3-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="acbd3-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="acbd3-176">Request</span></span>
<span data-ttu-id="acbd3-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="acbd3-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="acbd3-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="acbd3-178">Response</span></span>
<span data-ttu-id="acbd3-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="acbd3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




