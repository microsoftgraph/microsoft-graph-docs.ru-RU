# <a name="create-windows10customconfiguration"></a><span data-ttu-id="2eb75-101">Создание объекта windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb75-101">Create windows10CustomConfiguration</span></span>

> <span data-ttu-id="2eb75-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2eb75-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2eb75-103">Создание объекта [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb75-103">Create a new [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2eb75-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2eb75-104">Prerequisites</span></span>
<span data-ttu-id="2eb75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2eb75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2eb75-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2eb75-107">Permission type</span></span>|<span data-ttu-id="2eb75-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2eb75-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2eb75-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2eb75-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2eb75-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb75-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2eb75-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2eb75-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2eb75-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2eb75-112">Not supported.</span></span>|
|<span data-ttu-id="2eb75-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2eb75-113">Application</span></span>|<span data-ttu-id="2eb75-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2eb75-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eb75-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2eb75-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2eb75-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2eb75-116">Request headers</span></span>
|<span data-ttu-id="2eb75-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2eb75-117">Header</span></span>|<span data-ttu-id="2eb75-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2eb75-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2eb75-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2eb75-119">Authorization</span></span>|<span data-ttu-id="2eb75-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2eb75-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2eb75-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2eb75-121">Accept</span></span>|<span data-ttu-id="2eb75-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2eb75-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eb75-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2eb75-123">Request body</span></span>
<span data-ttu-id="2eb75-124">В тексте запроса добавьте представление объекта windows10CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2eb75-124">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="2eb75-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта windows10CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2eb75-125">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="2eb75-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2eb75-126">Property</span></span>|<span data-ttu-id="2eb75-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2eb75-127">Type</span></span>|<span data-ttu-id="2eb75-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2eb75-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2eb75-129">id</span><span class="sxs-lookup"><span data-stu-id="2eb75-129">id</span></span>|<span data-ttu-id="2eb75-130">String</span><span class="sxs-lookup"><span data-stu-id="2eb75-130">String</span></span>|<span data-ttu-id="2eb75-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2eb75-131">Key of the entity.</span></span> <span data-ttu-id="2eb75-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb75-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb75-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2eb75-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2eb75-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eb75-134">DateTimeOffset</span></span>|<span data-ttu-id="2eb75-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2eb75-135">DateTime the object was last modified.</span></span> <span data-ttu-id="2eb75-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb75-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb75-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2eb75-137">createdDateTime</span></span>|<span data-ttu-id="2eb75-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eb75-138">DateTimeOffset</span></span>|<span data-ttu-id="2eb75-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2eb75-139">DateTime the object was created.</span></span> <span data-ttu-id="2eb75-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb75-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb75-141">description</span><span class="sxs-lookup"><span data-stu-id="2eb75-141">description</span></span>|<span data-ttu-id="2eb75-142">String</span><span class="sxs-lookup"><span data-stu-id="2eb75-142">String</span></span>|<span data-ttu-id="2eb75-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2eb75-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2eb75-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb75-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb75-145">displayName</span><span class="sxs-lookup"><span data-stu-id="2eb75-145">displayName</span></span>|<span data-ttu-id="2eb75-146">String</span><span class="sxs-lookup"><span data-stu-id="2eb75-146">String</span></span>|<span data-ttu-id="2eb75-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2eb75-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2eb75-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb75-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb75-149">version</span><span class="sxs-lookup"><span data-stu-id="2eb75-149">version</span></span>|<span data-ttu-id="2eb75-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2eb75-150">Int32</span></span>|<span data-ttu-id="2eb75-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2eb75-151">Version of the device configuration.</span></span> <span data-ttu-id="2eb75-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb75-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb75-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="2eb75-153">omaSettings</span></span>|<span data-ttu-id="2eb75-154">Коллекция [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2eb75-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="2eb75-155">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="2eb75-155">OMA settings.</span></span> <span data-ttu-id="2eb75-156">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="2eb75-156">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="2eb75-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="2eb75-157">Response</span></span>
<span data-ttu-id="2eb75-158">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2eb75-158">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune_deviceconfig_windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eb75-159">Пример</span><span class="sxs-lookup"><span data-stu-id="2eb75-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="2eb75-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="2eb75-160">Request</span></span>
<span data-ttu-id="2eb75-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2eb75-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="2eb75-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="2eb75-162">Response</span></span>
<span data-ttu-id="2eb75-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2eb75-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



