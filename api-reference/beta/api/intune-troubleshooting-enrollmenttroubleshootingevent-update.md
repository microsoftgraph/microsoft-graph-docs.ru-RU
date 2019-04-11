---
title: Обновление enrollmentTroubleshootingEvent
description: Обновление свойств объекта enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eafa5ec230bd439e02f86bc19f13350aa35d2a8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776418"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="475d4-103">Обновление enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="475d4-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="475d4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="475d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="475d4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="475d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="475d4-106">Обновление свойств объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="475d4-106">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="475d4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="475d4-107">Prerequisites</span></span>
<span data-ttu-id="475d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="475d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="475d4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="475d4-110">Permission type</span></span>|<span data-ttu-id="475d4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="475d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="475d4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="475d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="475d4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="475d4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="475d4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="475d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="475d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="475d4-115">Not supported.</span></span>|
|<span data-ttu-id="475d4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="475d4-116">Application</span></span>|<span data-ttu-id="475d4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="475d4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="475d4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="475d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="475d4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="475d4-119">Request headers</span></span>
|<span data-ttu-id="475d4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="475d4-120">Header</span></span>|<span data-ttu-id="475d4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="475d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="475d4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="475d4-122">Authorization</span></span>|<span data-ttu-id="475d4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="475d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="475d4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="475d4-124">Accept</span></span>|<span data-ttu-id="475d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="475d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="475d4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="475d4-126">Request body</span></span>
<span data-ttu-id="475d4-127">В теле запроса добавьте представление объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="475d4-127">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="475d4-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="475d4-128">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="475d4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="475d4-129">Property</span></span>|<span data-ttu-id="475d4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="475d4-130">Type</span></span>|<span data-ttu-id="475d4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="475d4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="475d4-132">id</span><span class="sxs-lookup"><span data-stu-id="475d4-132">id</span></span>|<span data-ttu-id="475d4-133">String</span><span class="sxs-lookup"><span data-stu-id="475d4-133">String</span></span>|<span data-ttu-id="475d4-134">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="475d4-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="475d4-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="475d4-135">eventDateTime</span></span>|<span data-ttu-id="475d4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="475d4-136">DateTimeOffset</span></span>|<span data-ttu-id="475d4-137">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="475d4-137">Time when the event occurred .</span></span> <span data-ttu-id="475d4-138">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="475d4-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="475d4-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="475d4-139">correlationId</span></span>|<span data-ttu-id="475d4-140">String</span><span class="sxs-lookup"><span data-stu-id="475d4-140">String</span></span>|<span data-ttu-id="475d4-141">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="475d4-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="475d4-142">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="475d4-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="475d4-143">Траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="475d4-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="475d4-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="475d4-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="475d4-145">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="475d4-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="475d4-146">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="475d4-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="475d4-147">eventName</span><span class="sxs-lookup"><span data-stu-id="475d4-147">eventName</span></span>|<span data-ttu-id="475d4-148">String</span><span class="sxs-lookup"><span data-stu-id="475d4-148">String</span></span>|<span data-ttu-id="475d4-149">Имя события, соответствующее соБытию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="475d4-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="475d4-150">Это неОбязательное поле, унаследованное от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="475d4-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="475d4-151">Аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="475d4-151">additionalInformation</span></span>|<span data-ttu-id="475d4-152">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="475d4-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="475d4-153">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок, наСледуемом от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="475d4-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="475d4-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="475d4-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="475d4-155">String</span><span class="sxs-lookup"><span data-stu-id="475d4-155">String</span></span>|<span data-ttu-id="475d4-156">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="475d4-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="475d4-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="475d4-157">operatingSystem</span></span>|<span data-ttu-id="475d4-158">String</span><span class="sxs-lookup"><span data-stu-id="475d4-158">String</span></span>|<span data-ttu-id="475d4-159">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="475d4-159">Operating System.</span></span>|
|<span data-ttu-id="475d4-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="475d4-160">osVersion</span></span>|<span data-ttu-id="475d4-161">String</span><span class="sxs-lookup"><span data-stu-id="475d4-161">String</span></span>|<span data-ttu-id="475d4-162">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="475d4-162">OS Version.</span></span>|
|<span data-ttu-id="475d4-163">userId</span><span class="sxs-lookup"><span data-stu-id="475d4-163">userId</span></span>|<span data-ttu-id="475d4-164">String</span><span class="sxs-lookup"><span data-stu-id="475d4-164">String</span></span>|<span data-ttu-id="475d4-165">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="475d4-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="475d4-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="475d4-166">deviceId</span></span>|<span data-ttu-id="475d4-167">String</span><span class="sxs-lookup"><span data-stu-id="475d4-167">String</span></span>|<span data-ttu-id="475d4-168">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="475d4-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="475d4-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="475d4-169">enrollmentType</span></span>|[<span data-ttu-id="475d4-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="475d4-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="475d4-171">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="475d4-171">Type of the enrollment.</span></span> <span data-ttu-id="475d4-172">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="475d4-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="475d4-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="475d4-173">failureCategory</span></span>|[<span data-ttu-id="475d4-174">Девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="475d4-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="475d4-175">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="475d4-175">Highlevel failure category.</span></span> <span data-ttu-id="475d4-176">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="475d4-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="475d4-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="475d4-177">failureReason</span></span>|<span data-ttu-id="475d4-178">String</span><span class="sxs-lookup"><span data-stu-id="475d4-178">String</span></span>|<span data-ttu-id="475d4-179">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="475d4-179">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="475d4-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="475d4-180">Response</span></span>
<span data-ttu-id="475d4-181">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="475d4-181">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="475d4-182">Пример</span><span class="sxs-lookup"><span data-stu-id="475d4-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="475d4-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="475d4-183">Request</span></span>
<span data-ttu-id="475d4-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="475d4-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="475d4-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="475d4-185">Response</span></span>
<span data-ttu-id="475d4-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="475d4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



