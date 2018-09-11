# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="49ed4-101">Создание deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="49ed4-101">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="49ed4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="49ed4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49ed4-103">Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49ed4-103">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49ed4-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49ed4-104">Prerequisites</span></span>
<span data-ttu-id="49ed4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="49ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="49ed4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49ed4-107">Permission type</span></span>|<span data-ttu-id="49ed4-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49ed4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49ed4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49ed4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="49ed4-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ed4-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="49ed4-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49ed4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49ed4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49ed4-112">Not supported.</span></span>|
|<span data-ttu-id="49ed4-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49ed4-113">Application</span></span>|<span data-ttu-id="49ed4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49ed4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49ed4-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49ed4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="49ed4-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49ed4-116">Request headers</span></span>
|<span data-ttu-id="49ed4-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49ed4-117">Header</span></span>|<span data-ttu-id="49ed4-118">Значение</span><span class="sxs-lookup"><span data-stu-id="49ed4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49ed4-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49ed4-119">Authorization</span></span>|<span data-ttu-id="49ed4-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="49ed4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49ed4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="49ed4-121">Accept</span></span>|<span data-ttu-id="49ed4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="49ed4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49ed4-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49ed4-123">Request body</span></span>
<span data-ttu-id="49ed4-124">В теле запроса добавьте представление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49ed4-124">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="49ed4-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="49ed4-125">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="49ed4-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="49ed4-126">Property</span></span>|<span data-ttu-id="49ed4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="49ed4-127">Type</span></span>|<span data-ttu-id="49ed4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="49ed4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49ed4-129">id</span><span class="sxs-lookup"><span data-stu-id="49ed4-129">id</span></span>|<span data-ttu-id="49ed4-130">Строка</span><span class="sxs-lookup"><span data-stu-id="49ed4-130">String</span></span>|<span data-ttu-id="49ed4-131">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49ed4-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49ed4-132">displayName</span><span class="sxs-lookup"><span data-stu-id="49ed4-132">displayName</span></span>|<span data-ttu-id="49ed4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="49ed4-133">String</span></span>|<span data-ttu-id="49ed4-134">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49ed4-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49ed4-135">description</span><span class="sxs-lookup"><span data-stu-id="49ed4-135">description</span></span>|<span data-ttu-id="49ed4-136">Строка</span><span class="sxs-lookup"><span data-stu-id="49ed4-136">String</span></span>|<span data-ttu-id="49ed4-137">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49ed4-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49ed4-138">priority</span><span class="sxs-lookup"><span data-stu-id="49ed4-138">priority</span></span>|<span data-ttu-id="49ed4-139">Int32</span><span class="sxs-lookup"><span data-stu-id="49ed4-139">Int32</span></span>|<span data-ttu-id="49ed4-140">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49ed4-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49ed4-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49ed4-141">createdDateTime</span></span>|<span data-ttu-id="49ed4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49ed4-142">DateTimeOffset</span></span>|<span data-ttu-id="49ed4-143">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49ed4-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49ed4-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49ed4-144">lastModifiedDateTime</span></span>|<span data-ttu-id="49ed4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49ed4-145">DateTimeOffset</span></span>|<span data-ttu-id="49ed4-146">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="49ed4-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49ed4-147">version</span><span class="sxs-lookup"><span data-stu-id="49ed4-147">version</span></span>|<span data-ttu-id="49ed4-148">Int32</span><span class="sxs-lookup"><span data-stu-id="49ed4-148">Int32</span></span>|<span data-ttu-id="49ed4-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49ed4-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="49ed4-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="49ed4-150">pinMinimumLength</span></span>|<span data-ttu-id="49ed4-151">Int32</span><span class="sxs-lookup"><span data-stu-id="49ed4-151">Int32</span></span>|<span data-ttu-id="49ed4-152">Н/Д</span><span class="sxs-lookup"><span data-stu-id="49ed4-152">Not yet documented</span></span>|
|<span data-ttu-id="49ed4-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="49ed4-153">pinMaximumLength</span></span>|<span data-ttu-id="49ed4-154">Int32</span><span class="sxs-lookup"><span data-stu-id="49ed4-154">Int32</span></span>|<span data-ttu-id="49ed4-155">Н/Д</span><span class="sxs-lookup"><span data-stu-id="49ed4-155">Not yet documented</span></span>|
|<span data-ttu-id="49ed4-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="49ed4-156">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="49ed4-157">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="49ed4-157">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="49ed4-p102">Еще не задокументировано. Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="49ed4-p102">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="49ed4-160">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="49ed4-160">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="49ed4-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="49ed4-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="49ed4-p103">Еще не задокументировано. Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="49ed4-p103">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="49ed4-164">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="49ed4-164">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="49ed4-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="49ed4-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="49ed4-p104">Еще не задокументировано. Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="49ed4-p104">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="49ed4-168">state</span><span class="sxs-lookup"><span data-stu-id="49ed4-168">state</span></span>|[<span data-ttu-id="49ed4-169">enablement</span><span class="sxs-lookup"><span data-stu-id="49ed4-169">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="49ed4-p105">Еще не задокументировано. Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="49ed4-p105">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="49ed4-172">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="49ed4-172">securityDeviceRequired</span></span>|<span data-ttu-id="49ed4-173">Логический</span><span class="sxs-lookup"><span data-stu-id="49ed4-173">Boolean</span></span>|<span data-ttu-id="49ed4-174">Н/Д</span><span class="sxs-lookup"><span data-stu-id="49ed4-174">Not yet documented</span></span>|
|<span data-ttu-id="49ed4-175">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="49ed4-175">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="49ed4-176">Логический</span><span class="sxs-lookup"><span data-stu-id="49ed4-176">Boolean</span></span>|<span data-ttu-id="49ed4-177">Н/Д</span><span class="sxs-lookup"><span data-stu-id="49ed4-177">Not yet documented</span></span>|
|<span data-ttu-id="49ed4-178">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="49ed4-178">remotePassportEnabled</span></span>|<span data-ttu-id="49ed4-179">Логический</span><span class="sxs-lookup"><span data-stu-id="49ed4-179">Boolean</span></span>|<span data-ttu-id="49ed4-180">Н/Д</span><span class="sxs-lookup"><span data-stu-id="49ed4-180">Not yet documented</span></span>|
|<span data-ttu-id="49ed4-181">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="49ed4-181">pinPreviousBlockCount</span></span>|<span data-ttu-id="49ed4-182">Int32</span><span class="sxs-lookup"><span data-stu-id="49ed4-182">Int32</span></span>|<span data-ttu-id="49ed4-183">Н/Д</span><span class="sxs-lookup"><span data-stu-id="49ed4-183">Not yet documented</span></span>|
|<span data-ttu-id="49ed4-184">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="49ed4-184">pinExpirationInDays</span></span>|<span data-ttu-id="49ed4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="49ed4-185">Int32</span></span>|<span data-ttu-id="49ed4-186">Н/Д</span><span class="sxs-lookup"><span data-stu-id="49ed4-186">Not yet documented</span></span>|
|<span data-ttu-id="49ed4-187">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="49ed4-187">enhancedBiometricsState</span></span>|[<span data-ttu-id="49ed4-188">enablement</span><span class="sxs-lookup"><span data-stu-id="49ed4-188">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="49ed4-p106">Еще не задокументировано. Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="49ed4-p106">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="49ed4-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="49ed4-191">Response</span></span>
<span data-ttu-id="49ed4-192">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="49ed4-192">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49ed4-193">Пример</span><span class="sxs-lookup"><span data-stu-id="49ed4-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="49ed4-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="49ed4-194">Request</span></span>
<span data-ttu-id="49ed4-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49ed4-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 693

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="49ed4-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="49ed4-196">Response</span></span>
<span data-ttu-id="49ed4-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49ed4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```








