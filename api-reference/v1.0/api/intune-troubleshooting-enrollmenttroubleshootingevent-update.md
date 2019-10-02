---
title: Обновление enrollmentTroubleshootingEvent
description: Обновление свойств объекта enrollmentTroubleshootingEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f53296202b3bfddb7632ff951258f269cdb11bd
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360995"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="fd03a-103">Обновление enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="fd03a-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="fd03a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd03a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd03a-105">Обновление свойств объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="fd03a-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd03a-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fd03a-106">Prerequisites</span></span>
<span data-ttu-id="fd03a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd03a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd03a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd03a-109">Permission type</span></span>|<span data-ttu-id="fd03a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd03a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd03a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd03a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fd03a-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd03a-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fd03a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd03a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd03a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd03a-114">Not supported.</span></span>|
|<span data-ttu-id="fd03a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd03a-115">Application</span></span>|<span data-ttu-id="fd03a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd03a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd03a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd03a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="fd03a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd03a-118">Request headers</span></span>
|<span data-ttu-id="fd03a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd03a-119">Header</span></span>|<span data-ttu-id="fd03a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fd03a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd03a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd03a-121">Authorization</span></span>|<span data-ttu-id="fd03a-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd03a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd03a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fd03a-123">Accept</span></span>|<span data-ttu-id="fd03a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fd03a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd03a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd03a-125">Request body</span></span>
<span data-ttu-id="fd03a-126">В теле запроса добавьте представление объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd03a-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="fd03a-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="fd03a-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="fd03a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd03a-128">Property</span></span>|<span data-ttu-id="fd03a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="fd03a-129">Type</span></span>|<span data-ttu-id="fd03a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fd03a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd03a-131">id</span><span class="sxs-lookup"><span data-stu-id="fd03a-131">id</span></span>|<span data-ttu-id="fd03a-132">Строка</span><span class="sxs-lookup"><span data-stu-id="fd03a-132">String</span></span>|<span data-ttu-id="fd03a-133">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="fd03a-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="fd03a-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="fd03a-134">eventDateTime</span></span>|<span data-ttu-id="fd03a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd03a-135">DateTimeOffset</span></span>|<span data-ttu-id="fd03a-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="fd03a-136">Time when the event occurred .</span></span> <span data-ttu-id="fd03a-137">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="fd03a-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="fd03a-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="fd03a-138">correlationId</span></span>|<span data-ttu-id="fd03a-139">String</span><span class="sxs-lookup"><span data-stu-id="fd03a-139">String</span></span>|<span data-ttu-id="fd03a-140">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="fd03a-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="fd03a-141">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="fd03a-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="fd03a-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="fd03a-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="fd03a-143">String</span><span class="sxs-lookup"><span data-stu-id="fd03a-143">String</span></span>|<span data-ttu-id="fd03a-144">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="fd03a-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="fd03a-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="fd03a-145">operatingSystem</span></span>|<span data-ttu-id="fd03a-146">String</span><span class="sxs-lookup"><span data-stu-id="fd03a-146">String</span></span>|<span data-ttu-id="fd03a-147">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="fd03a-147">Operating System.</span></span>|
|<span data-ttu-id="fd03a-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="fd03a-148">osVersion</span></span>|<span data-ttu-id="fd03a-149">String</span><span class="sxs-lookup"><span data-stu-id="fd03a-149">String</span></span>|<span data-ttu-id="fd03a-150">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="fd03a-150">OS Version.</span></span>|
|<span data-ttu-id="fd03a-151">userId</span><span class="sxs-lookup"><span data-stu-id="fd03a-151">userId</span></span>|<span data-ttu-id="fd03a-152">String</span><span class="sxs-lookup"><span data-stu-id="fd03a-152">String</span></span>|<span data-ttu-id="fd03a-153">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="fd03a-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="fd03a-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="fd03a-154">deviceId</span></span>|<span data-ttu-id="fd03a-155">String</span><span class="sxs-lookup"><span data-stu-id="fd03a-155">String</span></span>|<span data-ttu-id="fd03a-156">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fd03a-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="fd03a-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="fd03a-157">enrollmentType</span></span>|[<span data-ttu-id="fd03a-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="fd03a-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="fd03a-159">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="fd03a-159">Type of the enrollment.</span></span> <span data-ttu-id="fd03a-160">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="fd03a-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="fd03a-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="fd03a-161">failureCategory</span></span>|[<span data-ttu-id="fd03a-162">девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="fd03a-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="fd03a-163">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="fd03a-163">Highlevel failure category.</span></span> <span data-ttu-id="fd03a-164">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="fd03a-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="fd03a-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="fd03a-165">failureReason</span></span>|<span data-ttu-id="fd03a-166">String</span><span class="sxs-lookup"><span data-stu-id="fd03a-166">String</span></span>|<span data-ttu-id="fd03a-167">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="fd03a-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="fd03a-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd03a-168">Response</span></span>
<span data-ttu-id="fd03a-169">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fd03a-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd03a-170">Пример</span><span class="sxs-lookup"><span data-stu-id="fd03a-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd03a-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd03a-171">Request</span></span>
<span data-ttu-id="fd03a-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd03a-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="fd03a-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd03a-173">Response</span></span>
<span data-ttu-id="fd03a-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd03a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




