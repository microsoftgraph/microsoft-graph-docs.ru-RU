# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="eb9a1-101">Обновление объекта windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="eb9a1-101">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="eb9a1-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb9a1-103">Обновление свойств объекта [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb9a1-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb9a1-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eb9a1-104">Prerequisites</span></span>
<span data-ttu-id="eb9a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb9a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eb9a1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb9a1-107">Permission type</span></span>|<span data-ttu-id="eb9a1-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb9a1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb9a1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb9a1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="eb9a1-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb9a1-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb9a1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb9a1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb9a1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-112">Not supported.</span></span>|
|<span data-ttu-id="eb9a1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb9a1-113">Application</span></span>|<span data-ttu-id="eb9a1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb9a1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb9a1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="eb9a1-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb9a1-116">Request headers</span></span>
|<span data-ttu-id="eb9a1-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb9a1-117">Header</span></span>|<span data-ttu-id="eb9a1-118">Значение</span><span class="sxs-lookup"><span data-stu-id="eb9a1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb9a1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb9a1-119">Authorization</span></span>|<span data-ttu-id="eb9a1-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eb9a1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="eb9a1-121">Accept</span></span>|<span data-ttu-id="eb9a1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="eb9a1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb9a1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb9a1-123">Request body</span></span>
<span data-ttu-id="eb9a1-124">В теле запроса добавьте представление объекта [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-124">In the request body, supply a JSON representation of [Attachment](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="eb9a1-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb9a1-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="eb9a1-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb9a1-126">Property</span></span>|<span data-ttu-id="eb9a1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="eb9a1-127">Type</span></span>|<span data-ttu-id="eb9a1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="eb9a1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb9a1-129">id</span><span class="sxs-lookup"><span data-stu-id="eb9a1-129">id</span></span>|<span data-ttu-id="eb9a1-130">String</span><span class="sxs-lookup"><span data-stu-id="eb9a1-130">String</span></span>|<span data-ttu-id="eb9a1-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-131">Key of the setting.</span></span> <span data-ttu-id="eb9a1-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb9a1-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb9a1-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb9a1-133">lastModifiedDateTime</span></span>|<span data-ttu-id="eb9a1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb9a1-134">DateTimeOffset</span></span>|<span data-ttu-id="eb9a1-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-135">DateTime the object was last modified.</span></span> <span data-ttu-id="eb9a1-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb9a1-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb9a1-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb9a1-137">createdDateTime</span></span>|<span data-ttu-id="eb9a1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb9a1-138">DateTimeOffset</span></span>|<span data-ttu-id="eb9a1-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-139">DateTime the object was created.</span></span> <span data-ttu-id="eb9a1-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb9a1-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb9a1-141">description</span><span class="sxs-lookup"><span data-stu-id="eb9a1-141">description</span></span>|<span data-ttu-id="eb9a1-142">String</span><span class="sxs-lookup"><span data-stu-id="eb9a1-142">String</span></span>|<span data-ttu-id="eb9a1-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eb9a1-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb9a1-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb9a1-145">displayName</span><span class="sxs-lookup"><span data-stu-id="eb9a1-145">displayName</span></span>|<span data-ttu-id="eb9a1-146">String</span><span class="sxs-lookup"><span data-stu-id="eb9a1-146">String</span></span>|<span data-ttu-id="eb9a1-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eb9a1-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb9a1-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb9a1-149">version</span><span class="sxs-lookup"><span data-stu-id="eb9a1-149">version</span></span>|<span data-ttu-id="eb9a1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="eb9a1-150">Int32</span></span>|<span data-ttu-id="eb9a1-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-151">Version of the device configuration.</span></span> <span data-ttu-id="eb9a1-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb9a1-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb9a1-153">launchUri</span><span class="sxs-lookup"><span data-stu-id="eb9a1-153">launchUri</span></span>|<span data-ttu-id="eb9a1-154">String</span><span class="sxs-lookup"><span data-stu-id="eb9a1-154">String</span></span>|<span data-ttu-id="eb9a1-155">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-155">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="eb9a1-156">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="eb9a1-156">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="eb9a1-157">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="eb9a1-157">configurationAccount</span></span>|<span data-ttu-id="eb9a1-158">String</span><span class="sxs-lookup"><span data-stu-id="eb9a1-158">String</span></span>|<span data-ttu-id="eb9a1-159">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-159">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="eb9a1-160">В качестве пользователя можно указать учетную запись домена (domen\polzovatel), учетную запись AAD (imya_polzovatelya@klient.com) или локальную учетную запись (имя пользователя).</span><span class="sxs-lookup"><span data-stu-id="eb9a1-160">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="eb9a1-161">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="eb9a1-161">allowPrinting</span></span>|<span data-ttu-id="eb9a1-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb9a1-162">Boolean</span></span>|<span data-ttu-id="eb9a1-163">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-163">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="eb9a1-164">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="eb9a1-164">allowScreenCapture</span></span>|<span data-ttu-id="eb9a1-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb9a1-165">Boolean</span></span>|<span data-ttu-id="eb9a1-166">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-166">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="eb9a1-167">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="eb9a1-167">allowTextSuggestion</span></span>|<span data-ttu-id="eb9a1-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb9a1-168">Boolean</span></span>|<span data-ttu-id="eb9a1-169">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-169">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="eb9a1-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb9a1-170">Response</span></span>
<span data-ttu-id="eb9a1-171">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-171">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb9a1-172">Пример</span><span class="sxs-lookup"><span data-stu-id="eb9a1-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb9a1-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb9a1-173">Request</span></span>
<span data-ttu-id="eb9a1-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 346

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="eb9a1-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb9a1-175">Response</span></span>
<span data-ttu-id="eb9a1-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="eb9a1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```



