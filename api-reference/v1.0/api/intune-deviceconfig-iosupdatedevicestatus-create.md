---
title: Создание объекта iosUpdateDeviceStatus
description: Создание объекта iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc97746eb2f22447f0d77cfd873cd2156ef15c73
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262624"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="f66f2-103">Создание объекта iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="f66f2-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="f66f2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f66f2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f66f2-105">Создание объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f66f2-105">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f66f2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f66f2-106">Prerequisites</span></span>
<span data-ttu-id="f66f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f66f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f66f2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f66f2-109">Permission type</span></span>|<span data-ttu-id="f66f2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f66f2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f66f2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f66f2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f66f2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f66f2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f66f2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f66f2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f66f2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f66f2-114">Not supported.</span></span>|
|<span data-ttu-id="f66f2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f66f2-115">Application</span></span>|<span data-ttu-id="f66f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f66f2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f66f2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f66f2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f66f2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f66f2-118">Request headers</span></span>
|<span data-ttu-id="f66f2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f66f2-119">Header</span></span>|<span data-ttu-id="f66f2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f66f2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f66f2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f66f2-121">Authorization</span></span>|<span data-ttu-id="f66f2-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f66f2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f66f2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f66f2-123">Accept</span></span>|<span data-ttu-id="f66f2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f66f2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f66f2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f66f2-125">Request body</span></span>
<span data-ttu-id="f66f2-126">В теле запроса добавьте представление объекта iosUpdateDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f66f2-126">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="f66f2-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="f66f2-127">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="f66f2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f66f2-128">Property</span></span>|<span data-ttu-id="f66f2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f66f2-129">Type</span></span>|<span data-ttu-id="f66f2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f66f2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f66f2-131">id</span><span class="sxs-lookup"><span data-stu-id="f66f2-131">id</span></span>|<span data-ttu-id="f66f2-132">Строка</span><span class="sxs-lookup"><span data-stu-id="f66f2-132">String</span></span>|<span data-ttu-id="f66f2-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f66f2-133">Key of the entity.</span></span>|
|<span data-ttu-id="f66f2-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="f66f2-134">installStatus</span></span>|[<span data-ttu-id="f66f2-135">Иосупдатесинсталлстатус</span><span class="sxs-lookup"><span data-stu-id="f66f2-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="f66f2-136">Состояние установки в отчете о политике.</span><span class="sxs-lookup"><span data-stu-id="f66f2-136">The installation status of the policy report.</span></span> <span data-ttu-id="f66f2-137">Возможные значения: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`,. `sharedDeviceUserLoggedInError`</span><span class="sxs-lookup"><span data-stu-id="f66f2-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="f66f2-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="f66f2-138">osVersion</span></span>|<span data-ttu-id="f66f2-139">String</span><span class="sxs-lookup"><span data-stu-id="f66f2-139">String</span></span>|<span data-ttu-id="f66f2-140">Версия устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="f66f2-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="f66f2-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="f66f2-141">deviceId</span></span>|<span data-ttu-id="f66f2-142">String</span><span class="sxs-lookup"><span data-stu-id="f66f2-142">String</span></span>|<span data-ttu-id="f66f2-143">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="f66f2-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="f66f2-144">userId</span><span class="sxs-lookup"><span data-stu-id="f66f2-144">userId</span></span>|<span data-ttu-id="f66f2-145">String</span><span class="sxs-lookup"><span data-stu-id="f66f2-145">String</span></span>|<span data-ttu-id="f66f2-146">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="f66f2-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="f66f2-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f66f2-147">deviceDisplayName</span></span>|<span data-ttu-id="f66f2-148">String</span><span class="sxs-lookup"><span data-stu-id="f66f2-148">String</span></span>|<span data-ttu-id="f66f2-149">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="f66f2-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f66f2-150">userName</span><span class="sxs-lookup"><span data-stu-id="f66f2-150">userName</span></span>|<span data-ttu-id="f66f2-151">String</span><span class="sxs-lookup"><span data-stu-id="f66f2-151">String</span></span>|<span data-ttu-id="f66f2-152">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="f66f2-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="f66f2-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f66f2-153">deviceModel</span></span>|<span data-ttu-id="f66f2-154">String</span><span class="sxs-lookup"><span data-stu-id="f66f2-154">String</span></span>|<span data-ttu-id="f66f2-155">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="f66f2-155">The device model that is being reported</span></span>|
|<span data-ttu-id="f66f2-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f66f2-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f66f2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f66f2-157">DateTimeOffset</span></span>|<span data-ttu-id="f66f2-158">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f66f2-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f66f2-159">status</span><span class="sxs-lookup"><span data-stu-id="f66f2-159">status</span></span>|[<span data-ttu-id="f66f2-160">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="f66f2-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f66f2-161">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="f66f2-161">Compliance status of the policy report.</span></span> <span data-ttu-id="f66f2-162">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f66f2-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f66f2-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f66f2-163">lastReportedDateTime</span></span>|<span data-ttu-id="f66f2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f66f2-164">DateTimeOffset</span></span>|<span data-ttu-id="f66f2-165">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="f66f2-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f66f2-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f66f2-166">userPrincipalName</span></span>|<span data-ttu-id="f66f2-167">Строка</span><span class="sxs-lookup"><span data-stu-id="f66f2-167">String</span></span>|<span data-ttu-id="f66f2-168">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="f66f2-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f66f2-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="f66f2-169">Response</span></span>
<span data-ttu-id="f66f2-170">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f66f2-170">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f66f2-171">Пример</span><span class="sxs-lookup"><span data-stu-id="f66f2-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="f66f2-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="f66f2-172">Request</span></span>
<span data-ttu-id="f66f2-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f66f2-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f66f2-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="f66f2-174">Response</span></span>
<span data-ttu-id="f66f2-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f66f2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



