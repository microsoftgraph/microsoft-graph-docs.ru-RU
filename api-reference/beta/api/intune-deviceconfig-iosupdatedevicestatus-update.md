---
title: Update iosUpdateDeviceStatus
description: Обновление свойств объекта iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b4b20782a39c2ed220f4bfdc6055fe5885d2fc9c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939149"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="2df67-103">Update iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2df67-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="2df67-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2df67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2df67-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2df67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2df67-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2df67-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2df67-107">Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="2df67-107">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2df67-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2df67-108">Prerequisites</span></span>
<span data-ttu-id="2df67-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df67-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2df67-111">Permission type</span></span>|<span data-ttu-id="2df67-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2df67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2df67-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2df67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2df67-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df67-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2df67-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2df67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2df67-116">Not supported.</span></span>|
|<span data-ttu-id="2df67-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2df67-117">Application</span></span>|<span data-ttu-id="2df67-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2df67-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2df67-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2df67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2df67-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2df67-120">Request headers</span></span>
|<span data-ttu-id="2df67-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2df67-121">Header</span></span>|<span data-ttu-id="2df67-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2df67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2df67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2df67-123">Authorization</span></span>|<span data-ttu-id="2df67-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2df67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2df67-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2df67-125">Accept</span></span>|<span data-ttu-id="2df67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2df67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2df67-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2df67-127">Request body</span></span>
<span data-ttu-id="2df67-128">В теле запроса добавьте представление объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2df67-128">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="2df67-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="2df67-129">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="2df67-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2df67-130">Property</span></span>|<span data-ttu-id="2df67-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2df67-131">Type</span></span>|<span data-ttu-id="2df67-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2df67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2df67-133">id</span><span class="sxs-lookup"><span data-stu-id="2df67-133">id</span></span>|<span data-ttu-id="2df67-134">String</span><span class="sxs-lookup"><span data-stu-id="2df67-134">String</span></span>|<span data-ttu-id="2df67-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2df67-135">Key of the entity.</span></span>|
|<span data-ttu-id="2df67-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="2df67-136">installStatus</span></span>|[<span data-ttu-id="2df67-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2df67-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="2df67-138">Состояние установки в отчете о политике.</span><span class="sxs-lookup"><span data-stu-id="2df67-138">The installation status of the policy report.</span></span> <span data-ttu-id="2df67-139">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="2df67-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="2df67-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="2df67-140">osVersion</span></span>|<span data-ttu-id="2df67-141">String</span><span class="sxs-lookup"><span data-stu-id="2df67-141">String</span></span>|<span data-ttu-id="2df67-142">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="2df67-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="2df67-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="2df67-143">deviceId</span></span>|<span data-ttu-id="2df67-144">String</span><span class="sxs-lookup"><span data-stu-id="2df67-144">String</span></span>|<span data-ttu-id="2df67-145">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="2df67-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="2df67-146">userId</span><span class="sxs-lookup"><span data-stu-id="2df67-146">userId</span></span>|<span data-ttu-id="2df67-147">String</span><span class="sxs-lookup"><span data-stu-id="2df67-147">String</span></span>|<span data-ttu-id="2df67-148">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="2df67-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="2df67-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2df67-149">deviceDisplayName</span></span>|<span data-ttu-id="2df67-150">String</span><span class="sxs-lookup"><span data-stu-id="2df67-150">String</span></span>|<span data-ttu-id="2df67-151">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="2df67-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2df67-152">userName</span><span class="sxs-lookup"><span data-stu-id="2df67-152">userName</span></span>|<span data-ttu-id="2df67-153">String</span><span class="sxs-lookup"><span data-stu-id="2df67-153">String</span></span>|<span data-ttu-id="2df67-154">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="2df67-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="2df67-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2df67-155">deviceModel</span></span>|<span data-ttu-id="2df67-156">String</span><span class="sxs-lookup"><span data-stu-id="2df67-156">String</span></span>|<span data-ttu-id="2df67-157">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="2df67-157">The device model that is being reported</span></span>|
|<span data-ttu-id="2df67-158">platform</span><span class="sxs-lookup"><span data-stu-id="2df67-158">platform</span></span>|<span data-ttu-id="2df67-159">Int32</span><span class="sxs-lookup"><span data-stu-id="2df67-159">Int32</span></span>|<span data-ttu-id="2df67-160">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="2df67-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="2df67-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2df67-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2df67-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2df67-162">DateTimeOffset</span></span>|<span data-ttu-id="2df67-163">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2df67-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="2df67-164">status</span><span class="sxs-lookup"><span data-stu-id="2df67-164">status</span></span>|[<span data-ttu-id="2df67-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2df67-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2df67-166">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="2df67-166">Compliance status of the policy report.</span></span> <span data-ttu-id="2df67-167">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2df67-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2df67-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2df67-168">lastReportedDateTime</span></span>|<span data-ttu-id="2df67-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2df67-169">DateTimeOffset</span></span>|<span data-ttu-id="2df67-170">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="2df67-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2df67-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2df67-171">userPrincipalName</span></span>|<span data-ttu-id="2df67-172">String</span><span class="sxs-lookup"><span data-stu-id="2df67-172">String</span></span>|<span data-ttu-id="2df67-173">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="2df67-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2df67-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="2df67-174">Response</span></span>
<span data-ttu-id="2df67-175">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2df67-175">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2df67-176">Пример</span><span class="sxs-lookup"><span data-stu-id="2df67-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="2df67-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="2df67-177">Request</span></span>
<span data-ttu-id="2df67-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2df67-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2df67-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="2df67-179">Response</span></span>
<span data-ttu-id="2df67-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2df67-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





