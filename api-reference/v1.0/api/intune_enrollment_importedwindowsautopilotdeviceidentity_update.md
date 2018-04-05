# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="a4796-101">Обновление importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a4796-101">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="a4796-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a4796-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4796-103">Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="a4796-103">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4796-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a4796-104">Prerequisites</span></span>
<span data-ttu-id="a4796-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a4796-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a4796-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4796-107">Permission type</span></span>|<span data-ttu-id="a4796-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4796-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4796-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4796-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a4796-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4796-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a4796-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4796-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4796-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4796-112">Not supported.</span></span>|
|<span data-ttu-id="a4796-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4796-113">Application</span></span>|<span data-ttu-id="a4796-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4796-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4796-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4796-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="a4796-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a4796-116">Request headers</span></span>
|<span data-ttu-id="a4796-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4796-117">Header</span></span>|<span data-ttu-id="a4796-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a4796-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4796-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4796-119">Authorization</span></span>|<span data-ttu-id="a4796-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4796-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4796-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a4796-121">Accept</span></span>|<span data-ttu-id="a4796-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a4796-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4796-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a4796-123">Request body</span></span>
<span data-ttu-id="a4796-124">В теле запроса добавьте представление объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4796-124">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="a4796-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="a4796-125">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="a4796-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4796-126">Property</span></span>|<span data-ttu-id="a4796-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a4796-127">Type</span></span>|<span data-ttu-id="a4796-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a4796-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4796-129">id</span><span class="sxs-lookup"><span data-stu-id="a4796-129">id</span></span>|<span data-ttu-id="a4796-130">Строка</span><span class="sxs-lookup"><span data-stu-id="a4796-130">String</span></span>|<span data-ttu-id="a4796-131">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="a4796-131">The GUID for the object.</span></span>|
|<span data-ttu-id="a4796-132">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="a4796-132">orderIdentifier</span></span>|<span data-ttu-id="a4796-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a4796-133">String</span></span>|<span data-ttu-id="a4796-134">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="a4796-134">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a4796-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a4796-135">serialNumber</span></span>|<span data-ttu-id="a4796-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a4796-136">String</span></span>|<span data-ttu-id="a4796-137">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="a4796-137">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a4796-138">productKey</span><span class="sxs-lookup"><span data-stu-id="a4796-138">productKey</span></span>|<span data-ttu-id="a4796-139">Строка</span><span class="sxs-lookup"><span data-stu-id="a4796-139">String</span></span>|<span data-ttu-id="a4796-140">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="a4796-140">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a4796-141">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="a4796-141">hardwareIdentifier</span></span>|<span data-ttu-id="a4796-142">Двоичный</span><span class="sxs-lookup"><span data-stu-id="a4796-142">Binary</span></span>|<span data-ttu-id="a4796-143">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="a4796-143">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a4796-144">state</span><span class="sxs-lookup"><span data-stu-id="a4796-144">state</span></span>|[<span data-ttu-id="a4796-145">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="a4796-145">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="a4796-146">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="a4796-146">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="a4796-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4796-147">Response</span></span>
<span data-ttu-id="a4796-148">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a4796-148">If successful, this method returns a `200 OK` response code and an updated [iosManagedAppProtection](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4796-149">Пример</span><span class="sxs-lookup"><span data-stu-id="a4796-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4796-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4796-150">Request</span></span>
<span data-ttu-id="a4796-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4796-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 464

{
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```

### <a name="response"></a><span data-ttu-id="a4796-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4796-152">Response</span></span>
<span data-ttu-id="a4796-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a4796-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```



