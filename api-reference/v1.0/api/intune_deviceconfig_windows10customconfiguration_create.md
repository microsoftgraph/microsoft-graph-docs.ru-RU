# <a name="create-windows10customconfiguration"></a><span data-ttu-id="a8e82-101">Создание объекта windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8e82-101">Create windows10CustomConfiguration</span></span>

> <span data-ttu-id="a8e82-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a8e82-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8e82-103">Создание объекта [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8e82-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8e82-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a8e82-104">Prerequisites</span></span>
<span data-ttu-id="a8e82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8e82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a8e82-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8e82-107">Permission type</span></span>|<span data-ttu-id="a8e82-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8e82-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8e82-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8e82-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a8e82-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8e82-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8e82-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8e82-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8e82-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8e82-112">Not supported.</span></span>|
|<span data-ttu-id="a8e82-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8e82-113">Application</span></span>|<span data-ttu-id="a8e82-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8e82-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8e82-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8e82-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a8e82-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8e82-116">Request headers</span></span>
|<span data-ttu-id="a8e82-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8e82-117">Header</span></span>|<span data-ttu-id="a8e82-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a8e82-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8e82-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8e82-119">Authorization</span></span>|<span data-ttu-id="a8e82-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8e82-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a8e82-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a8e82-121">Accept</span></span>|<span data-ttu-id="a8e82-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a8e82-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8e82-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8e82-123">Request body</span></span>
<span data-ttu-id="a8e82-124">В тексте запроса добавьте представление объекта windows10CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8e82-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="a8e82-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта windows10CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a8e82-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a8e82-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8e82-126">Property</span></span>|<span data-ttu-id="a8e82-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a8e82-127">Type</span></span>|<span data-ttu-id="a8e82-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a8e82-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e82-129">id</span><span class="sxs-lookup"><span data-stu-id="a8e82-129">id</span></span>|<span data-ttu-id="a8e82-130">String</span><span class="sxs-lookup"><span data-stu-id="a8e82-130">String</span></span>|<span data-ttu-id="a8e82-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a8e82-131">Key of the setting.</span></span> <span data-ttu-id="a8e82-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8e82-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e82-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e82-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a8e82-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e82-134">DateTimeOffset</span></span>|<span data-ttu-id="a8e82-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a8e82-135">DateTime the object was last modified.</span></span> <span data-ttu-id="a8e82-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8e82-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e82-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e82-137">createdDateTime</span></span>|<span data-ttu-id="a8e82-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e82-138">DateTimeOffset</span></span>|<span data-ttu-id="a8e82-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a8e82-139">DateTime the object was created.</span></span> <span data-ttu-id="a8e82-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8e82-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e82-141">description</span><span class="sxs-lookup"><span data-stu-id="a8e82-141">description</span></span>|<span data-ttu-id="a8e82-142">String</span><span class="sxs-lookup"><span data-stu-id="a8e82-142">String</span></span>|<span data-ttu-id="a8e82-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8e82-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a8e82-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8e82-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e82-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a8e82-145">displayName</span></span>|<span data-ttu-id="a8e82-146">String</span><span class="sxs-lookup"><span data-stu-id="a8e82-146">String</span></span>|<span data-ttu-id="a8e82-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8e82-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a8e82-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8e82-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e82-149">version</span><span class="sxs-lookup"><span data-stu-id="a8e82-149">version</span></span>|<span data-ttu-id="a8e82-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a8e82-150">Int32</span></span>|<span data-ttu-id="a8e82-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8e82-151">Version of the device configuration.</span></span> <span data-ttu-id="a8e82-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8e82-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e82-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="a8e82-153">omaSettings</span></span>|<span data-ttu-id="a8e82-154">Коллекция [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a8e82-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="a8e82-155">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="a8e82-155">OMA settings.</span></span> <span data-ttu-id="a8e82-156">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="a8e82-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a8e82-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8e82-157">Response</span></span>
<span data-ttu-id="a8e82-158">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a8e82-158">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8e82-159">Пример</span><span class="sxs-lookup"><span data-stu-id="a8e82-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8e82-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8e82-160">Request</span></span>
<span data-ttu-id="a8e82-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8e82-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 468

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="a8e82-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8e82-162">Response</span></span>
<span data-ttu-id="a8e82-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a8e82-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



