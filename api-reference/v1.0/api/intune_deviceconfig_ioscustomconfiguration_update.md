# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="dffbd-101">Обновление объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="dffbd-101">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="dffbd-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dffbd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dffbd-103">Обновление свойств объекта [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dffbd-103">Update the properties of a [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dffbd-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dffbd-104">Prerequisites</span></span>
<span data-ttu-id="dffbd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dffbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dffbd-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dffbd-107">Permission type</span></span>|<span data-ttu-id="dffbd-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dffbd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dffbd-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dffbd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dffbd-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dffbd-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dffbd-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dffbd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dffbd-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dffbd-112">Not supported.</span></span>|
|<span data-ttu-id="dffbd-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dffbd-113">Application</span></span>|<span data-ttu-id="dffbd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dffbd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dffbd-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dffbd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dffbd-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dffbd-116">Request headers</span></span>
|<span data-ttu-id="dffbd-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dffbd-117">Header</span></span>|<span data-ttu-id="dffbd-118">Значение</span><span class="sxs-lookup"><span data-stu-id="dffbd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dffbd-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dffbd-119">Authorization</span></span>|<span data-ttu-id="dffbd-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="dffbd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dffbd-121">Принять</span><span class="sxs-lookup"><span data-stu-id="dffbd-121">Accept</span></span>|<span data-ttu-id="dffbd-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="dffbd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dffbd-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dffbd-123">Request body</span></span>
<span data-ttu-id="dffbd-124">В теле запроса добавьте представление объекта [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dffbd-124">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="dffbd-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dffbd-125">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="dffbd-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="dffbd-126">Property</span></span>|<span data-ttu-id="dffbd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="dffbd-127">Type</span></span>|<span data-ttu-id="dffbd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="dffbd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dffbd-129">ИД</span><span class="sxs-lookup"><span data-stu-id="dffbd-129">id</span></span>|<span data-ttu-id="dffbd-130">Строка</span><span class="sxs-lookup"><span data-stu-id="dffbd-130">String</span></span>|<span data-ttu-id="dffbd-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dffbd-131">Key of the entity.</span></span> <span data-ttu-id="dffbd-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dffbd-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dffbd-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dffbd-133">lastModifiedDateTime</span></span>|<span data-ttu-id="dffbd-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dffbd-134">DateTimeOffset</span></span>|<span data-ttu-id="dffbd-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dffbd-135">DateTime the object was last modified.</span></span> <span data-ttu-id="dffbd-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dffbd-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dffbd-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dffbd-137">createdDateTime</span></span>|<span data-ttu-id="dffbd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dffbd-138">DateTimeOffset</span></span>|<span data-ttu-id="dffbd-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="dffbd-139">DateTime the object was created.</span></span> <span data-ttu-id="dffbd-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dffbd-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dffbd-141">описание</span><span class="sxs-lookup"><span data-stu-id="dffbd-141">description</span></span>|<span data-ttu-id="dffbd-142">Строка</span><span class="sxs-lookup"><span data-stu-id="dffbd-142">String</span></span>|<span data-ttu-id="dffbd-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dffbd-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dffbd-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dffbd-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dffbd-145">displayName</span><span class="sxs-lookup"><span data-stu-id="dffbd-145">displayName</span></span>|<span data-ttu-id="dffbd-146">Строка</span><span class="sxs-lookup"><span data-stu-id="dffbd-146">String</span></span>|<span data-ttu-id="dffbd-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dffbd-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dffbd-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dffbd-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dffbd-149">версия</span><span class="sxs-lookup"><span data-stu-id="dffbd-149">version</span></span>|<span data-ttu-id="dffbd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="dffbd-150">Int32</span></span>|<span data-ttu-id="dffbd-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dffbd-151">Version of the device configuration.</span></span> <span data-ttu-id="dffbd-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dffbd-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dffbd-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="dffbd-153">payloadName</span></span>|<span data-ttu-id="dffbd-154">Строка</span><span class="sxs-lookup"><span data-stu-id="dffbd-154">String</span></span>|<span data-ttu-id="dffbd-155">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="dffbd-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="dffbd-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="dffbd-156">payloadFileName</span></span>|<span data-ttu-id="dffbd-157">Строка</span><span class="sxs-lookup"><span data-stu-id="dffbd-157">String</span></span>|<span data-ttu-id="dffbd-158">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="dffbd-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="dffbd-159">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="dffbd-159">\*.xml).</span></span>|
|<span data-ttu-id="dffbd-160">payload</span><span class="sxs-lookup"><span data-stu-id="dffbd-160">payload</span></span>|<span data-ttu-id="dffbd-161">Двоичный</span><span class="sxs-lookup"><span data-stu-id="dffbd-161">Binary</span></span>|<span data-ttu-id="dffbd-162">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="dffbd-162">Payload.</span></span> <span data-ttu-id="dffbd-163">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="dffbd-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="dffbd-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="dffbd-164">Response</span></span>
<span data-ttu-id="dffbd-165">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dffbd-165">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dffbd-166">Пример</span><span class="sxs-lookup"><span data-stu-id="dffbd-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="dffbd-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="dffbd-167">Request</span></span>
<span data-ttu-id="dffbd-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dffbd-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dffbd-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="dffbd-169">Response</span></span>
<span data-ttu-id="dffbd-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dffbd-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








