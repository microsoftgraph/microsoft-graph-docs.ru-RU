# <a name="update-devicecategory"></a><span data-ttu-id="0ac27-101">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0ac27-101">Update deviceCategory</span></span>

> <span data-ttu-id="0ac27-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0ac27-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ac27-103">Обновление свойств объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="0ac27-103">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ac27-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0ac27-104">Prerequisites</span></span>
<span data-ttu-id="0ac27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ac27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0ac27-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ac27-107">Permission type</span></span>|<span data-ttu-id="0ac27-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ac27-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ac27-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ac27-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0ac27-110">&nbsp;&nbsp; **Адаптация новых сотрудников** и</span><span class="sxs-lookup"><span data-stu-id="0ac27-110">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="0ac27-111">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="0ac27-111">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="0ac27-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac27-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0ac27-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ac27-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ac27-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ac27-114">Not supported.</span></span>|
|<span data-ttu-id="0ac27-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ac27-115">Application</span></span>|<span data-ttu-id="0ac27-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ac27-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ac27-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ac27-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="0ac27-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ac27-118">Request headers</span></span>
|<span data-ttu-id="0ac27-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ac27-119">Header</span></span>|<span data-ttu-id="0ac27-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0ac27-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ac27-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ac27-121">Authorization</span></span>|<span data-ttu-id="0ac27-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0ac27-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ac27-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0ac27-123">Accept</span></span>|<span data-ttu-id="0ac27-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0ac27-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ac27-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ac27-125">Request body</span></span>
<span data-ttu-id="0ac27-126">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune_shared_devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ac27-126">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

<span data-ttu-id="0ac27-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="0ac27-127">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>

|<span data-ttu-id="0ac27-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ac27-128">Property</span></span>|<span data-ttu-id="0ac27-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0ac27-129">Type</span></span>|<span data-ttu-id="0ac27-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0ac27-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ac27-131">id</span><span class="sxs-lookup"><span data-stu-id="0ac27-131">id</span></span>|<span data-ttu-id="0ac27-132">String</span><span class="sxs-lookup"><span data-stu-id="0ac27-132">String</span></span>|<span data-ttu-id="0ac27-133">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="0ac27-133">Unique identifier for the device category.</span></span> <span data-ttu-id="0ac27-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ac27-134">Read-only.</span></span>|
|<span data-ttu-id="0ac27-135">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="0ac27-135">**Onboarding**</span></span>|
|<span data-ttu-id="0ac27-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0ac27-136">displayName</span></span>|<span data-ttu-id="0ac27-137">String</span><span class="sxs-lookup"><span data-stu-id="0ac27-137">String</span></span>|<span data-ttu-id="0ac27-138">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="0ac27-138">Display name for the device category.</span></span>|
|<span data-ttu-id="0ac27-139">описание</span><span class="sxs-lookup"><span data-stu-id="0ac27-139">description</span></span>|<span data-ttu-id="0ac27-140">String</span><span class="sxs-lookup"><span data-stu-id="0ac27-140">String</span></span>|<span data-ttu-id="0ac27-141">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="0ac27-141">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="0ac27-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ac27-142">Response</span></span>
<span data-ttu-id="0ac27-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune_shared_devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0ac27-143">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac27-144">Пример</span><span class="sxs-lookup"><span data-stu-id="0ac27-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ac27-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ac27-145">Request</span></span>
<span data-ttu-id="0ac27-146">Ниже приведены примеры запроса.</span><span class="sxs-lookup"><span data-stu-id="0ac27-146">Here are examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ac27-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ac27-147">Response</span></span>
<span data-ttu-id="0ac27-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ac27-148">Here is an example of the response.</span></span> <span data-ttu-id="0ac27-149">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="0ac27-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0ac27-150">Свойства ответа будет отличаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="0ac27-150">Response properties will vary according to context.</span></span>
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



