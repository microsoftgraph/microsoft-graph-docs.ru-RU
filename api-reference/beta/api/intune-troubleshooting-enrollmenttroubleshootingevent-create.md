---
title: Создание объекта enrollmentTroubleshootingEvent
description: Создание объекта enrollmentTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3d3cdd865bf2d2316d2e50e433375eb875c4406
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541439"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="8e941-103">Создание объекта enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8e941-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="8e941-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e941-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e941-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e941-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e941-106">Создание объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8e941-106">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e941-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8e941-107">Prerequisites</span></span>
<span data-ttu-id="8e941-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e941-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e941-110">Permission type</span></span>|<span data-ttu-id="8e941-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e941-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e941-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e941-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e941-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e941-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8e941-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e941-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e941-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e941-115">Not supported.</span></span>|
|<span data-ttu-id="8e941-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e941-116">Application</span></span>|<span data-ttu-id="8e941-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e941-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e941-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e941-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="8e941-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e941-119">Request headers</span></span>
|<span data-ttu-id="8e941-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e941-120">Header</span></span>|<span data-ttu-id="8e941-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8e941-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e941-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e941-122">Authorization</span></span>|<span data-ttu-id="8e941-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e941-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e941-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8e941-124">Accept</span></span>|<span data-ttu-id="8e941-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e941-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e941-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e941-126">Request body</span></span>
<span data-ttu-id="8e941-127">В теле запроса добавьте представление объекта enrollmentTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e941-127">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="8e941-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="8e941-128">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="8e941-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e941-129">Property</span></span>|<span data-ttu-id="8e941-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8e941-130">Type</span></span>|<span data-ttu-id="8e941-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8e941-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e941-132">id</span><span class="sxs-lookup"><span data-stu-id="8e941-132">id</span></span>|<span data-ttu-id="8e941-133">String</span><span class="sxs-lookup"><span data-stu-id="8e941-133">String</span></span>|<span data-ttu-id="8e941-134">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8e941-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e941-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="8e941-135">eventDateTime</span></span>|<span data-ttu-id="8e941-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e941-136">DateTimeOffset</span></span>|<span data-ttu-id="8e941-137">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="8e941-137">Time when the event occurred .</span></span> <span data-ttu-id="8e941-138">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8e941-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e941-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="8e941-139">correlationId</span></span>|<span data-ttu-id="8e941-140">String</span><span class="sxs-lookup"><span data-stu-id="8e941-140">String</span></span>|<span data-ttu-id="8e941-141">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="8e941-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="8e941-142">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8e941-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e941-143">Траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="8e941-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="8e941-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="8e941-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="8e941-145">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="8e941-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="8e941-146">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8e941-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e941-147">eventName</span><span class="sxs-lookup"><span data-stu-id="8e941-147">eventName</span></span>|<span data-ttu-id="8e941-148">String</span><span class="sxs-lookup"><span data-stu-id="8e941-148">String</span></span>|<span data-ttu-id="8e941-149">Имя события, соответствующее соБытию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="8e941-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="8e941-150">Это неОбязательное поле, унаследованное от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8e941-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e941-151">Аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="8e941-151">additionalInformation</span></span>|<span data-ttu-id="8e941-152">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8e941-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="8e941-153">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок, наСледуемом от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="8e941-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8e941-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e941-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="8e941-155">String</span><span class="sxs-lookup"><span data-stu-id="8e941-155">String</span></span>|<span data-ttu-id="8e941-156">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="8e941-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="8e941-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8e941-157">operatingSystem</span></span>|<span data-ttu-id="8e941-158">String</span><span class="sxs-lookup"><span data-stu-id="8e941-158">String</span></span>|<span data-ttu-id="8e941-159">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="8e941-159">Operating System.</span></span>|
|<span data-ttu-id="8e941-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="8e941-160">osVersion</span></span>|<span data-ttu-id="8e941-161">String</span><span class="sxs-lookup"><span data-stu-id="8e941-161">String</span></span>|<span data-ttu-id="8e941-162">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="8e941-162">OS Version.</span></span>|
|<span data-ttu-id="8e941-163">userId</span><span class="sxs-lookup"><span data-stu-id="8e941-163">userId</span></span>|<span data-ttu-id="8e941-164">String</span><span class="sxs-lookup"><span data-stu-id="8e941-164">String</span></span>|<span data-ttu-id="8e941-165">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="8e941-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="8e941-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="8e941-166">deviceId</span></span>|<span data-ttu-id="8e941-167">String</span><span class="sxs-lookup"><span data-stu-id="8e941-167">String</span></span>|<span data-ttu-id="8e941-168">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8e941-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="8e941-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="8e941-169">enrollmentType</span></span>|[<span data-ttu-id="8e941-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="8e941-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="8e941-171">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="8e941-171">Type of the enrollment.</span></span> <span data-ttu-id="8e941-172">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="8e941-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="8e941-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="8e941-173">failureCategory</span></span>|[<span data-ttu-id="8e941-174">Девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="8e941-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="8e941-175">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="8e941-175">Highlevel failure category.</span></span> <span data-ttu-id="8e941-176">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="8e941-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="8e941-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="8e941-177">failureReason</span></span>|<span data-ttu-id="8e941-178">String</span><span class="sxs-lookup"><span data-stu-id="8e941-178">String</span></span>|<span data-ttu-id="8e941-179">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="8e941-179">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="8e941-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e941-180">Response</span></span>
<span data-ttu-id="8e941-181">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8e941-181">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e941-182">Пример</span><span class="sxs-lookup"><span data-stu-id="8e941-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e941-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e941-183">Request</span></span>
<span data-ttu-id="8e941-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e941-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="8e941-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e941-185">Response</span></span>
<span data-ttu-id="8e941-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e941-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



