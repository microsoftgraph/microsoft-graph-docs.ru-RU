---
title: Обновление enrollmentTroubleshootingEvent
description: Обновление свойств объекта enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 785835eb0daabd55add7d7d903990abd4725ab9c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886207"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="4817c-103">Обновление enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4817c-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="4817c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4817c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4817c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4817c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4817c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4817c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4817c-107">Обновление свойств объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="4817c-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4817c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4817c-108">Prerequisites</span></span>
<span data-ttu-id="4817c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4817c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4817c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4817c-111">Permission type</span></span>|<span data-ttu-id="4817c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4817c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4817c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4817c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4817c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4817c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4817c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4817c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4817c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4817c-116">Not supported.</span></span>|
|<span data-ttu-id="4817c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4817c-117">Application</span></span>|<span data-ttu-id="4817c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4817c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4817c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4817c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="4817c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4817c-120">Request headers</span></span>
|<span data-ttu-id="4817c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4817c-121">Header</span></span>|<span data-ttu-id="4817c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4817c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4817c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4817c-123">Authorization</span></span>|<span data-ttu-id="4817c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4817c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4817c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4817c-125">Accept</span></span>|<span data-ttu-id="4817c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4817c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4817c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4817c-127">Request body</span></span>
<span data-ttu-id="4817c-128">В теле запроса добавьте представление объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4817c-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="4817c-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="4817c-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="4817c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4817c-130">Property</span></span>|<span data-ttu-id="4817c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4817c-131">Type</span></span>|<span data-ttu-id="4817c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4817c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4817c-133">id</span><span class="sxs-lookup"><span data-stu-id="4817c-133">id</span></span>|<span data-ttu-id="4817c-134">String</span><span class="sxs-lookup"><span data-stu-id="4817c-134">String</span></span>|<span data-ttu-id="4817c-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="4817c-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4817c-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="4817c-136">eventDateTime</span></span>|<span data-ttu-id="4817c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4817c-137">DateTimeOffset</span></span>|<span data-ttu-id="4817c-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="4817c-138">Time when the event occurred .</span></span> <span data-ttu-id="4817c-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="4817c-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4817c-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="4817c-140">correlationId</span></span>|<span data-ttu-id="4817c-141">String</span><span class="sxs-lookup"><span data-stu-id="4817c-141">String</span></span>|<span data-ttu-id="4817c-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="4817c-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="4817c-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="4817c-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="4817c-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4817c-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="4817c-145">String</span><span class="sxs-lookup"><span data-stu-id="4817c-145">String</span></span>|<span data-ttu-id="4817c-146">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="4817c-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="4817c-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="4817c-147">operatingSystem</span></span>|<span data-ttu-id="4817c-148">String</span><span class="sxs-lookup"><span data-stu-id="4817c-148">String</span></span>|<span data-ttu-id="4817c-149">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="4817c-149">Operating System.</span></span>|
|<span data-ttu-id="4817c-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="4817c-150">osVersion</span></span>|<span data-ttu-id="4817c-151">String</span><span class="sxs-lookup"><span data-stu-id="4817c-151">String</span></span>|<span data-ttu-id="4817c-152">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="4817c-152">OS Version.</span></span>|
|<span data-ttu-id="4817c-153">userId</span><span class="sxs-lookup"><span data-stu-id="4817c-153">userId</span></span>|<span data-ttu-id="4817c-154">String</span><span class="sxs-lookup"><span data-stu-id="4817c-154">String</span></span>|<span data-ttu-id="4817c-155">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="4817c-155">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="4817c-156">deviceId</span><span class="sxs-lookup"><span data-stu-id="4817c-156">deviceId</span></span>|<span data-ttu-id="4817c-157">String</span><span class="sxs-lookup"><span data-stu-id="4817c-157">String</span></span>|<span data-ttu-id="4817c-158">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4817c-158">Azure AD device identifier.</span></span>|
|<span data-ttu-id="4817c-159">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="4817c-159">enrollmentType</span></span>|[<span data-ttu-id="4817c-160">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4817c-160">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="4817c-161">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="4817c-161">Type of the enrollment.</span></span> <span data-ttu-id="4817c-162">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="4817c-162">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="4817c-163">failureCategory</span><span class="sxs-lookup"><span data-stu-id="4817c-163">failureCategory</span></span>|[<span data-ttu-id="4817c-164">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="4817c-164">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="4817c-165">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="4817c-165">Highlevel failure category.</span></span> <span data-ttu-id="4817c-166">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="4817c-166">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="4817c-167">failureReason</span><span class="sxs-lookup"><span data-stu-id="4817c-167">failureReason</span></span>|<span data-ttu-id="4817c-168">String</span><span class="sxs-lookup"><span data-stu-id="4817c-168">String</span></span>|<span data-ttu-id="4817c-169">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="4817c-169">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="4817c-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="4817c-170">Response</span></span>
<span data-ttu-id="4817c-171">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4817c-171">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4817c-172">Пример</span><span class="sxs-lookup"><span data-stu-id="4817c-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="4817c-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="4817c-173">Request</span></span>
<span data-ttu-id="4817c-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4817c-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="4817c-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="4817c-175">Response</span></span>
<span data-ttu-id="4817c-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4817c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





