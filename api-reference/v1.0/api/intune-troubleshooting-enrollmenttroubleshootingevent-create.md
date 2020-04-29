---
title: Создание объекта enrollmentTroubleshootingEvent
description: Создание объекта enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 770a784cacd9b74529142e3b81ca3cef0f76af92
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43368746"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="3eff4-103">Создание объекта enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3eff4-103">Create enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="3eff4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eff4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3eff4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3eff4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eff4-106">Создание объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3eff4-106">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3eff4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3eff4-107">Prerequisites</span></span>
<span data-ttu-id="3eff4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eff4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eff4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3eff4-110">Permission type</span></span>|<span data-ttu-id="3eff4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3eff4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eff4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3eff4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3eff4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eff4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3eff4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3eff4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eff4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eff4-115">Not supported.</span></span>|
|<span data-ttu-id="3eff4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3eff4-116">Application</span></span>|<span data-ttu-id="3eff4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eff4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eff4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3eff4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="3eff4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3eff4-119">Request headers</span></span>
|<span data-ttu-id="3eff4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3eff4-120">Header</span></span>|<span data-ttu-id="3eff4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3eff4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eff4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3eff4-122">Authorization</span></span>|<span data-ttu-id="3eff4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3eff4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eff4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3eff4-124">Accept</span></span>|<span data-ttu-id="3eff4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3eff4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eff4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3eff4-126">Request body</span></span>
<span data-ttu-id="3eff4-127">В теле запроса добавьте представление объекта enrollmentTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3eff4-127">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="3eff4-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="3eff4-128">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="3eff4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3eff4-129">Property</span></span>|<span data-ttu-id="3eff4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3eff4-130">Type</span></span>|<span data-ttu-id="3eff4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3eff4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eff4-132">id</span><span class="sxs-lookup"><span data-stu-id="3eff4-132">id</span></span>|<span data-ttu-id="3eff4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="3eff4-133">String</span></span>|<span data-ttu-id="3eff4-134">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3eff4-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3eff4-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="3eff4-135">eventDateTime</span></span>|<span data-ttu-id="3eff4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eff4-136">DateTimeOffset</span></span>|<span data-ttu-id="3eff4-137">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="3eff4-137">Time when the event occurred .</span></span> <span data-ttu-id="3eff4-138">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3eff4-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3eff4-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="3eff4-139">correlationId</span></span>|<span data-ttu-id="3eff4-140">String</span><span class="sxs-lookup"><span data-stu-id="3eff4-140">String</span></span>|<span data-ttu-id="3eff4-141">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="3eff4-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="3eff4-142">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="3eff4-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="3eff4-143">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3eff4-143">managedDeviceIdentifier</span></span>|<span data-ttu-id="3eff4-144">String</span><span class="sxs-lookup"><span data-stu-id="3eff4-144">String</span></span>|<span data-ttu-id="3eff4-145">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="3eff4-145">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="3eff4-146">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="3eff4-146">operatingSystem</span></span>|<span data-ttu-id="3eff4-147">String</span><span class="sxs-lookup"><span data-stu-id="3eff4-147">String</span></span>|<span data-ttu-id="3eff4-148">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="3eff4-148">Operating System.</span></span>|
|<span data-ttu-id="3eff4-149">osVersion</span><span class="sxs-lookup"><span data-stu-id="3eff4-149">osVersion</span></span>|<span data-ttu-id="3eff4-150">String</span><span class="sxs-lookup"><span data-stu-id="3eff4-150">String</span></span>|<span data-ttu-id="3eff4-151">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="3eff4-151">OS Version.</span></span>|
|<span data-ttu-id="3eff4-152">userId</span><span class="sxs-lookup"><span data-stu-id="3eff4-152">userId</span></span>|<span data-ttu-id="3eff4-153">String</span><span class="sxs-lookup"><span data-stu-id="3eff4-153">String</span></span>|<span data-ttu-id="3eff4-154">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="3eff4-154">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="3eff4-155">deviceId</span><span class="sxs-lookup"><span data-stu-id="3eff4-155">deviceId</span></span>|<span data-ttu-id="3eff4-156">String</span><span class="sxs-lookup"><span data-stu-id="3eff4-156">String</span></span>|<span data-ttu-id="3eff4-157">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3eff4-157">Azure AD device identifier.</span></span>|
|<span data-ttu-id="3eff4-158">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="3eff4-158">enrollmentType</span></span>|[<span data-ttu-id="3eff4-159">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3eff4-159">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="3eff4-160">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="3eff4-160">Type of the enrollment.</span></span> <span data-ttu-id="3eff4-161">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="3eff4-161">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="3eff4-162">failureCategory</span><span class="sxs-lookup"><span data-stu-id="3eff4-162">failureCategory</span></span>|[<span data-ttu-id="3eff4-163">девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="3eff4-163">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="3eff4-164">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="3eff4-164">Highlevel failure category.</span></span> <span data-ttu-id="3eff4-165">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="3eff4-165">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="3eff4-166">failureReason</span><span class="sxs-lookup"><span data-stu-id="3eff4-166">failureReason</span></span>|<span data-ttu-id="3eff4-167">String</span><span class="sxs-lookup"><span data-stu-id="3eff4-167">String</span></span>|<span data-ttu-id="3eff4-168">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="3eff4-168">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="3eff4-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eff4-169">Response</span></span>
<span data-ttu-id="3eff4-170">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3eff4-170">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eff4-171">Пример</span><span class="sxs-lookup"><span data-stu-id="3eff4-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="3eff4-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="3eff4-172">Request</span></span>
<span data-ttu-id="3eff4-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3eff4-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```

### <a name="response"></a><span data-ttu-id="3eff4-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eff4-174">Response</span></span>
<span data-ttu-id="3eff4-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3eff4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 558

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```






