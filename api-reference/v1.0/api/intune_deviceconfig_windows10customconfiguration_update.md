# <a name="update-windows10customconfiguration"></a><span data-ttu-id="319bb-101">Обновление объекта windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="319bb-101">Update windows10CustomConfiguration</span></span>

> <span data-ttu-id="319bb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="319bb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="319bb-103">Обновление свойств объекта [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="319bb-103">Update the properties of a [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="319bb-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="319bb-104">Prerequisites</span></span>
<span data-ttu-id="319bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="319bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="319bb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="319bb-107">Permission type</span></span>|<span data-ttu-id="319bb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="319bb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="319bb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="319bb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="319bb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="319bb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="319bb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="319bb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="319bb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="319bb-112">Not supported.</span></span>|
|<span data-ttu-id="319bb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="319bb-113">Application</span></span>|<span data-ttu-id="319bb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="319bb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="319bb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="319bb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="319bb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="319bb-116">Request headers</span></span>
|<span data-ttu-id="319bb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="319bb-117">Header</span></span>|<span data-ttu-id="319bb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="319bb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="319bb-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="319bb-119">Authorization</span></span>|<span data-ttu-id="319bb-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="319bb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="319bb-121">Принять</span><span class="sxs-lookup"><span data-stu-id="319bb-121">Accept</span></span>|<span data-ttu-id="319bb-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="319bb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="319bb-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="319bb-123">Request body</span></span>
<span data-ttu-id="319bb-124">В теле запроса добавьте представление объекта [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="319bb-124">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="319bb-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="319bb-125">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md).</span></span>

|<span data-ttu-id="319bb-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="319bb-126">Property</span></span>|<span data-ttu-id="319bb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="319bb-127">Type</span></span>|<span data-ttu-id="319bb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="319bb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="319bb-129">ИД</span><span class="sxs-lookup"><span data-stu-id="319bb-129">id</span></span>|<span data-ttu-id="319bb-130">Строка</span><span class="sxs-lookup"><span data-stu-id="319bb-130">String</span></span>|<span data-ttu-id="319bb-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="319bb-131">Key of the entity.</span></span> <span data-ttu-id="319bb-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="319bb-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319bb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="319bb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="319bb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="319bb-134">DateTimeOffset</span></span>|<span data-ttu-id="319bb-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="319bb-135">DateTime the object was last modified.</span></span> <span data-ttu-id="319bb-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="319bb-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319bb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="319bb-137">createdDateTime</span></span>|<span data-ttu-id="319bb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="319bb-138">DateTimeOffset</span></span>|<span data-ttu-id="319bb-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="319bb-139">DateTime the object was created.</span></span> <span data-ttu-id="319bb-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="319bb-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319bb-141">описание</span><span class="sxs-lookup"><span data-stu-id="319bb-141">description</span></span>|<span data-ttu-id="319bb-142">Строка</span><span class="sxs-lookup"><span data-stu-id="319bb-142">String</span></span>|<span data-ttu-id="319bb-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="319bb-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="319bb-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="319bb-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319bb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="319bb-145">displayName</span></span>|<span data-ttu-id="319bb-146">Строка</span><span class="sxs-lookup"><span data-stu-id="319bb-146">String</span></span>|<span data-ttu-id="319bb-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="319bb-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="319bb-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="319bb-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319bb-149">версия</span><span class="sxs-lookup"><span data-stu-id="319bb-149">version</span></span>|<span data-ttu-id="319bb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="319bb-150">Int32</span></span>|<span data-ttu-id="319bb-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="319bb-151">Version of the device configuration.</span></span> <span data-ttu-id="319bb-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="319bb-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="319bb-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="319bb-153">omaSettings</span></span>|<span data-ttu-id="319bb-154">Коллекция [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="319bb-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="319bb-155">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="319bb-155">OMA settings.</span></span> <span data-ttu-id="319bb-156">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="319bb-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="319bb-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="319bb-157">Response</span></span>
<span data-ttu-id="319bb-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="319bb-158">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="319bb-159">Пример</span><span class="sxs-lookup"><span data-stu-id="319bb-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="319bb-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="319bb-160">Request</span></span>
<span data-ttu-id="319bb-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="319bb-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 401

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="319bb-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="319bb-162">Response</span></span>
<span data-ttu-id="319bb-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="319bb-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```








