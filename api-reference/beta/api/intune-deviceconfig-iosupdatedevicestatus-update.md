---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e501171c66b2bfc18f82376d382f026f39291e5a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419816"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="62a4f-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="62a4f-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="62a4f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62a4f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="62a4f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62a4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62a4f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62a4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62a4f-107">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="62a4f-107">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62a4f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="62a4f-108">Prerequisites</span></span>
<span data-ttu-id="62a4f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="62a4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="62a4f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62a4f-111">Permission type</span></span>|<span data-ttu-id="62a4f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62a4f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62a4f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62a4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62a4f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a4f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62a4f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62a4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62a4f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62a4f-116">Not supported.</span></span>|
|<span data-ttu-id="62a4f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62a4f-117">Application</span></span>|<span data-ttu-id="62a4f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62a4f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62a4f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62a4f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="62a4f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62a4f-120">Request headers</span></span>
|<span data-ttu-id="62a4f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62a4f-121">Header</span></span>|<span data-ttu-id="62a4f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="62a4f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62a4f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62a4f-123">Authorization</span></span>|<span data-ttu-id="62a4f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="62a4f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62a4f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="62a4f-125">Accept</span></span>|<span data-ttu-id="62a4f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62a4f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62a4f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="62a4f-127">Request body</span></span>
<span data-ttu-id="62a4f-128">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62a4f-128">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="62a4f-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="62a4f-129">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="62a4f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="62a4f-130">Property</span></span>|<span data-ttu-id="62a4f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="62a4f-131">Type</span></span>|<span data-ttu-id="62a4f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="62a4f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a4f-133">id</span><span class="sxs-lookup"><span data-stu-id="62a4f-133">id</span></span>|<span data-ttu-id="62a4f-134">String</span><span class="sxs-lookup"><span data-stu-id="62a4f-134">String</span></span>|<span data-ttu-id="62a4f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="62a4f-135">Key of the entity.</span></span>|
|<span data-ttu-id="62a4f-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="62a4f-136">installStatus</span></span>|[<span data-ttu-id="62a4f-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="62a4f-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="62a4f-138">Состояние установки в отчете о политике.</span><span class="sxs-lookup"><span data-stu-id="62a4f-138">The installation status of the policy report.</span></span> <span data-ttu-id="62a4f-139">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="62a4f-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="62a4f-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="62a4f-140">osVersion</span></span>|<span data-ttu-id="62a4f-141">String</span><span class="sxs-lookup"><span data-stu-id="62a4f-141">String</span></span>|<span data-ttu-id="62a4f-142">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="62a4f-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="62a4f-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="62a4f-143">deviceId</span></span>|<span data-ttu-id="62a4f-144">String</span><span class="sxs-lookup"><span data-stu-id="62a4f-144">String</span></span>|<span data-ttu-id="62a4f-145">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="62a4f-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="62a4f-146">userId</span><span class="sxs-lookup"><span data-stu-id="62a4f-146">userId</span></span>|<span data-ttu-id="62a4f-147">String</span><span class="sxs-lookup"><span data-stu-id="62a4f-147">String</span></span>|<span data-ttu-id="62a4f-148">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="62a4f-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="62a4f-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="62a4f-149">deviceDisplayName</span></span>|<span data-ttu-id="62a4f-150">String</span><span class="sxs-lookup"><span data-stu-id="62a4f-150">String</span></span>|<span data-ttu-id="62a4f-151">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="62a4f-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="62a4f-152">userName</span><span class="sxs-lookup"><span data-stu-id="62a4f-152">userName</span></span>|<span data-ttu-id="62a4f-153">String</span><span class="sxs-lookup"><span data-stu-id="62a4f-153">String</span></span>|<span data-ttu-id="62a4f-154">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="62a4f-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="62a4f-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="62a4f-155">deviceModel</span></span>|<span data-ttu-id="62a4f-156">String</span><span class="sxs-lookup"><span data-stu-id="62a4f-156">String</span></span>|<span data-ttu-id="62a4f-157">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="62a4f-157">The device model that is being reported</span></span>|
|<span data-ttu-id="62a4f-158">platform</span><span class="sxs-lookup"><span data-stu-id="62a4f-158">platform</span></span>|<span data-ttu-id="62a4f-159">Int32</span><span class="sxs-lookup"><span data-stu-id="62a4f-159">Int32</span></span>|<span data-ttu-id="62a4f-160">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="62a4f-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="62a4f-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="62a4f-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="62a4f-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62a4f-162">DateTimeOffset</span></span>|<span data-ttu-id="62a4f-163">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="62a4f-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="62a4f-164">status</span><span class="sxs-lookup"><span data-stu-id="62a4f-164">status</span></span>|[<span data-ttu-id="62a4f-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="62a4f-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="62a4f-166">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="62a4f-166">Compliance status of the policy report.</span></span> <span data-ttu-id="62a4f-167">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="62a4f-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="62a4f-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="62a4f-168">lastReportedDateTime</span></span>|<span data-ttu-id="62a4f-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62a4f-169">DateTimeOffset</span></span>|<span data-ttu-id="62a4f-170">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="62a4f-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="62a4f-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="62a4f-171">userPrincipalName</span></span>|<span data-ttu-id="62a4f-172">String</span><span class="sxs-lookup"><span data-stu-id="62a4f-172">String</span></span>|<span data-ttu-id="62a4f-173">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="62a4f-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="62a4f-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="62a4f-174">Response</span></span>
<span data-ttu-id="62a4f-175">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="62a4f-175">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62a4f-176">Пример</span><span class="sxs-lookup"><span data-stu-id="62a4f-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="62a4f-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="62a4f-177">Request</span></span>
<span data-ttu-id="62a4f-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62a4f-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62a4f-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="62a4f-179">Response</span></span>
<span data-ttu-id="62a4f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="62a4f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




