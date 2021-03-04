---
title: Обновление enrollmentTroubleshootingEvent
description: Обновление свойств объекта enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27316867ddf692d5cec2a29e600e076d05c46890
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443792"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="78670-103">Обновление enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="78670-103">Update enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="78670-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78670-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78670-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78670-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78670-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78670-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78670-107">Обновление свойств объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="78670-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78670-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="78670-108">Prerequisites</span></span>
<span data-ttu-id="78670-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78670-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78670-111">Permission type</span></span>|<span data-ttu-id="78670-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="78670-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78670-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78670-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78670-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78670-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="78670-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78670-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78670-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78670-116">Not supported.</span></span>|
|<span data-ttu-id="78670-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="78670-117">Application</span></span>|<span data-ttu-id="78670-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78670-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78670-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78670-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="78670-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="78670-120">Request headers</span></span>
|<span data-ttu-id="78670-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78670-121">Header</span></span>|<span data-ttu-id="78670-122">Значение</span><span class="sxs-lookup"><span data-stu-id="78670-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78670-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78670-123">Authorization</span></span>|<span data-ttu-id="78670-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78670-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78670-125">Accept</span><span class="sxs-lookup"><span data-stu-id="78670-125">Accept</span></span>|<span data-ttu-id="78670-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78670-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78670-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="78670-127">Request body</span></span>
<span data-ttu-id="78670-128">В теле запроса добавьте представление объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78670-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="78670-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="78670-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="78670-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="78670-130">Property</span></span>|<span data-ttu-id="78670-131">Тип</span><span class="sxs-lookup"><span data-stu-id="78670-131">Type</span></span>|<span data-ttu-id="78670-132">Описание</span><span class="sxs-lookup"><span data-stu-id="78670-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78670-133">id</span><span class="sxs-lookup"><span data-stu-id="78670-133">id</span></span>|<span data-ttu-id="78670-134">String</span><span class="sxs-lookup"><span data-stu-id="78670-134">String</span></span>|<span data-ttu-id="78670-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="78670-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="78670-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="78670-136">eventDateTime</span></span>|<span data-ttu-id="78670-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78670-137">DateTimeOffset</span></span>|<span data-ttu-id="78670-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="78670-138">Time when the event occurred .</span></span> <span data-ttu-id="78670-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="78670-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="78670-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="78670-140">correlationId</span></span>|<span data-ttu-id="78670-141">String</span><span class="sxs-lookup"><span data-stu-id="78670-141">String</span></span>|<span data-ttu-id="78670-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="78670-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="78670-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="78670-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="78670-144">устранение неполадокErrorDetails</span><span class="sxs-lookup"><span data-stu-id="78670-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="78670-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="78670-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="78670-146">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="78670-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="78670-147">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="78670-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="78670-148">eventName</span><span class="sxs-lookup"><span data-stu-id="78670-148">eventName</span></span>|<span data-ttu-id="78670-149">String</span><span class="sxs-lookup"><span data-stu-id="78670-149">String</span></span>|<span data-ttu-id="78670-150">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="78670-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="78670-151">Это необязательный поле, унаследованный от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="78670-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="78670-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="78670-152">additionalInformation</span></span>|<span data-ttu-id="78670-153">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="78670-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="78670-154">Набор пар строк и пар значений строк, которые предоставляют дополнительные сведения о событии устранения неполадок, унаследованных от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="78670-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="78670-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="78670-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="78670-156">String</span><span class="sxs-lookup"><span data-stu-id="78670-156">String</span></span>|<span data-ttu-id="78670-157">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="78670-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="78670-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="78670-158">operatingSystem</span></span>|<span data-ttu-id="78670-159">String</span><span class="sxs-lookup"><span data-stu-id="78670-159">String</span></span>|<span data-ttu-id="78670-160">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="78670-160">Operating System.</span></span>|
|<span data-ttu-id="78670-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="78670-161">osVersion</span></span>|<span data-ttu-id="78670-162">String</span><span class="sxs-lookup"><span data-stu-id="78670-162">String</span></span>|<span data-ttu-id="78670-163">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="78670-163">OS Version.</span></span>|
|<span data-ttu-id="78670-164">userId</span><span class="sxs-lookup"><span data-stu-id="78670-164">userId</span></span>|<span data-ttu-id="78670-165">String</span><span class="sxs-lookup"><span data-stu-id="78670-165">String</span></span>|<span data-ttu-id="78670-166">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="78670-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="78670-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="78670-167">deviceId</span></span>|<span data-ttu-id="78670-168">String</span><span class="sxs-lookup"><span data-stu-id="78670-168">String</span></span>|<span data-ttu-id="78670-169">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="78670-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="78670-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="78670-170">enrollmentType</span></span>|[<span data-ttu-id="78670-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="78670-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="78670-172">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="78670-172">Type of the enrollment.</span></span> <span data-ttu-id="78670-173">Возможные значения: `unknown` `userEnrollment` , , , , , `deviceEnrollmentManager` , , `appleBulkWithUser` , `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` .</span><span class="sxs-lookup"><span data-stu-id="78670-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="78670-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="78670-174">failureCategory</span></span>|[<span data-ttu-id="78670-175">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="78670-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="78670-176">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="78670-176">Highlevel failure category.</span></span> <span data-ttu-id="78670-177">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="78670-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="78670-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="78670-178">failureReason</span></span>|<span data-ttu-id="78670-179">String</span><span class="sxs-lookup"><span data-stu-id="78670-179">String</span></span>|<span data-ttu-id="78670-180">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="78670-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="78670-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="78670-181">Response</span></span>
<span data-ttu-id="78670-182">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="78670-182">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78670-183">Пример</span><span class="sxs-lookup"><span data-stu-id="78670-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="78670-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="78670-184">Request</span></span>
<span data-ttu-id="78670-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78670-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="78670-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="78670-186">Response</span></span>
<span data-ttu-id="78670-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78670-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




