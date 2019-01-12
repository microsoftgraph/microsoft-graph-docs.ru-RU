---
title: Обновление enrollmentTroubleshootingEvent
description: Обновление свойств объекта enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 002f1e29c993326ab85d17d5092935525249a9db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939773"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="12aef-103">Обновление enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="12aef-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="12aef-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="12aef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12aef-105">Обновление свойств объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="12aef-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12aef-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12aef-106">Prerequisites</span></span>
<span data-ttu-id="12aef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12aef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12aef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12aef-109">Permission type</span></span>|<span data-ttu-id="12aef-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12aef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12aef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12aef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12aef-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12aef-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="12aef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12aef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12aef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12aef-114">Not supported.</span></span>|
|<span data-ttu-id="12aef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12aef-115">Application</span></span>|<span data-ttu-id="12aef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12aef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12aef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12aef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="12aef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12aef-118">Request headers</span></span>
|<span data-ttu-id="12aef-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12aef-119">Header</span></span>|<span data-ttu-id="12aef-120">Значение</span><span class="sxs-lookup"><span data-stu-id="12aef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12aef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="12aef-121">Authorization</span></span>|<span data-ttu-id="12aef-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="12aef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12aef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="12aef-123">Accept</span></span>|<span data-ttu-id="12aef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="12aef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12aef-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12aef-125">Request body</span></span>
<span data-ttu-id="12aef-126">В теле запроса добавьте представление объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12aef-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="12aef-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="12aef-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="12aef-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="12aef-128">Property</span></span>|<span data-ttu-id="12aef-129">Тип</span><span class="sxs-lookup"><span data-stu-id="12aef-129">Type</span></span>|<span data-ttu-id="12aef-130">Описание</span><span class="sxs-lookup"><span data-stu-id="12aef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12aef-131">id</span><span class="sxs-lookup"><span data-stu-id="12aef-131">id</span></span>|<span data-ttu-id="12aef-132">String</span><span class="sxs-lookup"><span data-stu-id="12aef-132">String</span></span>|<span data-ttu-id="12aef-133">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="12aef-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="12aef-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="12aef-134">eventDateTime</span></span>|<span data-ttu-id="12aef-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12aef-135">DateTimeOffset</span></span>|<span data-ttu-id="12aef-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="12aef-136">Time when the event occurred .</span></span> <span data-ttu-id="12aef-137">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="12aef-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="12aef-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="12aef-138">correlationId</span></span>|<span data-ttu-id="12aef-139">String</span><span class="sxs-lookup"><span data-stu-id="12aef-139">String</span></span>|<span data-ttu-id="12aef-140">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="12aef-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="12aef-141">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="12aef-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="12aef-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="12aef-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="12aef-143">String</span><span class="sxs-lookup"><span data-stu-id="12aef-143">String</span></span>|<span data-ttu-id="12aef-144">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="12aef-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="12aef-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="12aef-145">operatingSystem</span></span>|<span data-ttu-id="12aef-146">String</span><span class="sxs-lookup"><span data-stu-id="12aef-146">String</span></span>|<span data-ttu-id="12aef-147">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="12aef-147">Operating System.</span></span>|
|<span data-ttu-id="12aef-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="12aef-148">osVersion</span></span>|<span data-ttu-id="12aef-149">String</span><span class="sxs-lookup"><span data-stu-id="12aef-149">String</span></span>|<span data-ttu-id="12aef-150">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="12aef-150">OS Version.</span></span>|
|<span data-ttu-id="12aef-151">userId</span><span class="sxs-lookup"><span data-stu-id="12aef-151">userId</span></span>|<span data-ttu-id="12aef-152">String</span><span class="sxs-lookup"><span data-stu-id="12aef-152">String</span></span>|<span data-ttu-id="12aef-153">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="12aef-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="12aef-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="12aef-154">deviceId</span></span>|<span data-ttu-id="12aef-155">String</span><span class="sxs-lookup"><span data-stu-id="12aef-155">String</span></span>|<span data-ttu-id="12aef-156">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="12aef-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="12aef-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="12aef-157">enrollmentType</span></span>|[<span data-ttu-id="12aef-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="12aef-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="12aef-159">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="12aef-159">Type of the enrollment.</span></span> <span data-ttu-id="12aef-160">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="12aef-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="12aef-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="12aef-161">failureCategory</span></span>|[<span data-ttu-id="12aef-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="12aef-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="12aef-163">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="12aef-163">Highlevel failure category.</span></span> <span data-ttu-id="12aef-164">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="12aef-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="12aef-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="12aef-165">failureReason</span></span>|<span data-ttu-id="12aef-166">String</span><span class="sxs-lookup"><span data-stu-id="12aef-166">String</span></span>|<span data-ttu-id="12aef-167">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="12aef-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="12aef-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="12aef-168">Response</span></span>
<span data-ttu-id="12aef-169">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="12aef-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12aef-170">Пример</span><span class="sxs-lookup"><span data-stu-id="12aef-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="12aef-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="12aef-171">Request</span></span>
<span data-ttu-id="12aef-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12aef-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 440

{
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

### <a name="response"></a><span data-ttu-id="12aef-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="12aef-173">Response</span></span>
<span data-ttu-id="12aef-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="12aef-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



