# <a name="update-devicecategory"></a><span data-ttu-id="62c61-101">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="62c61-101">Update deviceCategory</span></span>

> <span data-ttu-id="62c61-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="62c61-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62c61-103">Обновление свойств объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="62c61-103">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62c61-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="62c61-104">Prerequisites</span></span>
<span data-ttu-id="62c61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="62c61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="62c61-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62c61-107">Permission type</span></span>|<span data-ttu-id="62c61-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62c61-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62c61-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62c61-109">Delegated (work or school account)</span></span>|<span data-ttu-id="62c61-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62c61-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="62c61-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62c61-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62c61-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62c61-112">Not supported.</span></span>|
|<span data-ttu-id="62c61-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62c61-113">Application</span></span>|<span data-ttu-id="62c61-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62c61-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62c61-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62c61-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="62c61-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="62c61-116">Request headers</span></span>
|<span data-ttu-id="62c61-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62c61-117">Header</span></span>|<span data-ttu-id="62c61-118">Значение</span><span class="sxs-lookup"><span data-stu-id="62c61-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62c61-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="62c61-119">Authorization</span></span>|<span data-ttu-id="62c61-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62c61-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62c61-121">Accept</span><span class="sxs-lookup"><span data-stu-id="62c61-121">Accept</span></span>|<span data-ttu-id="62c61-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="62c61-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62c61-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="62c61-123">Request body</span></span>
<span data-ttu-id="62c61-124">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune_shared_devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62c61-124">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

<span data-ttu-id="62c61-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="62c61-125">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>

|<span data-ttu-id="62c61-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="62c61-126">Property</span></span>|<span data-ttu-id="62c61-127">Тип</span><span class="sxs-lookup"><span data-stu-id="62c61-127">Type</span></span>|<span data-ttu-id="62c61-128">Описание</span><span class="sxs-lookup"><span data-stu-id="62c61-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62c61-129">id</span><span class="sxs-lookup"><span data-stu-id="62c61-129">id</span></span>|<span data-ttu-id="62c61-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="62c61-130">String</span></span>|<span data-ttu-id="62c61-131">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="62c61-131">Unique identifier for the device category.</span></span> <span data-ttu-id="62c61-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62c61-132">Read-only.</span></span>|
|<span data-ttu-id="62c61-133">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="62c61-133">**On-boarding**</span></span>|
|<span data-ttu-id="62c61-134">displayName</span><span class="sxs-lookup"><span data-stu-id="62c61-134">displayName</span></span>|<span data-ttu-id="62c61-135">String (строка)</span><span class="sxs-lookup"><span data-stu-id="62c61-135">String</span></span>|<span data-ttu-id="62c61-136">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="62c61-136">Display name for the device category.</span></span>|
|<span data-ttu-id="62c61-137">description</span><span class="sxs-lookup"><span data-stu-id="62c61-137">description</span></span>|<span data-ttu-id="62c61-138">String (строка)</span><span class="sxs-lookup"><span data-stu-id="62c61-138">String</span></span>|<span data-ttu-id="62c61-139">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="62c61-139">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="62c61-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="62c61-140">Response</span></span>
<span data-ttu-id="62c61-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune_shared_devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="62c61-141">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62c61-142">Пример</span><span class="sxs-lookup"><span data-stu-id="62c61-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="62c61-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="62c61-143">Request</span></span>
<span data-ttu-id="62c61-144">Ниже приведены примеры запросов.</span><span class="sxs-lookup"><span data-stu-id="62c61-144">Here are a couple of examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="62c61-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="62c61-145">Response</span></span>
<span data-ttu-id="62c61-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="62c61-146">Here is an example of the response.</span></span> <span data-ttu-id="62c61-147">Примечание: представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="62c61-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="62c61-148">Свойства ответа будут отличаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="62c61-148">Response properties will vary according to context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



