# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="55580-101">Создание androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="55580-101">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="55580-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="55580-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55580-103">Создание нового объекта [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55580-103">Create a new [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55580-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="55580-104">Prerequisites</span></span>
<span data-ttu-id="55580-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="55580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="55580-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55580-107">Permission type</span></span>|<span data-ttu-id="55580-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55580-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55580-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55580-109">Delegated (work or school account)</span></span>|<span data-ttu-id="55580-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55580-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55580-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55580-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55580-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55580-112">Not supported.</span></span>|
|<span data-ttu-id="55580-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55580-113">Application</span></span>|<span data-ttu-id="55580-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55580-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55580-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55580-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="55580-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55580-116">Request headers</span></span>
|<span data-ttu-id="55580-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55580-117">Header</span></span>|<span data-ttu-id="55580-118">Значение</span><span class="sxs-lookup"><span data-stu-id="55580-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55580-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55580-119">Authorization</span></span>|<span data-ttu-id="55580-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="55580-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55580-121">Принять</span><span class="sxs-lookup"><span data-stu-id="55580-121">Accept</span></span>|<span data-ttu-id="55580-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="55580-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55580-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55580-123">Request body</span></span>
<span data-ttu-id="55580-124">В тексте запроса добавьте представление объекта androidWorkProfileCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55580-124">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="55580-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="55580-125">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="55580-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="55580-126">Property</span></span>|<span data-ttu-id="55580-127">Тип</span><span class="sxs-lookup"><span data-stu-id="55580-127">Type</span></span>|<span data-ttu-id="55580-128">Описание</span><span class="sxs-lookup"><span data-stu-id="55580-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55580-129">id</span><span class="sxs-lookup"><span data-stu-id="55580-129">id</span></span>|<span data-ttu-id="55580-130">Строка</span><span class="sxs-lookup"><span data-stu-id="55580-130">String</span></span>|<span data-ttu-id="55580-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="55580-131">Key of the entity.</span></span> <span data-ttu-id="55580-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55580-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55580-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55580-133">lastModifiedDateTime</span></span>|<span data-ttu-id="55580-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55580-134">DateTimeOffset</span></span>|<span data-ttu-id="55580-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="55580-135">DateTime the object was last modified.</span></span> <span data-ttu-id="55580-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55580-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55580-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55580-137">createdDateTime</span></span>|<span data-ttu-id="55580-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55580-138">DateTimeOffset</span></span>|<span data-ttu-id="55580-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="55580-139">DateTime the object was created.</span></span> <span data-ttu-id="55580-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55580-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55580-141">описание</span><span class="sxs-lookup"><span data-stu-id="55580-141">description</span></span>|<span data-ttu-id="55580-142">Строка</span><span class="sxs-lookup"><span data-stu-id="55580-142">String</span></span>|<span data-ttu-id="55580-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="55580-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="55580-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55580-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55580-145">displayName</span><span class="sxs-lookup"><span data-stu-id="55580-145">displayName</span></span>|<span data-ttu-id="55580-146">Строка</span><span class="sxs-lookup"><span data-stu-id="55580-146">String</span></span>|<span data-ttu-id="55580-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="55580-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="55580-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55580-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55580-149">version</span><span class="sxs-lookup"><span data-stu-id="55580-149">version</span></span>|<span data-ttu-id="55580-150">Int32</span><span class="sxs-lookup"><span data-stu-id="55580-150">Int32</span></span>|<span data-ttu-id="55580-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="55580-151">Version of the device configuration.</span></span> <span data-ttu-id="55580-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55580-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55580-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="55580-153">omaSettings</span></span>|<span data-ttu-id="55580-154">Коллекция [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="55580-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="55580-155">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="55580-155">OMA settings.</span></span> <span data-ttu-id="55580-156">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="55580-156">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="55580-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="55580-157">Response</span></span>
<span data-ttu-id="55580-158">В случае успеха этот метод возвращает код отклика `201 Created` и объект [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55580-158">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55580-159">Пример</span><span class="sxs-lookup"><span data-stu-id="55580-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="55580-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="55580-160">Request</span></span>
<span data-ttu-id="55580-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55580-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 477

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="55580-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="55580-162">Response</span></span>
<span data-ttu-id="55580-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55580-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








