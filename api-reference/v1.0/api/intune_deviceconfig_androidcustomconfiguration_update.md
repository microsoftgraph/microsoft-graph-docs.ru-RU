# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="4bfd6-101">Update androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="4bfd6-101">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="4bfd6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bfd6-103">Обновление свойств объекта [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bfd6-103">Update the properties of a [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4bfd6-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4bfd6-104">Prerequisites</span></span>
<span data-ttu-id="4bfd6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4bfd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4bfd6-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bfd6-107">Permission type</span></span>|<span data-ttu-id="4bfd6-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bfd6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bfd6-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bfd6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4bfd6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bfd6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4bfd6-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bfd6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bfd6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-112">Not supported.</span></span>|
|<span data-ttu-id="4bfd6-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bfd6-113">Application</span></span>|<span data-ttu-id="4bfd6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bfd6-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bfd6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4bfd6-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4bfd6-116">Request headers</span></span>
|<span data-ttu-id="4bfd6-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bfd6-117">Header</span></span>|<span data-ttu-id="4bfd6-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4bfd6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bfd6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bfd6-119">Authorization</span></span>|<span data-ttu-id="4bfd6-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bfd6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4bfd6-121">Accept</span></span>|<span data-ttu-id="4bfd6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4bfd6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bfd6-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4bfd6-123">Request body</span></span>
<span data-ttu-id="4bfd6-124">В теле запроса добавьте представление объекта [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-124">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="4bfd6-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bfd6-125">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="4bfd6-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bfd6-126">Property</span></span>|<span data-ttu-id="4bfd6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4bfd6-127">Type</span></span>|<span data-ttu-id="4bfd6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4bfd6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bfd6-129">id</span><span class="sxs-lookup"><span data-stu-id="4bfd6-129">id</span></span>|<span data-ttu-id="4bfd6-130">String</span><span class="sxs-lookup"><span data-stu-id="4bfd6-130">String</span></span>|<span data-ttu-id="4bfd6-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-131">Key of the entity.</span></span> <span data-ttu-id="4bfd6-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bfd6-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bfd6-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bfd6-133">lastModifiedDateTime</span></span>|<span data-ttu-id="4bfd6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bfd6-134">DateTimeOffset</span></span>|<span data-ttu-id="4bfd6-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-135">DateTime the object was last modified.</span></span> <span data-ttu-id="4bfd6-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bfd6-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bfd6-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4bfd6-137">createdDateTime</span></span>|<span data-ttu-id="4bfd6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bfd6-138">DateTimeOffset</span></span>|<span data-ttu-id="4bfd6-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-139">DateTime the object was created.</span></span> <span data-ttu-id="4bfd6-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bfd6-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bfd6-141">description</span><span class="sxs-lookup"><span data-stu-id="4bfd6-141">description</span></span>|<span data-ttu-id="4bfd6-142">String</span><span class="sxs-lookup"><span data-stu-id="4bfd6-142">String</span></span>|<span data-ttu-id="4bfd6-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4bfd6-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bfd6-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bfd6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4bfd6-145">displayName</span></span>|<span data-ttu-id="4bfd6-146">String</span><span class="sxs-lookup"><span data-stu-id="4bfd6-146">String</span></span>|<span data-ttu-id="4bfd6-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4bfd6-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bfd6-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bfd6-149">version</span><span class="sxs-lookup"><span data-stu-id="4bfd6-149">version</span></span>|<span data-ttu-id="4bfd6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4bfd6-150">Int32</span></span>|<span data-ttu-id="4bfd6-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-151">Version of the device configuration.</span></span> <span data-ttu-id="4bfd6-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bfd6-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4bfd6-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="4bfd6-153">omaSettings</span></span>|<span data-ttu-id="4bfd6-154">Коллекция [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4bfd6-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="4bfd6-155">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-155">OMA settings.</span></span> <span data-ttu-id="4bfd6-156">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4bfd6-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bfd6-157">Response</span></span>
<span data-ttu-id="4bfd6-158">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-158">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune_deviceconfig_androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bfd6-159">Пример</span><span class="sxs-lookup"><span data-stu-id="4bfd6-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="4bfd6-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bfd6-160">Request</span></span>
<span data-ttu-id="4bfd6-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="4bfd6-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bfd6-162">Response</span></span>
<span data-ttu-id="4bfd6-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4bfd6-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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



