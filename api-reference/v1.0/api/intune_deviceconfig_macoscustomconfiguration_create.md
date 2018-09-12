# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="1dbea-101">Создание объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="1dbea-101">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="1dbea-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1dbea-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1dbea-103">Создание объекта [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbea-103">Create a new [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1dbea-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1dbea-104">Prerequisites</span></span>
<span data-ttu-id="1dbea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1dbea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1dbea-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dbea-107">Permission type</span></span>|<span data-ttu-id="1dbea-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dbea-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dbea-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dbea-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1dbea-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dbea-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1dbea-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dbea-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dbea-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dbea-112">Not supported.</span></span>|
|<span data-ttu-id="1dbea-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dbea-113">Application</span></span>|<span data-ttu-id="1dbea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dbea-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dbea-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dbea-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1dbea-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dbea-116">Request headers</span></span>
|<span data-ttu-id="1dbea-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1dbea-117">Header</span></span>|<span data-ttu-id="1dbea-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1dbea-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dbea-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dbea-119">Authorization</span></span>|<span data-ttu-id="1dbea-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="1dbea-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dbea-121">Принять</span><span class="sxs-lookup"><span data-stu-id="1dbea-121">Accept</span></span>|<span data-ttu-id="1dbea-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1dbea-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dbea-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1dbea-123">Request body</span></span>
<span data-ttu-id="1dbea-124">В теле запроса добавьте представление объекта macOSCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1dbea-124">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="1dbea-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1dbea-125">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="1dbea-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="1dbea-126">Property</span></span>|<span data-ttu-id="1dbea-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1dbea-127">Type</span></span>|<span data-ttu-id="1dbea-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1dbea-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dbea-129">id</span><span class="sxs-lookup"><span data-stu-id="1dbea-129">id</span></span>|<span data-ttu-id="1dbea-130">Строка</span><span class="sxs-lookup"><span data-stu-id="1dbea-130">String</span></span>|<span data-ttu-id="1dbea-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1dbea-131">Key of the entity.</span></span> <span data-ttu-id="1dbea-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbea-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dbea-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dbea-133">lastModifiedDateTime</span></span>|<span data-ttu-id="1dbea-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dbea-134">DateTimeOffset</span></span>|<span data-ttu-id="1dbea-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1dbea-135">DateTime the object was last modified.</span></span> <span data-ttu-id="1dbea-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbea-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dbea-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1dbea-137">createdDateTime</span></span>|<span data-ttu-id="1dbea-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dbea-138">DateTimeOffset</span></span>|<span data-ttu-id="1dbea-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1dbea-139">DateTime the object was created.</span></span> <span data-ttu-id="1dbea-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbea-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dbea-141">description</span><span class="sxs-lookup"><span data-stu-id="1dbea-141">description</span></span>|<span data-ttu-id="1dbea-142">Строка</span><span class="sxs-lookup"><span data-stu-id="1dbea-142">String</span></span>|<span data-ttu-id="1dbea-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1dbea-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1dbea-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbea-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dbea-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1dbea-145">displayName</span></span>|<span data-ttu-id="1dbea-146">Строка</span><span class="sxs-lookup"><span data-stu-id="1dbea-146">String</span></span>|<span data-ttu-id="1dbea-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1dbea-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1dbea-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbea-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dbea-149">version</span><span class="sxs-lookup"><span data-stu-id="1dbea-149">version</span></span>|<span data-ttu-id="1dbea-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1dbea-150">Int32</span></span>|<span data-ttu-id="1dbea-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1dbea-151">Version of the device configuration.</span></span> <span data-ttu-id="1dbea-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1dbea-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dbea-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="1dbea-153">payloadName</span></span>|<span data-ttu-id="1dbea-154">String (строка)</span><span class="sxs-lookup"><span data-stu-id="1dbea-154">String</span></span>|<span data-ttu-id="1dbea-155">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="1dbea-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="1dbea-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="1dbea-156">payloadFileName</span></span>|<span data-ttu-id="1dbea-157">String (строка)</span><span class="sxs-lookup"><span data-stu-id="1dbea-157">String</span></span>|<span data-ttu-id="1dbea-158">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="1dbea-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="1dbea-159">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="1dbea-159">\*.xml).</span></span>|
|<span data-ttu-id="1dbea-160">payload</span><span class="sxs-lookup"><span data-stu-id="1dbea-160">payload</span></span>|<span data-ttu-id="1dbea-161">Binary</span><span class="sxs-lookup"><span data-stu-id="1dbea-161">Binary</span></span>|<span data-ttu-id="1dbea-162">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="1dbea-162">Payload.</span></span> <span data-ttu-id="1dbea-163">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="1dbea-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="1dbea-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dbea-164">Response</span></span>
<span data-ttu-id="1dbea-165">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1dbea-165">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dbea-166">Пример</span><span class="sxs-lookup"><span data-stu-id="1dbea-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="1dbea-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dbea-167">Request</span></span>
<span data-ttu-id="1dbea-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dbea-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="1dbea-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="1dbea-169">Response</span></span>
<span data-ttu-id="1dbea-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1dbea-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








