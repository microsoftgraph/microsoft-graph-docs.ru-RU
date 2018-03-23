# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="79745-101">Создание объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="79745-101">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="79745-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="79745-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79745-103">Создание объекта [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79745-103">Create a new [plannerBucket](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79745-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79745-104">Prerequisites</span></span>
<span data-ttu-id="79745-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="79745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="79745-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79745-107">Permission type</span></span>|<span data-ttu-id="79745-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79745-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79745-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79745-109">Delegated (work or school account)</span></span>|<span data-ttu-id="79745-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79745-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79745-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79745-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79745-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79745-112">Not supported.</span></span>|
|<span data-ttu-id="79745-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79745-113">Application</span></span>|<span data-ttu-id="79745-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79745-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79745-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79745-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="79745-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79745-116">Request headers</span></span>
|<span data-ttu-id="79745-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79745-117">Header</span></span>|<span data-ttu-id="79745-118">Значение</span><span class="sxs-lookup"><span data-stu-id="79745-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79745-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="79745-119">Authorization</span></span>|<span data-ttu-id="79745-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79745-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="79745-121">Accept</span><span class="sxs-lookup"><span data-stu-id="79745-121">Accept</span></span>|<span data-ttu-id="79745-122">application/json</span><span class="sxs-lookup"><span data-stu-id="79745-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79745-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79745-123">Request body</span></span>
<span data-ttu-id="79745-124">В теле запроса добавьте представление объекта macOSDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79745-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="79745-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="79745-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="79745-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="79745-126">Property</span></span>|<span data-ttu-id="79745-127">Тип</span><span class="sxs-lookup"><span data-stu-id="79745-127">Type</span></span>|<span data-ttu-id="79745-128">Описание</span><span class="sxs-lookup"><span data-stu-id="79745-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79745-129">id</span><span class="sxs-lookup"><span data-stu-id="79745-129">id</span></span>|<span data-ttu-id="79745-130">String</span><span class="sxs-lookup"><span data-stu-id="79745-130">String</span></span>|<span data-ttu-id="79745-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="79745-131">Key of the setting.</span></span> <span data-ttu-id="79745-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79745-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79745-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79745-133">lastModifiedDateTime</span></span>|<span data-ttu-id="79745-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79745-134">DateTimeOffset</span></span>|<span data-ttu-id="79745-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="79745-135">DateTime the object was last modified.</span></span> <span data-ttu-id="79745-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79745-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79745-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79745-137">createdDateTime</span></span>|<span data-ttu-id="79745-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79745-138">DateTimeOffset</span></span>|<span data-ttu-id="79745-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="79745-139">DateTime the object was created.</span></span> <span data-ttu-id="79745-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79745-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79745-141">description</span><span class="sxs-lookup"><span data-stu-id="79745-141">description</span></span>|<span data-ttu-id="79745-142">String</span><span class="sxs-lookup"><span data-stu-id="79745-142">String</span></span>|<span data-ttu-id="79745-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79745-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="79745-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79745-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79745-145">displayName</span><span class="sxs-lookup"><span data-stu-id="79745-145">displayName</span></span>|<span data-ttu-id="79745-146">String</span><span class="sxs-lookup"><span data-stu-id="79745-146">String</span></span>|<span data-ttu-id="79745-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79745-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="79745-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79745-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79745-149">version</span><span class="sxs-lookup"><span data-stu-id="79745-149">version</span></span>|<span data-ttu-id="79745-150">Int32</span><span class="sxs-lookup"><span data-stu-id="79745-150">Int32</span></span>|<span data-ttu-id="79745-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="79745-151">Version of the device configuration.</span></span> <span data-ttu-id="79745-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79745-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="79745-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="79745-153">Response</span></span>
<span data-ttu-id="79745-154">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="79745-154">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79745-155">Пример</span><span class="sxs-lookup"><span data-stu-id="79745-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="79745-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="79745-156">Request</span></span>
<span data-ttu-id="79745-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79745-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="79745-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="79745-158">Response</span></span>
<span data-ttu-id="79745-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="79745-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



