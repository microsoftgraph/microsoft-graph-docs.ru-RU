---
title: Обновление enrollmentTroubleshootingEvent
description: Обновление свойств объекта enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58273ba4e42bd3ed27e35fd3eee16321202eb416
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223341"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="7fc27-103">Обновление enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="7fc27-103">Update enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="7fc27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fc27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7fc27-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fc27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fc27-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7fc27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fc27-107">Обновление свойств объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="7fc27-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fc27-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7fc27-108">Prerequisites</span></span>
<span data-ttu-id="7fc27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fc27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fc27-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fc27-111">Permission type</span></span>|<span data-ttu-id="7fc27-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fc27-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fc27-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fc27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7fc27-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fc27-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7fc27-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fc27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fc27-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fc27-116">Not supported.</span></span>|
|<span data-ttu-id="7fc27-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7fc27-117">Application</span></span>|<span data-ttu-id="7fc27-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fc27-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fc27-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fc27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="7fc27-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7fc27-120">Request headers</span></span>
|<span data-ttu-id="7fc27-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fc27-121">Header</span></span>|<span data-ttu-id="7fc27-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7fc27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fc27-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fc27-123">Authorization</span></span>|<span data-ttu-id="7fc27-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fc27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fc27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7fc27-125">Accept</span></span>|<span data-ttu-id="7fc27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7fc27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fc27-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fc27-127">Request body</span></span>
<span data-ttu-id="7fc27-128">В теле запроса добавьте представление объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fc27-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="7fc27-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="7fc27-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="7fc27-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fc27-130">Property</span></span>|<span data-ttu-id="7fc27-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7fc27-131">Type</span></span>|<span data-ttu-id="7fc27-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7fc27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fc27-133">id</span><span class="sxs-lookup"><span data-stu-id="7fc27-133">id</span></span>|<span data-ttu-id="7fc27-134">String</span><span class="sxs-lookup"><span data-stu-id="7fc27-134">String</span></span>|<span data-ttu-id="7fc27-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="7fc27-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7fc27-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="7fc27-136">eventDateTime</span></span>|<span data-ttu-id="7fc27-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fc27-137">DateTimeOffset</span></span>|<span data-ttu-id="7fc27-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="7fc27-138">Time when the event occurred .</span></span> <span data-ttu-id="7fc27-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="7fc27-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7fc27-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="7fc27-140">correlationId</span></span>|<span data-ttu-id="7fc27-141">String</span><span class="sxs-lookup"><span data-stu-id="7fc27-141">String</span></span>|<span data-ttu-id="7fc27-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="7fc27-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="7fc27-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="7fc27-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7fc27-144">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="7fc27-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="7fc27-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="7fc27-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="7fc27-146">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="7fc27-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="7fc27-147">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="7fc27-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7fc27-148">eventName</span><span class="sxs-lookup"><span data-stu-id="7fc27-148">eventName</span></span>|<span data-ttu-id="7fc27-149">String</span><span class="sxs-lookup"><span data-stu-id="7fc27-149">String</span></span>|<span data-ttu-id="7fc27-150">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="7fc27-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="7fc27-151">Это необязательное поле, унаследованное от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="7fc27-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7fc27-152">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="7fc27-152">additionalInformation</span></span>|<span data-ttu-id="7fc27-153">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7fc27-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7fc27-154">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок, наследуемом от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="7fc27-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="7fc27-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7fc27-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="7fc27-156">String</span><span class="sxs-lookup"><span data-stu-id="7fc27-156">String</span></span>|<span data-ttu-id="7fc27-157">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="7fc27-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="7fc27-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="7fc27-158">operatingSystem</span></span>|<span data-ttu-id="7fc27-159">String</span><span class="sxs-lookup"><span data-stu-id="7fc27-159">String</span></span>|<span data-ttu-id="7fc27-160">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="7fc27-160">Operating System.</span></span>|
|<span data-ttu-id="7fc27-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="7fc27-161">osVersion</span></span>|<span data-ttu-id="7fc27-162">String</span><span class="sxs-lookup"><span data-stu-id="7fc27-162">String</span></span>|<span data-ttu-id="7fc27-163">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="7fc27-163">OS Version.</span></span>|
|<span data-ttu-id="7fc27-164">userId</span><span class="sxs-lookup"><span data-stu-id="7fc27-164">userId</span></span>|<span data-ttu-id="7fc27-165">String</span><span class="sxs-lookup"><span data-stu-id="7fc27-165">String</span></span>|<span data-ttu-id="7fc27-166">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="7fc27-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="7fc27-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="7fc27-167">deviceId</span></span>|<span data-ttu-id="7fc27-168">String</span><span class="sxs-lookup"><span data-stu-id="7fc27-168">String</span></span>|<span data-ttu-id="7fc27-169">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7fc27-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="7fc27-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="7fc27-170">enrollmentType</span></span>|[<span data-ttu-id="7fc27-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="7fc27-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="7fc27-172">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="7fc27-172">Type of the enrollment.</span></span> <span data-ttu-id="7fc27-173">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="7fc27-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="7fc27-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="7fc27-174">failureCategory</span></span>|[<span data-ttu-id="7fc27-175">девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="7fc27-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="7fc27-176">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="7fc27-176">Highlevel failure category.</span></span> <span data-ttu-id="7fc27-177">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="7fc27-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="7fc27-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="7fc27-178">failureReason</span></span>|<span data-ttu-id="7fc27-179">String</span><span class="sxs-lookup"><span data-stu-id="7fc27-179">String</span></span>|<span data-ttu-id="7fc27-180">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="7fc27-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="7fc27-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc27-181">Response</span></span>
<span data-ttu-id="7fc27-182">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7fc27-182">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fc27-183">Пример</span><span class="sxs-lookup"><span data-stu-id="7fc27-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fc27-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fc27-184">Request</span></span>
<span data-ttu-id="7fc27-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fc27-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7fc27-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc27-186">Response</span></span>
<span data-ttu-id="7fc27-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7fc27-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




