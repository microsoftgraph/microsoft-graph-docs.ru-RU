# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="64101-101">Обновление объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="64101-101">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="64101-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="64101-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64101-103">Обновление свойств объекта [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64101-103">Update the properties of a [calendar](../resources/intune_deviceconfig_macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64101-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="64101-104">Prerequisites</span></span>
<span data-ttu-id="64101-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="64101-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="64101-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64101-107">Permission type</span></span>|<span data-ttu-id="64101-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64101-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64101-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64101-109">Delegated (work or school account)</span></span>|<span data-ttu-id="64101-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64101-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64101-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64101-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64101-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64101-112">Not supported.</span></span>|
|<span data-ttu-id="64101-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64101-113">Application</span></span>|<span data-ttu-id="64101-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64101-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64101-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64101-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="64101-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64101-116">Request headers</span></span>
|<span data-ttu-id="64101-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64101-117">Header</span></span>|<span data-ttu-id="64101-118">Значение</span><span class="sxs-lookup"><span data-stu-id="64101-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64101-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="64101-119">Authorization</span></span>|<span data-ttu-id="64101-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64101-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="64101-121">Accept</span><span class="sxs-lookup"><span data-stu-id="64101-121">Accept</span></span>|<span data-ttu-id="64101-122">application/json</span><span class="sxs-lookup"><span data-stu-id="64101-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64101-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64101-123">Request body</span></span>
<span data-ttu-id="64101-124">В теле запроса добавьте представление объекта [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64101-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="64101-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64101-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="64101-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="64101-126">Property</span></span>|<span data-ttu-id="64101-127">Тип</span><span class="sxs-lookup"><span data-stu-id="64101-127">Type</span></span>|<span data-ttu-id="64101-128">Описание</span><span class="sxs-lookup"><span data-stu-id="64101-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64101-129">id</span><span class="sxs-lookup"><span data-stu-id="64101-129">id</span></span>|<span data-ttu-id="64101-130">String</span><span class="sxs-lookup"><span data-stu-id="64101-130">String</span></span>|<span data-ttu-id="64101-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="64101-131">Key of the setting.</span></span> <span data-ttu-id="64101-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64101-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64101-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64101-133">lastModifiedDateTime</span></span>|<span data-ttu-id="64101-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64101-134">DateTimeOffset</span></span>|<span data-ttu-id="64101-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="64101-135">DateTime the object was last modified.</span></span> <span data-ttu-id="64101-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64101-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64101-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64101-137">createdDateTime</span></span>|<span data-ttu-id="64101-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64101-138">DateTimeOffset</span></span>|<span data-ttu-id="64101-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="64101-139">DateTime the object was created.</span></span> <span data-ttu-id="64101-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64101-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64101-141">description</span><span class="sxs-lookup"><span data-stu-id="64101-141">description</span></span>|<span data-ttu-id="64101-142">String</span><span class="sxs-lookup"><span data-stu-id="64101-142">String</span></span>|<span data-ttu-id="64101-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="64101-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64101-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64101-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64101-145">displayName</span><span class="sxs-lookup"><span data-stu-id="64101-145">displayName</span></span>|<span data-ttu-id="64101-146">String</span><span class="sxs-lookup"><span data-stu-id="64101-146">String</span></span>|<span data-ttu-id="64101-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="64101-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64101-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64101-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64101-149">version</span><span class="sxs-lookup"><span data-stu-id="64101-149">version</span></span>|<span data-ttu-id="64101-150">Int32</span><span class="sxs-lookup"><span data-stu-id="64101-150">Int32</span></span>|<span data-ttu-id="64101-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="64101-151">Version of the device configuration.</span></span> <span data-ttu-id="64101-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64101-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64101-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="64101-153">payloadName</span></span>|<span data-ttu-id="64101-154">String</span><span class="sxs-lookup"><span data-stu-id="64101-154">String</span></span>|<span data-ttu-id="64101-155">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="64101-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="64101-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="64101-156">payloadFileName</span></span>|<span data-ttu-id="64101-157">String</span><span class="sxs-lookup"><span data-stu-id="64101-157">String</span></span>|<span data-ttu-id="64101-158">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="64101-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="64101-159">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="64101-159">XML</span></span>|
|<span data-ttu-id="64101-160">payload</span><span class="sxs-lookup"><span data-stu-id="64101-160">Notification payload</span></span>|<span data-ttu-id="64101-161">Binary</span><span class="sxs-lookup"><span data-stu-id="64101-161">Binary</span></span>|<span data-ttu-id="64101-162">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="64101-162">Payload.</span></span> <span data-ttu-id="64101-163">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="64101-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="64101-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="64101-164">Response</span></span>
<span data-ttu-id="64101-165">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64101-165">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64101-166">Пример</span><span class="sxs-lookup"><span data-stu-id="64101-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="64101-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="64101-167">Request</span></span>
<span data-ttu-id="64101-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64101-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 282

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="64101-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="64101-169">Response</span></span>
<span data-ttu-id="64101-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="64101-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
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



