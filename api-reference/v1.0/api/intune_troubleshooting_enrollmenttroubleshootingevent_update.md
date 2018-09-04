# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="9f87d-101">Обновление enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="9f87d-101">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="9f87d-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9f87d-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f87d-103">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f87d-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f87d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9f87d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f87d-105">Обновление свойств объекта [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="9f87d-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f87d-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f87d-106">Prerequisites</span></span>
<span data-ttu-id="9f87d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f87d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9f87d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f87d-109">Permission type</span></span>|<span data-ttu-id="9f87d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f87d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f87d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f87d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f87d-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f87d-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9f87d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f87d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f87d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f87d-114">Not supported.</span></span>|
|<span data-ttu-id="9f87d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f87d-115">Application</span></span>|<span data-ttu-id="9f87d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f87d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f87d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f87d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="9f87d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f87d-118">Request headers</span></span>
|<span data-ttu-id="9f87d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f87d-119">Header</span></span>|<span data-ttu-id="9f87d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9f87d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f87d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f87d-121">Authorization</span></span>|<span data-ttu-id="9f87d-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="9f87d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f87d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9f87d-123">Accept</span></span>|<span data-ttu-id="9f87d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9f87d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f87d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f87d-125">Request body</span></span>
<span data-ttu-id="9f87d-126">В теле запроса добавьте представление объекта [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f87d-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="9f87d-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="9f87d-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="9f87d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f87d-128">Property</span></span>|<span data-ttu-id="9f87d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9f87d-129">Type</span></span>|<span data-ttu-id="9f87d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9f87d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f87d-131">id</span><span class="sxs-lookup"><span data-stu-id="9f87d-131">id</span></span>|<span data-ttu-id="9f87d-132">String</span><span class="sxs-lookup"><span data-stu-id="9f87d-132">String</span></span>|<span data-ttu-id="9f87d-133">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="9f87d-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="9f87d-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="9f87d-134">eventDateTime</span></span>|<span data-ttu-id="9f87d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f87d-135">DateTimeOffset</span></span>|<span data-ttu-id="9f87d-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="9f87d-136">Time when the event occurred .</span></span> <span data-ttu-id="9f87d-137">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="9f87d-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="9f87d-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="9f87d-138">correlationId</span></span>|<span data-ttu-id="9f87d-139">String</span><span class="sxs-lookup"><span data-stu-id="9f87d-139">String</span></span>|<span data-ttu-id="9f87d-140">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="9f87d-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="9f87d-141">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="9f87d-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="9f87d-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9f87d-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="9f87d-143">String</span><span class="sxs-lookup"><span data-stu-id="9f87d-143">String</span></span>|<span data-ttu-id="9f87d-144">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="9f87d-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="9f87d-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="9f87d-145">operatingSystem</span></span>|<span data-ttu-id="9f87d-146">String</span><span class="sxs-lookup"><span data-stu-id="9f87d-146">String</span></span>|<span data-ttu-id="9f87d-147">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="9f87d-147">Operating System.</span></span>|
|<span data-ttu-id="9f87d-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="9f87d-148">osVersion</span></span>|<span data-ttu-id="9f87d-149">String</span><span class="sxs-lookup"><span data-stu-id="9f87d-149">String</span></span>|<span data-ttu-id="9f87d-150">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="9f87d-150">OS Version.</span></span>|
|<span data-ttu-id="9f87d-151">userId</span><span class="sxs-lookup"><span data-stu-id="9f87d-151">userId</span></span>|<span data-ttu-id="9f87d-152">String</span><span class="sxs-lookup"><span data-stu-id="9f87d-152">String</span></span>|<span data-ttu-id="9f87d-153">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="9f87d-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="9f87d-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="9f87d-154">deviceId</span></span>|<span data-ttu-id="9f87d-155">String</span><span class="sxs-lookup"><span data-stu-id="9f87d-155">String</span></span>|<span data-ttu-id="9f87d-156">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9f87d-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="9f87d-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="9f87d-157">enrollmentType</span></span>|[<span data-ttu-id="9f87d-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9f87d-158">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="9f87d-159">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="9f87d-159">Type of the enrollment.</span></span> <span data-ttu-id="9f87d-160">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="9f87d-160">The possible values are `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, , or .</span></span>|
|<span data-ttu-id="9f87d-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="9f87d-161">failureCategory</span></span>|[<span data-ttu-id="9f87d-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="9f87d-162">deviceEnrollmentFailureReason values</span></span>](../resources/intune_troubleshooting_deviceenrollmentfailurereason.md)|<span data-ttu-id="9f87d-163">Категория ошибки высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="9f87d-163">Highlevel failure category.</span></span> <span data-ttu-id="9f87d-164">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span><span class="sxs-lookup"><span data-stu-id="9f87d-164">The possible values are `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, or .</span></span>|
|<span data-ttu-id="9f87d-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="9f87d-165">failureReason</span></span>|<span data-ttu-id="9f87d-166">String</span><span class="sxs-lookup"><span data-stu-id="9f87d-166">String</span></span>|<span data-ttu-id="9f87d-167">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="9f87d-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="9f87d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f87d-168">Response</span></span>
<span data-ttu-id="9f87d-169">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9f87d-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f87d-170">Пример</span><span class="sxs-lookup"><span data-stu-id="9f87d-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f87d-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f87d-171">Request</span></span>
<span data-ttu-id="9f87d-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f87d-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="9f87d-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f87d-173">Response</span></span>
<span data-ttu-id="9f87d-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f87d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



