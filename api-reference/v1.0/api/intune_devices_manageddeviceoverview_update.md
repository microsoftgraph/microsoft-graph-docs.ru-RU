# <a name="update-manageddeviceoverview"></a><span data-ttu-id="5c395-101">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5c395-101">Update managedDeviceOverview</span></span>

> <span data-ttu-id="5c395-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5c395-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c395-103">Обновление свойств объекта [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="5c395-103">Update the properties of a [calendar](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c395-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5c395-104">Prerequisites</span></span>
<span data-ttu-id="5c395-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5c395-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5c395-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c395-107">Permission type</span></span>|<span data-ttu-id="5c395-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c395-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c395-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c395-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5c395-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c395-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5c395-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c395-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c395-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c395-112">Not supported.</span></span>|
|<span data-ttu-id="5c395-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c395-113">Application</span></span>|<span data-ttu-id="5c395-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c395-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c395-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c395-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="5c395-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c395-116">Request headers</span></span>
|<span data-ttu-id="5c395-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c395-117">Header</span></span>|<span data-ttu-id="5c395-118">Значение</span><span class="sxs-lookup"><span data-stu-id="5c395-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c395-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c395-119">Authorization</span></span>|<span data-ttu-id="5c395-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c395-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5c395-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5c395-121">Accept</span></span>|<span data-ttu-id="5c395-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5c395-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c395-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c395-123">Request body</span></span>
<span data-ttu-id="5c395-124">В теле запроса добавьте представление объекта [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c395-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="5c395-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="5c395-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5c395-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c395-126">Property</span></span>|<span data-ttu-id="5c395-127">Тип</span><span class="sxs-lookup"><span data-stu-id="5c395-127">Type</span></span>|<span data-ttu-id="5c395-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5c395-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c395-129">id</span><span class="sxs-lookup"><span data-stu-id="5c395-129">id</span></span>|<span data-ttu-id="5c395-130">String</span><span class="sxs-lookup"><span data-stu-id="5c395-130">String</span></span>|<span data-ttu-id="5c395-131">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="5c395-131">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="5c395-132">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c395-132">enrolledDeviceCount</span></span>|<span data-ttu-id="5c395-133">Int32</span><span class="sxs-lookup"><span data-stu-id="5c395-133">Int32</span></span>|<span data-ttu-id="5c395-134">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="5c395-134">Total enrolled device count.</span></span> <span data-ttu-id="5c395-135">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="5c395-135">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="5c395-136">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="5c395-136">mdmEnrolledCount</span></span>|<span data-ttu-id="5c395-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5c395-137">Int32</span></span>|<span data-ttu-id="5c395-138">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="5c395-138">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="5c395-139">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5c395-139">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="5c395-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5c395-140">Int32</span></span>|<span data-ttu-id="5c395-141">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="5c395-141">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="5c395-142">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="5c395-142">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="5c395-143">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="5c395-143">deviceOperatingSystemSummary</span></span>](../resources/intune_devices_deviceoperatingsystemsummary.md)|<span data-ttu-id="5c395-144">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="5c395-144">Device operating system summary.</span></span>|
|<span data-ttu-id="5c395-145">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="5c395-145">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="5c395-146">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="5c395-146">deviceExchangeAccessStateSummary</span></span>](../resources/intune_devices_deviceexchangeaccessstatesummary.md)|<span data-ttu-id="5c395-147">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="5c395-147">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="5c395-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c395-148">Response</span></span>
<span data-ttu-id="5c395-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5c395-149">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c395-150">Пример</span><span class="sxs-lookup"><span data-stu-id="5c395-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c395-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c395-151">Request</span></span>
<span data-ttu-id="5c395-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c395-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 625

{
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```

### <a name="response"></a><span data-ttu-id="5c395-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c395-153">Response</span></span>
<span data-ttu-id="5c395-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c395-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 734

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "42a91653-1653-42a9-5316-a9425316a942",
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```



