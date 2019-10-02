---
title: Создание объекта enrollmentTroubleshootingEvent
description: Создание объекта enrollmentTroubleshootingEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64894d39d38359331815818c6342d46dae35d09a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361030"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="68757-103">Создание объекта enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="68757-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="68757-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68757-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68757-105">Создание объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="68757-105">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68757-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="68757-106">Prerequisites</span></span>
<span data-ttu-id="68757-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68757-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68757-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68757-109">Permission type</span></span>|<span data-ttu-id="68757-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68757-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68757-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68757-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68757-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68757-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="68757-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68757-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68757-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68757-114">Not supported.</span></span>|
|<span data-ttu-id="68757-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68757-115">Application</span></span>|<span data-ttu-id="68757-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68757-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68757-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68757-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="68757-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68757-118">Request headers</span></span>
|<span data-ttu-id="68757-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68757-119">Header</span></span>|<span data-ttu-id="68757-120">Значение</span><span class="sxs-lookup"><span data-stu-id="68757-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68757-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68757-121">Authorization</span></span>|<span data-ttu-id="68757-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68757-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68757-123">Accept</span><span class="sxs-lookup"><span data-stu-id="68757-123">Accept</span></span>|<span data-ttu-id="68757-124">application/json</span><span class="sxs-lookup"><span data-stu-id="68757-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68757-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68757-125">Request body</span></span>
<span data-ttu-id="68757-126">В теле запроса добавьте представление объекта enrollmentTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68757-126">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="68757-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="68757-127">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="68757-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="68757-128">Property</span></span>|<span data-ttu-id="68757-129">Тип</span><span class="sxs-lookup"><span data-stu-id="68757-129">Type</span></span>|<span data-ttu-id="68757-130">Описание</span><span class="sxs-lookup"><span data-stu-id="68757-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68757-131">id</span><span class="sxs-lookup"><span data-stu-id="68757-131">id</span></span>|<span data-ttu-id="68757-132">Строка</span><span class="sxs-lookup"><span data-stu-id="68757-132">String</span></span>|<span data-ttu-id="68757-133">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="68757-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="68757-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="68757-134">eventDateTime</span></span>|<span data-ttu-id="68757-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68757-135">DateTimeOffset</span></span>|<span data-ttu-id="68757-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="68757-136">Time when the event occurred .</span></span> <span data-ttu-id="68757-137">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="68757-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="68757-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="68757-138">correlationId</span></span>|<span data-ttu-id="68757-139">String</span><span class="sxs-lookup"><span data-stu-id="68757-139">String</span></span>|<span data-ttu-id="68757-140">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="68757-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="68757-141">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="68757-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="68757-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="68757-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="68757-143">String</span><span class="sxs-lookup"><span data-stu-id="68757-143">String</span></span>|<span data-ttu-id="68757-144">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="68757-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="68757-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="68757-145">operatingSystem</span></span>|<span data-ttu-id="68757-146">String</span><span class="sxs-lookup"><span data-stu-id="68757-146">String</span></span>|<span data-ttu-id="68757-147">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="68757-147">Operating System.</span></span>|
|<span data-ttu-id="68757-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="68757-148">osVersion</span></span>|<span data-ttu-id="68757-149">String</span><span class="sxs-lookup"><span data-stu-id="68757-149">String</span></span>|<span data-ttu-id="68757-150">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="68757-150">OS Version.</span></span>|
|<span data-ttu-id="68757-151">userId</span><span class="sxs-lookup"><span data-stu-id="68757-151">userId</span></span>|<span data-ttu-id="68757-152">String</span><span class="sxs-lookup"><span data-stu-id="68757-152">String</span></span>|<span data-ttu-id="68757-153">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="68757-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="68757-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="68757-154">deviceId</span></span>|<span data-ttu-id="68757-155">String</span><span class="sxs-lookup"><span data-stu-id="68757-155">String</span></span>|<span data-ttu-id="68757-156">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="68757-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="68757-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="68757-157">enrollmentType</span></span>|[<span data-ttu-id="68757-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="68757-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="68757-159">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="68757-159">Type of the enrollment.</span></span> <span data-ttu-id="68757-160">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="68757-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="68757-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="68757-161">failureCategory</span></span>|[<span data-ttu-id="68757-162">девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="68757-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="68757-163">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="68757-163">Highlevel failure category.</span></span> <span data-ttu-id="68757-164">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="68757-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="68757-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="68757-165">failureReason</span></span>|<span data-ttu-id="68757-166">String</span><span class="sxs-lookup"><span data-stu-id="68757-166">String</span></span>|<span data-ttu-id="68757-167">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="68757-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="68757-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="68757-168">Response</span></span>
<span data-ttu-id="68757-169">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="68757-169">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68757-170">Пример</span><span class="sxs-lookup"><span data-stu-id="68757-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="68757-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="68757-171">Request</span></span>
<span data-ttu-id="68757-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68757-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68757-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="68757-173">Response</span></span>
<span data-ttu-id="68757-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68757-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




