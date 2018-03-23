# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="d3046-101">Создание объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3046-101">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="d3046-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d3046-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3046-103">Создание объекта [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3046-103">Create a new [plannerBucket](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3046-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d3046-104">Prerequisites</span></span>
<span data-ttu-id="d3046-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d3046-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d3046-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3046-107">Permission type</span></span>|<span data-ttu-id="d3046-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3046-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3046-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3046-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d3046-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3046-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3046-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3046-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3046-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3046-112">Not supported.</span></span>|
|<span data-ttu-id="d3046-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3046-113">Application</span></span>|<span data-ttu-id="d3046-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3046-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3046-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3046-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d3046-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3046-116">Request headers</span></span>
|<span data-ttu-id="d3046-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3046-117">Header</span></span>|<span data-ttu-id="d3046-118">Значение</span><span class="sxs-lookup"><span data-stu-id="d3046-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3046-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3046-119">Authorization</span></span>|<span data-ttu-id="d3046-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3046-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d3046-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d3046-121">Accept</span></span>|<span data-ttu-id="d3046-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d3046-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3046-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d3046-123">Request body</span></span>
<span data-ttu-id="d3046-124">В теле запроса добавьте представление объекта iosCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3046-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="d3046-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d3046-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d3046-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3046-126">Property</span></span>|<span data-ttu-id="d3046-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d3046-127">Type</span></span>|<span data-ttu-id="d3046-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d3046-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3046-129">id</span><span class="sxs-lookup"><span data-stu-id="d3046-129">id</span></span>|<span data-ttu-id="d3046-130">String</span><span class="sxs-lookup"><span data-stu-id="d3046-130">String</span></span>|<span data-ttu-id="d3046-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d3046-131">Key of the setting.</span></span> <span data-ttu-id="d3046-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3046-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3046-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3046-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d3046-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3046-134">DateTimeOffset</span></span>|<span data-ttu-id="d3046-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d3046-135">DateTime the object was last modified.</span></span> <span data-ttu-id="d3046-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3046-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3046-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3046-137">createdDateTime</span></span>|<span data-ttu-id="d3046-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3046-138">DateTimeOffset</span></span>|<span data-ttu-id="d3046-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d3046-139">DateTime the object was created.</span></span> <span data-ttu-id="d3046-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3046-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3046-141">description</span><span class="sxs-lookup"><span data-stu-id="d3046-141">description</span></span>|<span data-ttu-id="d3046-142">String</span><span class="sxs-lookup"><span data-stu-id="d3046-142">String</span></span>|<span data-ttu-id="d3046-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d3046-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d3046-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3046-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3046-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d3046-145">displayName</span></span>|<span data-ttu-id="d3046-146">String</span><span class="sxs-lookup"><span data-stu-id="d3046-146">String</span></span>|<span data-ttu-id="d3046-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d3046-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d3046-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3046-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3046-149">version</span><span class="sxs-lookup"><span data-stu-id="d3046-149">version</span></span>|<span data-ttu-id="d3046-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d3046-150">Int32</span></span>|<span data-ttu-id="d3046-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d3046-151">Version of the device configuration.</span></span> <span data-ttu-id="d3046-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3046-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d3046-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="d3046-153">payloadName</span></span>|<span data-ttu-id="d3046-154">String</span><span class="sxs-lookup"><span data-stu-id="d3046-154">String</span></span>|<span data-ttu-id="d3046-155">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="d3046-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="d3046-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="d3046-156">payloadFileName</span></span>|<span data-ttu-id="d3046-157">String</span><span class="sxs-lookup"><span data-stu-id="d3046-157">String</span></span>|<span data-ttu-id="d3046-158">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="d3046-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="d3046-159">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="d3046-159">XML</span></span>|
|<span data-ttu-id="d3046-160">payload</span><span class="sxs-lookup"><span data-stu-id="d3046-160">Notification payload</span></span>|<span data-ttu-id="d3046-161">Binary</span><span class="sxs-lookup"><span data-stu-id="d3046-161">Binary</span></span>|<span data-ttu-id="d3046-162">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="d3046-162">Payload.</span></span> <span data-ttu-id="d3046-163">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="d3046-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="d3046-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3046-164">Response</span></span>
<span data-ttu-id="d3046-165">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d3046-165">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_deviceconfig_ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3046-166">Пример</span><span class="sxs-lookup"><span data-stu-id="d3046-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3046-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3046-167">Request</span></span>
<span data-ttu-id="d3046-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3046-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 343

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="d3046-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3046-169">Response</span></span>
<span data-ttu-id="d3046-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d3046-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```



