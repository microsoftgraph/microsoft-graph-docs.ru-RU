# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="01547-101">Обновление объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="01547-101">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="01547-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="01547-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01547-103">Обновление свойств объекта [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01547-103">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01547-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="01547-104">Prerequisites</span></span>
<span data-ttu-id="01547-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01547-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01547-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01547-107">Permission type</span></span>|<span data-ttu-id="01547-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01547-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01547-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01547-109">Delegated (work or school account)</span></span>|<span data-ttu-id="01547-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01547-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01547-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01547-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01547-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01547-112">Not supported.</span></span>|
|<span data-ttu-id="01547-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01547-113">Application</span></span>|<span data-ttu-id="01547-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01547-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01547-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01547-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="01547-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01547-116">Request headers</span></span>
|<span data-ttu-id="01547-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01547-117">Header</span></span>|<span data-ttu-id="01547-118">Значение</span><span class="sxs-lookup"><span data-stu-id="01547-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01547-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01547-119">Authorization</span></span>|<span data-ttu-id="01547-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="01547-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01547-121">Принять</span><span class="sxs-lookup"><span data-stu-id="01547-121">Accept</span></span>|<span data-ttu-id="01547-122">application/json</span><span class="sxs-lookup"><span data-stu-id="01547-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01547-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01547-123">Request body</span></span>
<span data-ttu-id="01547-124">В теле запроса добавьте представление объекта [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01547-124">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="01547-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01547-125">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="01547-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="01547-126">Property</span></span>|<span data-ttu-id="01547-127">Тип</span><span class="sxs-lookup"><span data-stu-id="01547-127">Type</span></span>|<span data-ttu-id="01547-128">Описание</span><span class="sxs-lookup"><span data-stu-id="01547-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01547-129">id</span><span class="sxs-lookup"><span data-stu-id="01547-129">id</span></span>|<span data-ttu-id="01547-130">Строка</span><span class="sxs-lookup"><span data-stu-id="01547-130">String</span></span>|<span data-ttu-id="01547-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01547-131">Key of the entity.</span></span> <span data-ttu-id="01547-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01547-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01547-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01547-133">lastModifiedDateTime</span></span>|<span data-ttu-id="01547-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01547-134">DateTimeOffset</span></span>|<span data-ttu-id="01547-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="01547-135">DateTime the object was last modified.</span></span> <span data-ttu-id="01547-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01547-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01547-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01547-137">createdDateTime</span></span>|<span data-ttu-id="01547-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01547-138">DateTimeOffset</span></span>|<span data-ttu-id="01547-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="01547-139">DateTime the object was created.</span></span> <span data-ttu-id="01547-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01547-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01547-141">description</span><span class="sxs-lookup"><span data-stu-id="01547-141">description</span></span>|<span data-ttu-id="01547-142">Строка</span><span class="sxs-lookup"><span data-stu-id="01547-142">String</span></span>|<span data-ttu-id="01547-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01547-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="01547-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01547-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01547-145">displayName</span><span class="sxs-lookup"><span data-stu-id="01547-145">displayName</span></span>|<span data-ttu-id="01547-146">Строка</span><span class="sxs-lookup"><span data-stu-id="01547-146">String</span></span>|<span data-ttu-id="01547-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01547-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="01547-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01547-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01547-149">version</span><span class="sxs-lookup"><span data-stu-id="01547-149">version</span></span>|<span data-ttu-id="01547-150">Int32</span><span class="sxs-lookup"><span data-stu-id="01547-150">Int32</span></span>|<span data-ttu-id="01547-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01547-151">Version of the device configuration.</span></span> <span data-ttu-id="01547-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01547-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="01547-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="01547-153">Response</span></span>
<span data-ttu-id="01547-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01547-154">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01547-155">Пример</span><span class="sxs-lookup"><span data-stu-id="01547-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="01547-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="01547-156">Request</span></span>
<span data-ttu-id="01547-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01547-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 163

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="01547-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="01547-158">Response</span></span>
<span data-ttu-id="01547-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01547-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```








