# <a name="update-devicecategory"></a><span data-ttu-id="3fc13-101">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="3fc13-101">Update deviceCategory</span></span>

> <span data-ttu-id="3fc13-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3fc13-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fc13-103">Обновление свойств объекта [deviceCategory](../resources/intune_devices_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="3fc13-103">Update the properties of a [calendar](../resources/intune_devices_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3fc13-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3fc13-104">Prerequisites</span></span>
<span data-ttu-id="3fc13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3fc13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3fc13-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fc13-107">Permission type</span></span>|<span data-ttu-id="3fc13-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fc13-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fc13-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fc13-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3fc13-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fc13-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3fc13-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fc13-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fc13-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fc13-112">Not supported.</span></span>|
|<span data-ttu-id="3fc13-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fc13-113">Application</span></span>|<span data-ttu-id="3fc13-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fc13-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fc13-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fc13-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="3fc13-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fc13-116">Request headers</span></span>
|<span data-ttu-id="3fc13-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fc13-117">Header</span></span>|<span data-ttu-id="3fc13-118">Значение</span><span class="sxs-lookup"><span data-stu-id="3fc13-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fc13-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fc13-119">Authorization</span></span>|<span data-ttu-id="3fc13-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fc13-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3fc13-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3fc13-121">Accept</span></span>|<span data-ttu-id="3fc13-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3fc13-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fc13-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3fc13-123">Request body</span></span>
<span data-ttu-id="3fc13-124">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune_devices_devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fc13-124">In the request body, supply a JSON representation of [Attachment](../resources/intune_devices_devicecategory.md) object.</span></span>

<span data-ttu-id="3fc13-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune_devices_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="3fc13-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="3fc13-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fc13-126">Property</span></span>|<span data-ttu-id="3fc13-127">Тип</span><span class="sxs-lookup"><span data-stu-id="3fc13-127">Type</span></span>|<span data-ttu-id="3fc13-128">Описание</span><span class="sxs-lookup"><span data-stu-id="3fc13-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fc13-129">id</span><span class="sxs-lookup"><span data-stu-id="3fc13-129">id</span></span>|<span data-ttu-id="3fc13-130">String</span><span class="sxs-lookup"><span data-stu-id="3fc13-130">String</span></span>|<span data-ttu-id="3fc13-131">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="3fc13-131">Unique identifier for the device category.</span></span> <span data-ttu-id="3fc13-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fc13-132">Read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="3fc13-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fc13-133">Response</span></span>
<span data-ttu-id="3fc13-134">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune_devices_devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3fc13-134">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fc13-135">Пример</span><span class="sxs-lookup"><span data-stu-id="3fc13-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="3fc13-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fc13-136">Request</span></span>
<span data-ttu-id="3fc13-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fc13-137">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="3fc13-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="3fc13-138">Response</span></span>
<span data-ttu-id="3fc13-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3fc13-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8"
}
```



