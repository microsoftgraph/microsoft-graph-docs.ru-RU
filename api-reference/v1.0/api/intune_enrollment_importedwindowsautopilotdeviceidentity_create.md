# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="96cd8-101">Создать importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="96cd8-101">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="96cd8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="96cd8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96cd8-103">Создать новый объект [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="96cd8-103">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96cd8-104">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="96cd8-104">Prerequisites</span></span>
<span data-ttu-id="96cd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="96cd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="96cd8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96cd8-107">Permission type</span></span>|<span data-ttu-id="96cd8-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96cd8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96cd8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96cd8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="96cd8-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96cd8-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="96cd8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96cd8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96cd8-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96cd8-112">Not supported.</span></span>|
|<span data-ttu-id="96cd8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96cd8-113">Application</span></span>|<span data-ttu-id="96cd8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96cd8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96cd8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96cd8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="96cd8-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="96cd8-116">Request headers</span></span>
|<span data-ttu-id="96cd8-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96cd8-117">Header</span></span>|<span data-ttu-id="96cd8-118">Значение</span><span class="sxs-lookup"><span data-stu-id="96cd8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96cd8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="96cd8-119">Authorization</span></span>|<span data-ttu-id="96cd8-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96cd8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96cd8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="96cd8-121">Accept</span></span>|<span data-ttu-id="96cd8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="96cd8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96cd8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96cd8-123">Request body</span></span>
<span data-ttu-id="96cd8-124">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96cd8-124">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="96cd8-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="96cd8-125">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="96cd8-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="96cd8-126">Property</span></span>|<span data-ttu-id="96cd8-127">Тип</span><span class="sxs-lookup"><span data-stu-id="96cd8-127">Type</span></span>|<span data-ttu-id="96cd8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="96cd8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96cd8-129">id</span><span class="sxs-lookup"><span data-stu-id="96cd8-129">id</span></span>|<span data-ttu-id="96cd8-130">Строка</span><span class="sxs-lookup"><span data-stu-id="96cd8-130">String</span></span>|<span data-ttu-id="96cd8-131">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="96cd8-131">The GUID for the object.</span></span>|
|<span data-ttu-id="96cd8-132">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="96cd8-132">orderIdentifier</span></span>|<span data-ttu-id="96cd8-133">Строка</span><span class="sxs-lookup"><span data-stu-id="96cd8-133">String</span></span>|<span data-ttu-id="96cd8-134">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="96cd8-134">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="96cd8-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="96cd8-135">serialNumber</span></span>|<span data-ttu-id="96cd8-136">Строка</span><span class="sxs-lookup"><span data-stu-id="96cd8-136">String</span></span>|<span data-ttu-id="96cd8-137">Серийный номер устройства Windows autopilot.</span><span class="sxs-lookup"><span data-stu-id="96cd8-137">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="96cd8-138">productKey</span><span class="sxs-lookup"><span data-stu-id="96cd8-138">productKey</span></span>|<span data-ttu-id="96cd8-139">Строка</span><span class="sxs-lookup"><span data-stu-id="96cd8-139">String</span></span>|<span data-ttu-id="96cd8-140">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="96cd8-140">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="96cd8-141">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="96cd8-141">hardwareIdentifier</span></span>|<span data-ttu-id="96cd8-142">Двоичный</span><span class="sxs-lookup"><span data-stu-id="96cd8-142">Binary</span></span>|<span data-ttu-id="96cd8-143">Комплектующие BLOB-объектов устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="96cd8-143">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="96cd8-144">состояние</span><span class="sxs-lookup"><span data-stu-id="96cd8-144">state</span></span>|[<span data-ttu-id="96cd8-145">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="96cd8-145">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="96cd8-146">Текущее состояние импортируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="96cd8-146">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="96cd8-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="96cd8-147">Response</span></span>
<span data-ttu-id="96cd8-148">В случае успешного выполнения данный метод возвращает код отклика `201 Created` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="96cd8-148">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96cd8-149">Пример</span><span class="sxs-lookup"><span data-stu-id="96cd8-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="96cd8-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="96cd8-150">Request</span></span>
<span data-ttu-id="96cd8-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96cd8-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 541

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
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

### <a name="response"></a><span data-ttu-id="96cd8-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="96cd8-152">Response</span></span>
<span data-ttu-id="96cd8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="96cd8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



