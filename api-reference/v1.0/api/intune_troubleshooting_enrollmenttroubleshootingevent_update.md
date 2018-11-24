# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="5dac7-101">Обновление enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="5dac7-101">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="5dac7-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5dac7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5dac7-103">Обновление свойств объекта [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="5dac7-103">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5dac7-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5dac7-104">Prerequisites</span></span>
<span data-ttu-id="5dac7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5dac7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5dac7-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5dac7-107">Permission type</span></span>|<span data-ttu-id="5dac7-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5dac7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dac7-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5dac7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5dac7-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dac7-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5dac7-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5dac7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dac7-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5dac7-112">Not supported.</span></span>|
|<span data-ttu-id="5dac7-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5dac7-113">Application</span></span>|<span data-ttu-id="5dac7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5dac7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dac7-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5dac7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="5dac7-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5dac7-116">Request headers</span></span>
|<span data-ttu-id="5dac7-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5dac7-117">Header</span></span>|<span data-ttu-id="5dac7-118">Значение</span><span class="sxs-lookup"><span data-stu-id="5dac7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dac7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dac7-119">Authorization</span></span>|<span data-ttu-id="5dac7-120">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5dac7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dac7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5dac7-121">Accept</span></span>|<span data-ttu-id="5dac7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5dac7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dac7-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5dac7-123">Request body</span></span>
<span data-ttu-id="5dac7-124">В теле запроса добавьте представление объекта [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dac7-124">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="5dac7-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="5dac7-125">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="5dac7-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="5dac7-126">Property</span></span>|<span data-ttu-id="5dac7-127">Тип</span><span class="sxs-lookup"><span data-stu-id="5dac7-127">Type</span></span>|<span data-ttu-id="5dac7-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5dac7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dac7-129">id</span><span class="sxs-lookup"><span data-stu-id="5dac7-129">id</span></span>|<span data-ttu-id="5dac7-130">String</span><span class="sxs-lookup"><span data-stu-id="5dac7-130">String</span></span>|<span data-ttu-id="5dac7-131">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="5dac7-131">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="5dac7-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="5dac7-132">eventDateTime</span></span>|<span data-ttu-id="5dac7-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dac7-133">DateTimeOffset</span></span>|<span data-ttu-id="5dac7-134">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="5dac7-134">Time when the event occurred .</span></span> <span data-ttu-id="5dac7-135">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="5dac7-135">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="5dac7-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="5dac7-136">correlationId</span></span>|<span data-ttu-id="5dac7-137">String</span><span class="sxs-lookup"><span data-stu-id="5dac7-137">String</span></span>|<span data-ttu-id="5dac7-138">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="5dac7-138">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="5dac7-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="5dac7-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="5dac7-140">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="5dac7-140">managedDeviceIdentifier</span></span>|<span data-ttu-id="5dac7-141">String</span><span class="sxs-lookup"><span data-stu-id="5dac7-141">String</span></span>|<span data-ttu-id="5dac7-142">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="5dac7-142">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="5dac7-143">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="5dac7-143">operatingSystem</span></span>|<span data-ttu-id="5dac7-144">String</span><span class="sxs-lookup"><span data-stu-id="5dac7-144">String</span></span>|<span data-ttu-id="5dac7-145">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="5dac7-145">Operating System.</span></span>|
|<span data-ttu-id="5dac7-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="5dac7-146">osVersion</span></span>|<span data-ttu-id="5dac7-147">String</span><span class="sxs-lookup"><span data-stu-id="5dac7-147">String</span></span>|<span data-ttu-id="5dac7-148">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="5dac7-148">OS Version.</span></span>|
|<span data-ttu-id="5dac7-149">userId</span><span class="sxs-lookup"><span data-stu-id="5dac7-149">userId</span></span>|<span data-ttu-id="5dac7-150">String</span><span class="sxs-lookup"><span data-stu-id="5dac7-150">String</span></span>|<span data-ttu-id="5dac7-151">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="5dac7-151">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="5dac7-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="5dac7-152">deviceId</span></span>|<span data-ttu-id="5dac7-153">String</span><span class="sxs-lookup"><span data-stu-id="5dac7-153">String</span></span>|<span data-ttu-id="5dac7-154">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5dac7-154">Azure AD device identifier.</span></span>|
|<span data-ttu-id="5dac7-155">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="5dac7-155">enrollmentType</span></span>|[<span data-ttu-id="5dac7-156">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5dac7-156">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="5dac7-157">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="5dac7-157">Type of the enrollment.</span></span> <span data-ttu-id="5dac7-158">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="5dac7-158">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="5dac7-159">failureCategory</span><span class="sxs-lookup"><span data-stu-id="5dac7-159">failureCategory</span></span>|[<span data-ttu-id="5dac7-160">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="5dac7-160">deviceEnrollmentFailureReason</span></span>](../resources/intune_troubleshooting_deviceenrollmentfailurereason.md)|<span data-ttu-id="5dac7-161">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="5dac7-161">Highlevel failure category.</span></span> <span data-ttu-id="5dac7-162">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="5dac7-162">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="5dac7-163">failureReason</span><span class="sxs-lookup"><span data-stu-id="5dac7-163">failureReason</span></span>|<span data-ttu-id="5dac7-164">String</span><span class="sxs-lookup"><span data-stu-id="5dac7-164">String</span></span>|<span data-ttu-id="5dac7-165">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="5dac7-165">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="5dac7-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="5dac7-166">Response</span></span>
<span data-ttu-id="5dac7-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5dac7-167">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dac7-168">Пример</span><span class="sxs-lookup"><span data-stu-id="5dac7-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="5dac7-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="5dac7-169">Request</span></span>
<span data-ttu-id="5dac7-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5dac7-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="5dac7-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="5dac7-171">Response</span></span>
<span data-ttu-id="5dac7-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5dac7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



