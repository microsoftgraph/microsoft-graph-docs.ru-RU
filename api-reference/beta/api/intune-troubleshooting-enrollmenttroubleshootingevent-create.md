---
title: Создание объекта enrollmentTroubleshootingEvent
description: Создание объекта enrollmentTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db572801f4e46e23dbac125f03ef1e03af06c785
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735325"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="a14dc-103">Создание объекта enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a14dc-103">Create enrollmentTroubleshootingEvent</span></span>

<span data-ttu-id="a14dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a14dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a14dc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a14dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a14dc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a14dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a14dc-107">Создание объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a14dc-107">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a14dc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a14dc-108">Prerequisites</span></span>
<span data-ttu-id="a14dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a14dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a14dc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a14dc-111">Permission type</span></span>|<span data-ttu-id="a14dc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a14dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a14dc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a14dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a14dc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a14dc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a14dc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a14dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a14dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a14dc-116">Not supported.</span></span>|
|<span data-ttu-id="a14dc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a14dc-117">Application</span></span>|<span data-ttu-id="a14dc-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a14dc-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a14dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a14dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="a14dc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a14dc-120">Request headers</span></span>
|<span data-ttu-id="a14dc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a14dc-121">Header</span></span>|<span data-ttu-id="a14dc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a14dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a14dc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a14dc-123">Authorization</span></span>|<span data-ttu-id="a14dc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a14dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a14dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a14dc-125">Accept</span></span>|<span data-ttu-id="a14dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a14dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a14dc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a14dc-127">Request body</span></span>
<span data-ttu-id="a14dc-128">В теле запроса добавьте представление объекта enrollmentTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a14dc-128">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="a14dc-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="a14dc-129">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="a14dc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a14dc-130">Property</span></span>|<span data-ttu-id="a14dc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a14dc-131">Type</span></span>|<span data-ttu-id="a14dc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a14dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a14dc-133">id</span><span class="sxs-lookup"><span data-stu-id="a14dc-133">id</span></span>|<span data-ttu-id="a14dc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a14dc-134">String</span></span>|<span data-ttu-id="a14dc-135">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a14dc-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a14dc-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a14dc-136">eventDateTime</span></span>|<span data-ttu-id="a14dc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a14dc-137">DateTimeOffset</span></span>|<span data-ttu-id="a14dc-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="a14dc-138">Time when the event occurred .</span></span> <span data-ttu-id="a14dc-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a14dc-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a14dc-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="a14dc-140">correlationId</span></span>|<span data-ttu-id="a14dc-141">String</span><span class="sxs-lookup"><span data-stu-id="a14dc-141">String</span></span>|<span data-ttu-id="a14dc-142">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="a14dc-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="a14dc-143">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a14dc-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a14dc-144">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="a14dc-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="a14dc-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a14dc-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="a14dc-146">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="a14dc-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="a14dc-147">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="a14dc-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a14dc-148">eventName</span><span class="sxs-lookup"><span data-stu-id="a14dc-148">eventName</span></span>|<span data-ttu-id="a14dc-149">Строка</span><span class="sxs-lookup"><span data-stu-id="a14dc-149">String</span></span>|<span data-ttu-id="a14dc-150">Имя события, соответствующее событию устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="a14dc-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="a14dc-151">Это необязательное поле, унаследованное от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="a14dc-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a14dc-152">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="a14dc-152">additionalInformation</span></span>|<span data-ttu-id="a14dc-153">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a14dc-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a14dc-154">Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок, наследуемом от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="a14dc-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a14dc-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a14dc-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="a14dc-156">String</span><span class="sxs-lookup"><span data-stu-id="a14dc-156">String</span></span>|<span data-ttu-id="a14dc-157">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="a14dc-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="a14dc-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="a14dc-158">operatingSystem</span></span>|<span data-ttu-id="a14dc-159">String</span><span class="sxs-lookup"><span data-stu-id="a14dc-159">String</span></span>|<span data-ttu-id="a14dc-160">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="a14dc-160">Operating System.</span></span>|
|<span data-ttu-id="a14dc-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="a14dc-161">osVersion</span></span>|<span data-ttu-id="a14dc-162">String</span><span class="sxs-lookup"><span data-stu-id="a14dc-162">String</span></span>|<span data-ttu-id="a14dc-163">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="a14dc-163">OS Version.</span></span>|
|<span data-ttu-id="a14dc-164">userId</span><span class="sxs-lookup"><span data-stu-id="a14dc-164">userId</span></span>|<span data-ttu-id="a14dc-165">String</span><span class="sxs-lookup"><span data-stu-id="a14dc-165">String</span></span>|<span data-ttu-id="a14dc-166">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="a14dc-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="a14dc-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="a14dc-167">deviceId</span></span>|<span data-ttu-id="a14dc-168">String</span><span class="sxs-lookup"><span data-stu-id="a14dc-168">String</span></span>|<span data-ttu-id="a14dc-169">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a14dc-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="a14dc-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="a14dc-170">enrollmentType</span></span>|[<span data-ttu-id="a14dc-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a14dc-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="a14dc-172">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="a14dc-172">Type of the enrollment.</span></span> <span data-ttu-id="a14dc-173">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="a14dc-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, `androidEnterpriseDedicatedDevice`, `androidEnterpriseFullyManaged`, `androidEnterpriseCorporateWorkProfile`.</span></span>|
|<span data-ttu-id="a14dc-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="a14dc-174">failureCategory</span></span>|[<span data-ttu-id="a14dc-175">девицеенроллментфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="a14dc-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="a14dc-176">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="a14dc-176">Highlevel failure category.</span></span> <span data-ttu-id="a14dc-177">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="a14dc-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="a14dc-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="a14dc-178">failureReason</span></span>|<span data-ttu-id="a14dc-179">String</span><span class="sxs-lookup"><span data-stu-id="a14dc-179">String</span></span>|<span data-ttu-id="a14dc-180">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="a14dc-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="a14dc-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="a14dc-181">Response</span></span>
<span data-ttu-id="a14dc-182">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a14dc-182">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a14dc-183">Пример</span><span class="sxs-lookup"><span data-stu-id="a14dc-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="a14dc-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="a14dc-184">Request</span></span>
<span data-ttu-id="a14dc-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a14dc-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a14dc-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="a14dc-186">Response</span></span>
<span data-ttu-id="a14dc-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a14dc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





