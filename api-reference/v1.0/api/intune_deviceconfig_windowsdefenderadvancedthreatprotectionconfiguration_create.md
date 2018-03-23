# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="38fba-101">Создание объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="38fba-101">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="38fba-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="38fba-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38fba-103">Создание объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38fba-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38fba-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="38fba-104">Prerequisites</span></span>
<span data-ttu-id="38fba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="38fba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="38fba-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38fba-107">Permission type</span></span>|<span data-ttu-id="38fba-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38fba-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38fba-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38fba-109">Delegated (work or school account)</span></span>|<span data-ttu-id="38fba-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38fba-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38fba-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38fba-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38fba-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38fba-112">Not supported.</span></span>|
|<span data-ttu-id="38fba-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38fba-113">Application</span></span>|<span data-ttu-id="38fba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38fba-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38fba-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38fba-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="38fba-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38fba-116">Request headers</span></span>
|<span data-ttu-id="38fba-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38fba-117">Header</span></span>|<span data-ttu-id="38fba-118">Значение</span><span class="sxs-lookup"><span data-stu-id="38fba-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38fba-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="38fba-119">Authorization</span></span>|<span data-ttu-id="38fba-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38fba-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="38fba-121">Accept</span><span class="sxs-lookup"><span data-stu-id="38fba-121">Accept</span></span>|<span data-ttu-id="38fba-122">application/json</span><span class="sxs-lookup"><span data-stu-id="38fba-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38fba-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38fba-123">Request body</span></span>
<span data-ttu-id="38fba-124">В теле запроса добавьте представление объекта windowsDefenderAdvancedThreatProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38fba-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="38fba-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="38fba-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="38fba-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="38fba-126">Property</span></span>|<span data-ttu-id="38fba-127">Тип</span><span class="sxs-lookup"><span data-stu-id="38fba-127">Type</span></span>|<span data-ttu-id="38fba-128">Описание</span><span class="sxs-lookup"><span data-stu-id="38fba-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38fba-129">id</span><span class="sxs-lookup"><span data-stu-id="38fba-129">id</span></span>|<span data-ttu-id="38fba-130">String</span><span class="sxs-lookup"><span data-stu-id="38fba-130">String</span></span>|<span data-ttu-id="38fba-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="38fba-131">Key of the setting.</span></span> <span data-ttu-id="38fba-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38fba-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38fba-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38fba-133">lastModifiedDateTime</span></span>|<span data-ttu-id="38fba-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38fba-134">DateTimeOffset</span></span>|<span data-ttu-id="38fba-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="38fba-135">DateTime the object was last modified.</span></span> <span data-ttu-id="38fba-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38fba-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38fba-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38fba-137">createdDateTime</span></span>|<span data-ttu-id="38fba-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38fba-138">DateTimeOffset</span></span>|<span data-ttu-id="38fba-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="38fba-139">DateTime the object was created.</span></span> <span data-ttu-id="38fba-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38fba-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38fba-141">description</span><span class="sxs-lookup"><span data-stu-id="38fba-141">description</span></span>|<span data-ttu-id="38fba-142">String</span><span class="sxs-lookup"><span data-stu-id="38fba-142">String</span></span>|<span data-ttu-id="38fba-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="38fba-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="38fba-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38fba-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38fba-145">displayName</span><span class="sxs-lookup"><span data-stu-id="38fba-145">displayName</span></span>|<span data-ttu-id="38fba-146">String</span><span class="sxs-lookup"><span data-stu-id="38fba-146">String</span></span>|<span data-ttu-id="38fba-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="38fba-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="38fba-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38fba-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38fba-149">version</span><span class="sxs-lookup"><span data-stu-id="38fba-149">version</span></span>|<span data-ttu-id="38fba-150">Int32</span><span class="sxs-lookup"><span data-stu-id="38fba-150">Int32</span></span>|<span data-ttu-id="38fba-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="38fba-151">Version of the device configuration.</span></span> <span data-ttu-id="38fba-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38fba-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38fba-153">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="38fba-153">allowSampleSharing</span></span>|<span data-ttu-id="38fba-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="38fba-154">Boolean</span></span>|<span data-ttu-id="38fba-155">Правило "Разрешить общий доступ к выборкам" службы Advanced Threat Protection в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="38fba-155">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="38fba-156">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="38fba-156">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="38fba-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="38fba-157">Boolean</span></span>|<span data-ttu-id="38fba-158">Увеличение частоты создания отчетов о телеметрии службой Advanced Threat Protection в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="38fba-158">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="38fba-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="38fba-159">Response</span></span>
<span data-ttu-id="38fba-160">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="38fba-160">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38fba-161">Пример</span><span class="sxs-lookup"><span data-stu-id="38fba-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="38fba-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="38fba-162">Request</span></span>
<span data-ttu-id="38fba-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38fba-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="38fba-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="38fba-164">Response</span></span>
<span data-ttu-id="38fba-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="38fba-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



