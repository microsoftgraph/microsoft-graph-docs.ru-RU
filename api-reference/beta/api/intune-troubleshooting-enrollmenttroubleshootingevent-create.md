---
title: Создание объекта enrollmentTroubleshootingEvent
description: Создание объекта enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ae80e2084945b1dd5fb0259b16b178ab2d38ec5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924568"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="91794-103">Создание объекта enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="91794-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="91794-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91794-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91794-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91794-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91794-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="91794-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91794-107">Создание объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="91794-107">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91794-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="91794-108">Prerequisites</span></span>
<span data-ttu-id="91794-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91794-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91794-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91794-111">Permission type</span></span>|<span data-ttu-id="91794-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91794-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91794-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91794-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91794-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91794-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="91794-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91794-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91794-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91794-116">Not supported.</span></span>|
|<span data-ttu-id="91794-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91794-117">Application</span></span>|<span data-ttu-id="91794-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91794-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91794-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91794-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="91794-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91794-120">Request headers</span></span>
|<span data-ttu-id="91794-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91794-121">Header</span></span>|<span data-ttu-id="91794-122">Значение</span><span class="sxs-lookup"><span data-stu-id="91794-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91794-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91794-123">Authorization</span></span>|<span data-ttu-id="91794-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="91794-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91794-125">Accept</span><span class="sxs-lookup"><span data-stu-id="91794-125">Accept</span></span>|<span data-ttu-id="91794-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91794-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91794-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91794-127">Request body</span></span>
<span data-ttu-id="91794-128">В теле запроса добавьте представление объекта enrollmentTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91794-128">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="91794-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="91794-129">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="91794-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="91794-130">Property</span></span>|<span data-ttu-id="91794-131">Тип</span><span class="sxs-lookup"><span data-stu-id="91794-131">Type</span></span>|<span data-ttu-id="91794-132">Описание</span><span class="sxs-lookup"><span data-stu-id="91794-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91794-133">id</span><span class="sxs-lookup"><span data-stu-id="91794-133">id</span></span>|<span data-ttu-id="91794-134">String</span><span class="sxs-lookup"><span data-stu-id="91794-134">String</span></span>|<span data-ttu-id="91794-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="91794-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="91794-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="91794-136">eventDateTime</span></span>|<span data-ttu-id="91794-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91794-137">DateTimeOffset</span></span>|<span data-ttu-id="91794-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="91794-138">Time when the event occurred .</span></span> <span data-ttu-id="91794-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="91794-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="91794-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="91794-140">correlationId</span></span>|<span data-ttu-id="91794-141">String</span><span class="sxs-lookup"><span data-stu-id="91794-141">String</span></span>|<span data-ttu-id="91794-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="91794-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="91794-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="91794-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="91794-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="91794-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="91794-145">String</span><span class="sxs-lookup"><span data-stu-id="91794-145">String</span></span>|<span data-ttu-id="91794-146">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="91794-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="91794-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="91794-147">operatingSystem</span></span>|<span data-ttu-id="91794-148">String</span><span class="sxs-lookup"><span data-stu-id="91794-148">String</span></span>|<span data-ttu-id="91794-149">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="91794-149">Operating System.</span></span>|
|<span data-ttu-id="91794-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="91794-150">osVersion</span></span>|<span data-ttu-id="91794-151">String</span><span class="sxs-lookup"><span data-stu-id="91794-151">String</span></span>|<span data-ttu-id="91794-152">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="91794-152">OS Version.</span></span>|
|<span data-ttu-id="91794-153">userId</span><span class="sxs-lookup"><span data-stu-id="91794-153">userId</span></span>|<span data-ttu-id="91794-154">String</span><span class="sxs-lookup"><span data-stu-id="91794-154">String</span></span>|<span data-ttu-id="91794-155">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="91794-155">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="91794-156">deviceId</span><span class="sxs-lookup"><span data-stu-id="91794-156">deviceId</span></span>|<span data-ttu-id="91794-157">String</span><span class="sxs-lookup"><span data-stu-id="91794-157">String</span></span>|<span data-ttu-id="91794-158">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="91794-158">Azure AD device identifier.</span></span>|
|<span data-ttu-id="91794-159">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="91794-159">enrollmentType</span></span>|[<span data-ttu-id="91794-160">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="91794-160">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="91794-161">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="91794-161">Type of the enrollment.</span></span> <span data-ttu-id="91794-162">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="91794-162">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="91794-163">failureCategory</span><span class="sxs-lookup"><span data-stu-id="91794-163">failureCategory</span></span>|[<span data-ttu-id="91794-164">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="91794-164">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="91794-165">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="91794-165">Highlevel failure category.</span></span> <span data-ttu-id="91794-166">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="91794-166">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="91794-167">failureReason</span><span class="sxs-lookup"><span data-stu-id="91794-167">failureReason</span></span>|<span data-ttu-id="91794-168">String</span><span class="sxs-lookup"><span data-stu-id="91794-168">String</span></span>|<span data-ttu-id="91794-169">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="91794-169">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="91794-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="91794-170">Response</span></span>
<span data-ttu-id="91794-171">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91794-171">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91794-172">Пример</span><span class="sxs-lookup"><span data-stu-id="91794-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="91794-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="91794-173">Request</span></span>
<span data-ttu-id="91794-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91794-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="91794-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="91794-175">Response</span></span>
<span data-ttu-id="91794-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="91794-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





