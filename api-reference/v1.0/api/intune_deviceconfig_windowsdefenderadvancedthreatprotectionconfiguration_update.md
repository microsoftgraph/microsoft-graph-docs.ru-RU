# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="ce327-101">Обновление объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce327-101">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="ce327-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ce327-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce327-103">Обновление свойств объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce327-103">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce327-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ce327-104">Prerequisites</span></span>
<span data-ttu-id="ce327-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce327-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce327-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce327-107">Permission type</span></span>|<span data-ttu-id="ce327-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce327-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce327-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce327-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ce327-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce327-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce327-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce327-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce327-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce327-112">Not supported.</span></span>|
|<span data-ttu-id="ce327-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce327-113">Application</span></span>|<span data-ttu-id="ce327-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce327-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce327-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce327-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ce327-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce327-116">Request headers</span></span>
|<span data-ttu-id="ce327-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce327-117">Header</span></span>|<span data-ttu-id="ce327-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ce327-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce327-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce327-119">Authorization</span></span>|<span data-ttu-id="ce327-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce327-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce327-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ce327-121">Accept</span></span>|<span data-ttu-id="ce327-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ce327-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce327-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ce327-123">Request body</span></span>
<span data-ttu-id="ce327-124">В теле запроса добавьте представление объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce327-124">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="ce327-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce327-125">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="ce327-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce327-126">Property</span></span>|<span data-ttu-id="ce327-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ce327-127">Type</span></span>|<span data-ttu-id="ce327-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ce327-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce327-129">id</span><span class="sxs-lookup"><span data-stu-id="ce327-129">id</span></span>|<span data-ttu-id="ce327-130">String</span><span class="sxs-lookup"><span data-stu-id="ce327-130">String</span></span>|<span data-ttu-id="ce327-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce327-131">Key of the entity.</span></span> <span data-ttu-id="ce327-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce327-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce327-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce327-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ce327-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce327-134">DateTimeOffset</span></span>|<span data-ttu-id="ce327-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ce327-135">DateTime the object was last modified.</span></span> <span data-ttu-id="ce327-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce327-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce327-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce327-137">createdDateTime</span></span>|<span data-ttu-id="ce327-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce327-138">DateTimeOffset</span></span>|<span data-ttu-id="ce327-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ce327-139">DateTime the object was created.</span></span> <span data-ttu-id="ce327-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce327-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce327-141">description</span><span class="sxs-lookup"><span data-stu-id="ce327-141">description</span></span>|<span data-ttu-id="ce327-142">String</span><span class="sxs-lookup"><span data-stu-id="ce327-142">String</span></span>|<span data-ttu-id="ce327-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce327-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce327-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce327-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce327-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ce327-145">displayName</span></span>|<span data-ttu-id="ce327-146">String</span><span class="sxs-lookup"><span data-stu-id="ce327-146">String</span></span>|<span data-ttu-id="ce327-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce327-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce327-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce327-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce327-149">version</span><span class="sxs-lookup"><span data-stu-id="ce327-149">version</span></span>|<span data-ttu-id="ce327-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ce327-150">Int32</span></span>|<span data-ttu-id="ce327-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce327-151">Version of the device configuration.</span></span> <span data-ttu-id="ce327-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce327-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce327-153">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="ce327-153">allowSampleSharing</span></span>|<span data-ttu-id="ce327-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce327-154">Boolean</span></span>|<span data-ttu-id="ce327-155">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="ce327-155">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="ce327-156">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="ce327-156">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="ce327-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce327-157">Boolean</span></span>|<span data-ttu-id="ce327-158">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="ce327-158">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="ce327-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce327-159">Response</span></span>
<span data-ttu-id="ce327-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ce327-160">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce327-161">Пример</span><span class="sxs-lookup"><span data-stu-id="ce327-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce327-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce327-162">Request</span></span>
<span data-ttu-id="ce327-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce327-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="ce327-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce327-164">Response</span></span>
<span data-ttu-id="ce327-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ce327-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```



