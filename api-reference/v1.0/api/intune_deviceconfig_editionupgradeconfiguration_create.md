# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="f4d74-101">Создание объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4d74-101">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="f4d74-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f4d74-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4d74-103">Создание объекта [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d74-103">Create a new [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4d74-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f4d74-104">Prerequisites</span></span>
<span data-ttu-id="f4d74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4d74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f4d74-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4d74-107">Permission type</span></span>|<span data-ttu-id="f4d74-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4d74-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4d74-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4d74-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f4d74-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d74-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4d74-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4d74-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4d74-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d74-112">Not supported.</span></span>|
|<span data-ttu-id="f4d74-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4d74-113">Application</span></span>|<span data-ttu-id="f4d74-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d74-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4d74-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4d74-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f4d74-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4d74-116">Request headers</span></span>
|<span data-ttu-id="f4d74-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4d74-117">Header</span></span>|<span data-ttu-id="f4d74-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f4d74-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4d74-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4d74-119">Authorization</span></span>|<span data-ttu-id="f4d74-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4d74-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4d74-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f4d74-121">Accept</span></span>|<span data-ttu-id="f4d74-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f4d74-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4d74-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4d74-123">Request body</span></span>
<span data-ttu-id="f4d74-124">В теле запроса добавьте представление объекта editionUpgradeConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4d74-124">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="f4d74-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f4d74-125">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="f4d74-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4d74-126">Property</span></span>|<span data-ttu-id="f4d74-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f4d74-127">Type</span></span>|<span data-ttu-id="f4d74-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f4d74-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4d74-129">id</span><span class="sxs-lookup"><span data-stu-id="f4d74-129">id</span></span>|<span data-ttu-id="f4d74-130">String</span><span class="sxs-lookup"><span data-stu-id="f4d74-130">String</span></span>|<span data-ttu-id="f4d74-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f4d74-131">Key of the entity.</span></span> <span data-ttu-id="f4d74-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d74-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d74-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4d74-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f4d74-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4d74-134">DateTimeOffset</span></span>|<span data-ttu-id="f4d74-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f4d74-135">DateTime the object was last modified.</span></span> <span data-ttu-id="f4d74-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d74-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d74-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4d74-137">createdDateTime</span></span>|<span data-ttu-id="f4d74-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4d74-138">DateTimeOffset</span></span>|<span data-ttu-id="f4d74-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f4d74-139">DateTime the object was created.</span></span> <span data-ttu-id="f4d74-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d74-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d74-141">description</span><span class="sxs-lookup"><span data-stu-id="f4d74-141">description</span></span>|<span data-ttu-id="f4d74-142">String</span><span class="sxs-lookup"><span data-stu-id="f4d74-142">String</span></span>|<span data-ttu-id="f4d74-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4d74-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4d74-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d74-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d74-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f4d74-145">displayName</span></span>|<span data-ttu-id="f4d74-146">String</span><span class="sxs-lookup"><span data-stu-id="f4d74-146">String</span></span>|<span data-ttu-id="f4d74-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4d74-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4d74-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d74-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d74-149">version</span><span class="sxs-lookup"><span data-stu-id="f4d74-149">version</span></span>|<span data-ttu-id="f4d74-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f4d74-150">Int32</span></span>|<span data-ttu-id="f4d74-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4d74-151">Version of the device configuration.</span></span> <span data-ttu-id="f4d74-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d74-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d74-153">licenseType</span><span class="sxs-lookup"><span data-stu-id="f4d74-153">licenseType</span></span>|[<span data-ttu-id="f4d74-154">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="f4d74-154">editionUpgradeLicenseType</span></span>](../resources/intune_deviceconfig_editionupgradelicensetype.md)|<span data-ttu-id="f4d74-155">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="f4d74-155">Edition Upgrade License Type.</span></span> <span data-ttu-id="f4d74-156">Возможные значения: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="f4d74-156">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="f4d74-157">targetEdition</span><span class="sxs-lookup"><span data-stu-id="f4d74-157">targetEdition</span></span>|[<span data-ttu-id="f4d74-158">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="f4d74-158">windows10EditionType</span></span>](../resources/intune_deviceconfig_windows10editiontype.md)|<span data-ttu-id="f4d74-159">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="f4d74-159">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="f4d74-160">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="f4d74-160">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="f4d74-161">license</span><span class="sxs-lookup"><span data-stu-id="f4d74-161">license</span></span>|<span data-ttu-id="f4d74-162">String</span><span class="sxs-lookup"><span data-stu-id="f4d74-162">String</span></span>|<span data-ttu-id="f4d74-163">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="f4d74-163">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="f4d74-164">productKey</span><span class="sxs-lookup"><span data-stu-id="f4d74-164">productKey</span></span>|<span data-ttu-id="f4d74-165">String</span><span class="sxs-lookup"><span data-stu-id="f4d74-165">String</span></span>|<span data-ttu-id="f4d74-166">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="f4d74-166">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="f4d74-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d74-167">Response</span></span>
<span data-ttu-id="f4d74-168">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f4d74-168">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4d74-169">Пример</span><span class="sxs-lookup"><span data-stu-id="f4d74-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4d74-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4d74-170">Request</span></span>
<span data-ttu-id="f4d74-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4d74-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="f4d74-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4d74-172">Response</span></span>
<span data-ttu-id="f4d74-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f4d74-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```



