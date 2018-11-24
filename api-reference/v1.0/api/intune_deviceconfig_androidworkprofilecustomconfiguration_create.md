# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="b72ab-101">Создание androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="b72ab-101">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="b72ab-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b72ab-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b72ab-103">Создание нового объекта [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b72ab-103">Create a new [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b72ab-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b72ab-104">Prerequisites</span></span>
<span data-ttu-id="b72ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b72ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b72ab-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b72ab-107">Permission type</span></span>|<span data-ttu-id="b72ab-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b72ab-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b72ab-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b72ab-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b72ab-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b72ab-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b72ab-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b72ab-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b72ab-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b72ab-112">Not supported.</span></span>|
|<span data-ttu-id="b72ab-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b72ab-113">Application</span></span>|<span data-ttu-id="b72ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b72ab-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b72ab-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b72ab-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b72ab-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b72ab-116">Request headers</span></span>
|<span data-ttu-id="b72ab-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b72ab-117">Header</span></span>|<span data-ttu-id="b72ab-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b72ab-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b72ab-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b72ab-119">Authorization</span></span>|<span data-ttu-id="b72ab-120">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b72ab-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b72ab-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b72ab-121">Accept</span></span>|<span data-ttu-id="b72ab-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b72ab-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b72ab-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b72ab-123">Request body</span></span>
<span data-ttu-id="b72ab-124">В тексте запроса укажите представление JSON для объекта androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b72ab-124">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="b72ab-125">В следующей таблице показаны свойства, которые необходимы для создания androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b72ab-125">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="b72ab-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b72ab-126">Property</span></span>|<span data-ttu-id="b72ab-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b72ab-127">Type</span></span>|<span data-ttu-id="b72ab-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b72ab-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b72ab-129">id</span><span class="sxs-lookup"><span data-stu-id="b72ab-129">id</span></span>|<span data-ttu-id="b72ab-130">String</span><span class="sxs-lookup"><span data-stu-id="b72ab-130">String</span></span>|<span data-ttu-id="b72ab-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b72ab-131">Key of the entity.</span></span> <span data-ttu-id="b72ab-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b72ab-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b72ab-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b72ab-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b72ab-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b72ab-134">DateTimeOffset</span></span>|<span data-ttu-id="b72ab-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b72ab-135">DateTime the object was last modified.</span></span> <span data-ttu-id="b72ab-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b72ab-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b72ab-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b72ab-137">createdDateTime</span></span>|<span data-ttu-id="b72ab-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b72ab-138">DateTimeOffset</span></span>|<span data-ttu-id="b72ab-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b72ab-139">DateTime the object was created.</span></span> <span data-ttu-id="b72ab-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b72ab-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b72ab-141">описание</span><span class="sxs-lookup"><span data-stu-id="b72ab-141">description</span></span>|<span data-ttu-id="b72ab-142">String</span><span class="sxs-lookup"><span data-stu-id="b72ab-142">String</span></span>|<span data-ttu-id="b72ab-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b72ab-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b72ab-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b72ab-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b72ab-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b72ab-145">displayName</span></span>|<span data-ttu-id="b72ab-146">String</span><span class="sxs-lookup"><span data-stu-id="b72ab-146">String</span></span>|<span data-ttu-id="b72ab-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b72ab-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b72ab-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b72ab-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b72ab-149">version</span><span class="sxs-lookup"><span data-stu-id="b72ab-149">version</span></span>|<span data-ttu-id="b72ab-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b72ab-150">Int32</span></span>|<span data-ttu-id="b72ab-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b72ab-151">Version of the device configuration.</span></span> <span data-ttu-id="b72ab-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b72ab-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b72ab-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="b72ab-153">omaSettings</span></span>|<span data-ttu-id="b72ab-154">Коллекция [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b72ab-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="b72ab-155">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="b72ab-155">OMA settings.</span></span> <span data-ttu-id="b72ab-156">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b72ab-156">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b72ab-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="b72ab-157">Response</span></span>
<span data-ttu-id="b72ab-158">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b72ab-158">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b72ab-159">Пример</span><span class="sxs-lookup"><span data-stu-id="b72ab-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="b72ab-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="b72ab-160">Request</span></span>
<span data-ttu-id="b72ab-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b72ab-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="b72ab-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="b72ab-162">Response</span></span>
<span data-ttu-id="b72ab-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b72ab-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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



