---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
author: tfitzmac
ms.openlocfilehash: d2fab69e918d92e07ed28f3e12aa59db9d50c53b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350213"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="8f140-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8f140-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="8f140-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f140-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f140-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f140-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f140-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8f140-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f140-107">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8f140-107">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f140-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8f140-108">Prerequisites</span></span>
<span data-ttu-id="8f140-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f140-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f140-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f140-111">Permission type</span></span>|<span data-ttu-id="8f140-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f140-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f140-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f140-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f140-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f140-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f140-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f140-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f140-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f140-116">Not supported.</span></span>|
|<span data-ttu-id="8f140-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f140-117">Application</span></span>|<span data-ttu-id="8f140-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f140-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f140-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f140-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="8f140-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f140-120">Request headers</span></span>
|<span data-ttu-id="8f140-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f140-121">Header</span></span>|<span data-ttu-id="8f140-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8f140-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f140-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f140-123">Authorization</span></span>|<span data-ttu-id="8f140-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8f140-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f140-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f140-125">Accept</span></span>|<span data-ttu-id="8f140-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f140-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f140-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f140-127">Request body</span></span>
<span data-ttu-id="8f140-128">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f140-128">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="8f140-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8f140-129">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="8f140-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f140-130">Property</span></span>|<span data-ttu-id="8f140-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8f140-131">Type</span></span>|<span data-ttu-id="8f140-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8f140-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f140-133">id</span><span class="sxs-lookup"><span data-stu-id="8f140-133">id</span></span>|<span data-ttu-id="8f140-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8f140-134">String</span></span>|<span data-ttu-id="8f140-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8f140-135">Key of the entity.</span></span>|
|<span data-ttu-id="8f140-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="8f140-136">installStatus</span></span>|[<span data-ttu-id="8f140-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="8f140-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="8f140-138">Состояние установки в отчете о политике.</span><span class="sxs-lookup"><span data-stu-id="8f140-138">The installation status of the policy report.</span></span> <span data-ttu-id="8f140-139">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="8f140-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="8f140-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="8f140-140">osVersion</span></span>|<span data-ttu-id="8f140-141">String</span><span class="sxs-lookup"><span data-stu-id="8f140-141">String</span></span>|<span data-ttu-id="8f140-142">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="8f140-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="8f140-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="8f140-143">deviceId</span></span>|<span data-ttu-id="8f140-144">String</span><span class="sxs-lookup"><span data-stu-id="8f140-144">String</span></span>|<span data-ttu-id="8f140-145">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="8f140-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="8f140-146">userId</span><span class="sxs-lookup"><span data-stu-id="8f140-146">userId</span></span>|<span data-ttu-id="8f140-147">String</span><span class="sxs-lookup"><span data-stu-id="8f140-147">String</span></span>|<span data-ttu-id="8f140-148">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="8f140-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="8f140-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8f140-149">deviceDisplayName</span></span>|<span data-ttu-id="8f140-150">String</span><span class="sxs-lookup"><span data-stu-id="8f140-150">String</span></span>|<span data-ttu-id="8f140-151">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="8f140-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="8f140-152">userName</span><span class="sxs-lookup"><span data-stu-id="8f140-152">userName</span></span>|<span data-ttu-id="8f140-153">String</span><span class="sxs-lookup"><span data-stu-id="8f140-153">String</span></span>|<span data-ttu-id="8f140-154">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="8f140-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="8f140-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8f140-155">deviceModel</span></span>|<span data-ttu-id="8f140-156">String</span><span class="sxs-lookup"><span data-stu-id="8f140-156">String</span></span>|<span data-ttu-id="8f140-157">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="8f140-157">The device model that is being reported</span></span>|
|<span data-ttu-id="8f140-158">platform</span><span class="sxs-lookup"><span data-stu-id="8f140-158">platform</span></span>|<span data-ttu-id="8f140-159">Int32</span><span class="sxs-lookup"><span data-stu-id="8f140-159">Int32</span></span>|<span data-ttu-id="8f140-160">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="8f140-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="8f140-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8f140-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8f140-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f140-162">DateTimeOffset</span></span>|<span data-ttu-id="8f140-163">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8f140-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="8f140-164">status</span><span class="sxs-lookup"><span data-stu-id="8f140-164">status</span></span>|[<span data-ttu-id="8f140-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8f140-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8f140-166">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="8f140-166">Compliance status of the policy report.</span></span> <span data-ttu-id="8f140-167">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8f140-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8f140-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f140-168">lastReportedDateTime</span></span>|<span data-ttu-id="8f140-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f140-169">DateTimeOffset</span></span>|<span data-ttu-id="8f140-170">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="8f140-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="8f140-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8f140-171">userPrincipalName</span></span>|<span data-ttu-id="8f140-172">String</span><span class="sxs-lookup"><span data-stu-id="8f140-172">String</span></span>|<span data-ttu-id="8f140-173">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="8f140-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="8f140-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f140-174">Response</span></span>
<span data-ttu-id="8f140-175">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8f140-175">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f140-176">Пример</span><span class="sxs-lookup"><span data-stu-id="8f140-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f140-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f140-177">Request</span></span>
<span data-ttu-id="8f140-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f140-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
Content-type: application/json
Content-length: 510

{
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

### <a name="response"></a><span data-ttu-id="8f140-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f140-179">Response</span></span>
<span data-ttu-id="8f140-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8f140-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





