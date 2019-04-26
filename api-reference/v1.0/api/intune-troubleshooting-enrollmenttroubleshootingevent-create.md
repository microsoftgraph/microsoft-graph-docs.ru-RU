---
title: Создание объекта enrollmentTroubleshootingEvent
description: Создание объекта enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 574e9c118601e68acdadeb7d1ccccd929438dbbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576551"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="b7537-103">Создание объекта enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="b7537-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="b7537-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7537-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7537-105">Создание объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="b7537-105">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7537-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b7537-106">Prerequisites</span></span>
<span data-ttu-id="b7537-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7537-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7537-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7537-109">Permission type</span></span>|<span data-ttu-id="b7537-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7537-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7537-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7537-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b7537-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7537-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b7537-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7537-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7537-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7537-114">Not supported.</span></span>|
|<span data-ttu-id="b7537-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7537-115">Application</span></span>|<span data-ttu-id="b7537-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7537-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7537-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7537-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="b7537-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7537-118">Request headers</span></span>
|<span data-ttu-id="b7537-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7537-119">Header</span></span>|<span data-ttu-id="b7537-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b7537-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7537-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7537-121">Authorization</span></span>|<span data-ttu-id="b7537-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7537-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7537-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b7537-123">Accept</span></span>|<span data-ttu-id="b7537-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b7537-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7537-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7537-125">Request body</span></span>
<span data-ttu-id="b7537-126">В теле запроса добавьте представление объекта enrollmentTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7537-126">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="b7537-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="b7537-127">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="b7537-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7537-128">Property</span></span>|<span data-ttu-id="b7537-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b7537-129">Type</span></span>|<span data-ttu-id="b7537-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b7537-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7537-131">id</span><span class="sxs-lookup"><span data-stu-id="b7537-131">id</span></span>|<span data-ttu-id="b7537-132">String</span><span class="sxs-lookup"><span data-stu-id="b7537-132">String</span></span>|<span data-ttu-id="b7537-133">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="b7537-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b7537-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b7537-134">eventDateTime</span></span>|<span data-ttu-id="b7537-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7537-135">DateTimeOffset</span></span>|<span data-ttu-id="b7537-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="b7537-136">Time when the event occurred .</span></span> <span data-ttu-id="b7537-137">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="b7537-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b7537-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="b7537-138">correlationId</span></span>|<span data-ttu-id="b7537-139">String</span><span class="sxs-lookup"><span data-stu-id="b7537-139">String</span></span>|<span data-ttu-id="b7537-140">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="b7537-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="b7537-141">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="b7537-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b7537-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b7537-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="b7537-143">String</span><span class="sxs-lookup"><span data-stu-id="b7537-143">String</span></span>|<span data-ttu-id="b7537-144">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="b7537-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="b7537-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b7537-145">operatingSystem</span></span>|<span data-ttu-id="b7537-146">String</span><span class="sxs-lookup"><span data-stu-id="b7537-146">String</span></span>|<span data-ttu-id="b7537-147">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="b7537-147">Operating System.</span></span>|
|<span data-ttu-id="b7537-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="b7537-148">osVersion</span></span>|<span data-ttu-id="b7537-149">String</span><span class="sxs-lookup"><span data-stu-id="b7537-149">String</span></span>|<span data-ttu-id="b7537-150">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="b7537-150">OS Version.</span></span>|
|<span data-ttu-id="b7537-151">userId</span><span class="sxs-lookup"><span data-stu-id="b7537-151">userId</span></span>|<span data-ttu-id="b7537-152">String</span><span class="sxs-lookup"><span data-stu-id="b7537-152">String</span></span>|<span data-ttu-id="b7537-153">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="b7537-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="b7537-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="b7537-154">deviceId</span></span>|<span data-ttu-id="b7537-155">String</span><span class="sxs-lookup"><span data-stu-id="b7537-155">String</span></span>|<span data-ttu-id="b7537-156">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b7537-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="b7537-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="b7537-157">enrollmentType</span></span>|[<span data-ttu-id="b7537-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b7537-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="b7537-159">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="b7537-159">Type of the enrollment.</span></span> <span data-ttu-id="b7537-160">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="b7537-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="b7537-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="b7537-161">failureCategory</span></span>|[<span data-ttu-id="b7537-162">Девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="b7537-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="b7537-163">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="b7537-163">Highlevel failure category.</span></span> <span data-ttu-id="b7537-164">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="b7537-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="b7537-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="b7537-165">failureReason</span></span>|<span data-ttu-id="b7537-166">String</span><span class="sxs-lookup"><span data-stu-id="b7537-166">String</span></span>|<span data-ttu-id="b7537-167">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="b7537-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="b7537-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7537-168">Response</span></span>
<span data-ttu-id="b7537-169">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b7537-169">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7537-170">Пример</span><span class="sxs-lookup"><span data-stu-id="b7537-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7537-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7537-171">Request</span></span>
<span data-ttu-id="b7537-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7537-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7537-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7537-173">Response</span></span>
<span data-ttu-id="b7537-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7537-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



