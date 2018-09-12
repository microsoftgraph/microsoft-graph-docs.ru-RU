# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="8edeb-101">Создание объекта enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8edeb-101">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="8edeb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8edeb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8edeb-103">Создание объекта [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8edeb-103">Create a new [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8edeb-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8edeb-104">Prerequisites</span></span>
<span data-ttu-id="8edeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8edeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8edeb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8edeb-107">Permission type</span></span>|<span data-ttu-id="8edeb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8edeb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8edeb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8edeb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8edeb-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8edeb-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8edeb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8edeb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8edeb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8edeb-112">Not supported.</span></span>|
|<span data-ttu-id="8edeb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8edeb-113">Application</span></span>|<span data-ttu-id="8edeb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8edeb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8edeb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8edeb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="8edeb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8edeb-116">Request headers</span></span>
|<span data-ttu-id="8edeb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8edeb-117">Header</span></span>|<span data-ttu-id="8edeb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8edeb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8edeb-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8edeb-119">Authorization</span></span>|<span data-ttu-id="8edeb-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="8edeb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8edeb-121">Принять</span><span class="sxs-lookup"><span data-stu-id="8edeb-121">Accept</span></span>|<span data-ttu-id="8edeb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8edeb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8edeb-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8edeb-123">Request body</span></span>
<span data-ttu-id="8edeb-124">В теле запроса добавьте представление объекта enrollmentTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8edeb-124">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="8edeb-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="8edeb-125">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="8edeb-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="8edeb-126">Property</span></span>|<span data-ttu-id="8edeb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8edeb-127">Type</span></span>|<span data-ttu-id="8edeb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8edeb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8edeb-129">id</span><span class="sxs-lookup"><span data-stu-id="8edeb-129">id</span></span>|<span data-ttu-id="8edeb-130">Строка</span><span class="sxs-lookup"><span data-stu-id="8edeb-130">String</span></span>|<span data-ttu-id="8edeb-131">UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8edeb-131">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8edeb-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="8edeb-132">eventDateTime</span></span>|<span data-ttu-id="8edeb-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8edeb-133">DateTimeOffset</span></span>|<span data-ttu-id="8edeb-134">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="8edeb-134">Time when the event occurred .</span></span> <span data-ttu-id="8edeb-135">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8edeb-135">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8edeb-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="8edeb-136">correlationId</span></span>|<span data-ttu-id="8edeb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="8edeb-137">String</span></span>|<span data-ttu-id="8edeb-138">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="8edeb-138">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="8edeb-139">Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8edeb-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="8edeb-140">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8edeb-140">managedDeviceIdentifier</span></span>|<span data-ttu-id="8edeb-141">Строка</span><span class="sxs-lookup"><span data-stu-id="8edeb-141">String</span></span>|<span data-ttu-id="8edeb-142">Идентификатор события, созданный или полученный службой Intune.</span><span class="sxs-lookup"><span data-stu-id="8edeb-142">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="8edeb-143">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8edeb-143">operatingSystem</span></span>|<span data-ttu-id="8edeb-144">Строка</span><span class="sxs-lookup"><span data-stu-id="8edeb-144">String</span></span>|<span data-ttu-id="8edeb-145">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="8edeb-145">Operating System.</span></span>|
|<span data-ttu-id="8edeb-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="8edeb-146">osVersion</span></span>|<span data-ttu-id="8edeb-147">Строка</span><span class="sxs-lookup"><span data-stu-id="8edeb-147">String</span></span>|<span data-ttu-id="8edeb-148">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="8edeb-148">OS Version.</span></span>|
|<span data-ttu-id="8edeb-149">userId</span><span class="sxs-lookup"><span data-stu-id="8edeb-149">userId</span></span>|<span data-ttu-id="8edeb-150">Строка</span><span class="sxs-lookup"><span data-stu-id="8edeb-150">String</span></span>|<span data-ttu-id="8edeb-151">Идентификатор пользователя, который пытался зарегистрировать устройство.</span><span class="sxs-lookup"><span data-stu-id="8edeb-151">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="8edeb-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="8edeb-152">deviceId</span></span>|<span data-ttu-id="8edeb-153">Строка</span><span class="sxs-lookup"><span data-stu-id="8edeb-153">String</span></span>|<span data-ttu-id="8edeb-154">Идентификатор устройства Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8edeb-154">Azure AD device identifier.</span></span>|
|<span data-ttu-id="8edeb-155">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="8edeb-155">enrollmentType</span></span>|[<span data-ttu-id="8edeb-156">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="8edeb-156">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="8edeb-157">Тип регистрации.</span><span class="sxs-lookup"><span data-stu-id="8edeb-157">Type of the enrollment.</span></span> <span data-ttu-id="8edeb-158">Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="8edeb-158">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="8edeb-159">failureCategory</span><span class="sxs-lookup"><span data-stu-id="8edeb-159">failureCategory</span></span>|[<span data-ttu-id="8edeb-160">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="8edeb-160">deviceEnrollmentFailureReason values</span></span>](../resources/intune_troubleshooting_deviceenrollmentfailurereason.md)|<span data-ttu-id="8edeb-161">Категория сбоя высокого уровня.</span><span class="sxs-lookup"><span data-stu-id="8edeb-161">Highlevel failure category.</span></span> <span data-ttu-id="8edeb-162">Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span><span class="sxs-lookup"><span data-stu-id="8edeb-162">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="8edeb-163">failureReason</span><span class="sxs-lookup"><span data-stu-id="8edeb-163">failureReason</span></span>|<span data-ttu-id="8edeb-164">Строка</span><span class="sxs-lookup"><span data-stu-id="8edeb-164">String</span></span>|<span data-ttu-id="8edeb-165">Подробная причина ошибки.</span><span class="sxs-lookup"><span data-stu-id="8edeb-165">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="8edeb-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="8edeb-166">Response</span></span>
<span data-ttu-id="8edeb-167">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8edeb-167">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8edeb-168">Пример</span><span class="sxs-lookup"><span data-stu-id="8edeb-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="8edeb-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="8edeb-169">Request</span></span>
<span data-ttu-id="8edeb-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8edeb-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="8edeb-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="8edeb-171">Response</span></span>
<span data-ttu-id="8edeb-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8edeb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




