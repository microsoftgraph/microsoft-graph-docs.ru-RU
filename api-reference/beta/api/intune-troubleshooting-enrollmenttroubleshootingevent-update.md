---
title: Обновление enrollmentTroubleshootingEvent
description: Обновление свойств объекта enrollmentTroubleshootingEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: efbc823b4ba7a5e28a0a2e7d82b7708102002a71
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399789"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="e6ce3-103">Обновление enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e6ce3-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="e6ce3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e6ce3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6ce3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6ce3-107">Обновление свойств объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e6ce3-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6ce3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e6ce3-108">Prerequisites</span></span>
<span data-ttu-id="e6ce3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6ce3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e6ce3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6ce3-111">Permission type</span></span>|<span data-ttu-id="e6ce3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6ce3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6ce3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6ce3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6ce3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ce3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e6ce3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6ce3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6ce3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-116">Not supported.</span></span>|
|<span data-ttu-id="e6ce3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6ce3-117">Application</span></span>|<span data-ttu-id="e6ce3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6ce3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6ce3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="e6ce3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6ce3-120">Request headers</span></span>
|<span data-ttu-id="e6ce3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6ce3-121">Header</span></span>|<span data-ttu-id="e6ce3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e6ce3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6ce3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6ce3-123">Authorization</span></span>|<span data-ttu-id="e6ce3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e6ce3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6ce3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e6ce3-125">Accept</span></span>|<span data-ttu-id="e6ce3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6ce3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6ce3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6ce3-127">Request body</span></span>
<span data-ttu-id="e6ce3-128">В теле запроса добавьте представление объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="e6ce3-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e6ce3-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="e6ce3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6ce3-130">Property</span></span>|<span data-ttu-id="e6ce3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e6ce3-131">Type</span></span>|<span data-ttu-id="e6ce3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e6ce3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6ce3-133">id</span><span class="sxs-lookup"><span data-stu-id="e6ce3-133">id</span></span>|<span data-ttu-id="e6ce3-134">String</span><span class="sxs-lookup"><span data-stu-id="e6ce3-134">String</span></span>|<span data-ttu-id="e6ce3-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e6ce3-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e6ce3-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="e6ce3-136">eventDateTime</span></span>|<span data-ttu-id="e6ce3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6ce3-137">DateTimeOffset</span></span>|<span data-ttu-id="e6ce3-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-138">Time when the event occurred .</span></span> <span data-ttu-id="e6ce3-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e6ce3-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e6ce3-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="e6ce3-140">correlationId</span></span>|<span data-ttu-id="e6ce3-141">String</span><span class="sxs-lookup"><span data-stu-id="e6ce3-141">String</span></span>|<span data-ttu-id="e6ce3-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="e6ce3-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e6ce3-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e6ce3-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e6ce3-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="e6ce3-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e6ce3-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="e6ce3-146">Объект, содержащий подробные сведения об ошибке и ее обновлений.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="e6ce3-147">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="e6ce3-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e6ce3-148">элемент eventName</span><span class="sxs-lookup"><span data-stu-id="e6ce3-148">eventName</span></span>|<span data-ttu-id="e6ce3-149">String</span><span class="sxs-lookup"><span data-stu-id="e6ce3-149">String</span></span>|<span data-ttu-id="e6ce3-150">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="e6ce3-151">Это необязательное поле унаследованные от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e6ce3-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e6ce3-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="e6ce3-152">additionalInformation</span></span>|<span data-ttu-id="e6ce3-153">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e6ce3-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e6ce3-154">Набор ключ строки и пар строковое значение которой содержатся дополнительные сведения на устранение неполадок события унаследованные от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="e6ce3-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="e6ce3-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e6ce3-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="e6ce3-156">String</span><span class="sxs-lookup"><span data-stu-id="e6ce3-156">String</span></span>|<span data-ttu-id="e6ce3-157">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="e6ce3-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="e6ce3-158">operatingSystem</span></span>|<span data-ttu-id="e6ce3-159">String</span><span class="sxs-lookup"><span data-stu-id="e6ce3-159">String</span></span>|<span data-ttu-id="e6ce3-160">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-160">Operating System.</span></span>|
|<span data-ttu-id="e6ce3-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="e6ce3-161">osVersion</span></span>|<span data-ttu-id="e6ce3-162">String</span><span class="sxs-lookup"><span data-stu-id="e6ce3-162">String</span></span>|<span data-ttu-id="e6ce3-163">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-163">OS Version.</span></span>|
|<span data-ttu-id="e6ce3-164">userId</span><span class="sxs-lookup"><span data-stu-id="e6ce3-164">userId</span></span>|<span data-ttu-id="e6ce3-165">String</span><span class="sxs-lookup"><span data-stu-id="e6ce3-165">String</span></span>|<span data-ttu-id="e6ce3-166">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="e6ce3-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="e6ce3-167">deviceId</span></span>|<span data-ttu-id="e6ce3-168">String</span><span class="sxs-lookup"><span data-stu-id="e6ce3-168">String</span></span>|<span data-ttu-id="e6ce3-169">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="e6ce3-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="e6ce3-170">enrollmentType</span></span>|[<span data-ttu-id="e6ce3-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="e6ce3-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="e6ce3-172">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-172">Type of the enrollment.</span></span> <span data-ttu-id="e6ce3-173">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="e6ce3-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="e6ce3-174">failureCategory</span></span>|[<span data-ttu-id="e6ce3-175">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="e6ce3-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="e6ce3-176">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-176">Highlevel failure category.</span></span> <span data-ttu-id="e6ce3-177">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="e6ce3-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="e6ce3-178">failureReason</span></span>|<span data-ttu-id="e6ce3-179">String</span><span class="sxs-lookup"><span data-stu-id="e6ce3-179">String</span></span>|<span data-ttu-id="e6ce3-180">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="e6ce3-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6ce3-181">Response</span></span>
<span data-ttu-id="e6ce3-182">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-182">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6ce3-183">Пример</span><span class="sxs-lookup"><span data-stu-id="e6ce3-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6ce3-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6ce3-184">Request</span></span>
<span data-ttu-id="e6ce3-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 1182

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="e6ce3-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6ce3-186">Response</span></span>
<span data-ttu-id="e6ce3-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1231

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
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




