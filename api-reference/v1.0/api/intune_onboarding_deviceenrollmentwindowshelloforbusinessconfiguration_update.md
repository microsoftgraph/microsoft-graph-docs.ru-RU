# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="2a3c5-101">Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a3c5-101">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="2a3c5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a3c5-103">Обновление свойств объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a3c5-103">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a3c5-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2a3c5-104">Prerequisites</span></span>
<span data-ttu-id="2a3c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2a3c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a3c5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a3c5-107">Permission type</span></span>|<span data-ttu-id="2a3c5-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a3c5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a3c5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a3c5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2a3c5-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a3c5-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a3c5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a3c5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a3c5-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-112">Not supported.</span></span>|
|<span data-ttu-id="2a3c5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a3c5-113">Application</span></span>|<span data-ttu-id="2a3c5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a3c5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a3c5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2a3c5-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a3c5-116">Request headers</span></span>
|<span data-ttu-id="2a3c5-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a3c5-117">Header</span></span>|<span data-ttu-id="2a3c5-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2a3c5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a3c5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a3c5-119">Authorization</span></span>|<span data-ttu-id="2a3c5-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a3c5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2a3c5-121">Accept</span></span>|<span data-ttu-id="2a3c5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2a3c5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a3c5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a3c5-123">Request body</span></span>
<span data-ttu-id="2a3c5-124">В теле запроса добавьте представление объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-124">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="2a3c5-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a3c5-125">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="2a3c5-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a3c5-126">Property</span></span>|<span data-ttu-id="2a3c5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2a3c5-127">Type</span></span>|<span data-ttu-id="2a3c5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2a3c5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a3c5-129">id</span><span class="sxs-lookup"><span data-stu-id="2a3c5-129">id</span></span>|<span data-ttu-id="2a3c5-130">String</span><span class="sxs-lookup"><span data-stu-id="2a3c5-130">String</span></span>|<span data-ttu-id="2a3c5-131">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a3c5-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a3c5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2a3c5-132">displayName</span></span>|<span data-ttu-id="2a3c5-133">String</span><span class="sxs-lookup"><span data-stu-id="2a3c5-133">String</span></span>|<span data-ttu-id="2a3c5-134">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a3c5-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a3c5-135">description</span><span class="sxs-lookup"><span data-stu-id="2a3c5-135">description</span></span>|<span data-ttu-id="2a3c5-136">String</span><span class="sxs-lookup"><span data-stu-id="2a3c5-136">String</span></span>|<span data-ttu-id="2a3c5-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a3c5-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a3c5-138">priority</span><span class="sxs-lookup"><span data-stu-id="2a3c5-138">priority</span></span>|<span data-ttu-id="2a3c5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2a3c5-139">Int32</span></span>|<span data-ttu-id="2a3c5-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a3c5-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a3c5-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a3c5-141">createdDateTime</span></span>|<span data-ttu-id="2a3c5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a3c5-142">DateTimeOffset</span></span>|<span data-ttu-id="2a3c5-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a3c5-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a3c5-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a3c5-144">lastModifiedDateTime</span></span>|<span data-ttu-id="2a3c5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a3c5-145">DateTimeOffset</span></span>|<span data-ttu-id="2a3c5-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a3c5-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a3c5-147">version</span><span class="sxs-lookup"><span data-stu-id="2a3c5-147">version</span></span>|<span data-ttu-id="2a3c5-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2a3c5-148">Int32</span></span>|<span data-ttu-id="2a3c5-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a3c5-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2a3c5-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2a3c5-150">pinMinimumLength</span></span>|<span data-ttu-id="2a3c5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2a3c5-151">Int32</span></span>|<span data-ttu-id="2a3c5-152">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="2a3c5-152">Not yet documented</span></span>|
|<span data-ttu-id="2a3c5-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="2a3c5-153">pinMaximumLength</span></span>|<span data-ttu-id="2a3c5-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2a3c5-154">Int32</span></span>|<span data-ttu-id="2a3c5-155">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="2a3c5-155">Not yet documented</span></span>|
|<span data-ttu-id="2a3c5-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="2a3c5-156">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="2a3c5-157">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="2a3c5-157">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="2a3c5-158">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-158">Not yet documented.</span></span> <span data-ttu-id="2a3c5-159">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-159">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="2a3c5-160">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="2a3c5-160">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="2a3c5-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="2a3c5-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="2a3c5-162">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-162">Not yet documented.</span></span> <span data-ttu-id="2a3c5-163">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="2a3c5-164">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="2a3c5-164">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="2a3c5-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="2a3c5-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="2a3c5-166">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-166">Not yet documented.</span></span> <span data-ttu-id="2a3c5-167">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="2a3c5-168">state</span><span class="sxs-lookup"><span data-stu-id="2a3c5-168">state</span></span>|[<span data-ttu-id="2a3c5-169">Включение</span><span class="sxs-lookup"><span data-stu-id="2a3c5-169">enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="2a3c5-170">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-170">Not yet documented.</span></span> <span data-ttu-id="2a3c5-171">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-171">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="2a3c5-172">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="2a3c5-172">securityDeviceRequired</span></span>|<span data-ttu-id="2a3c5-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a3c5-173">Boolean</span></span>|<span data-ttu-id="2a3c5-174">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2a3c5-174">Not yet documented</span></span>|
|<span data-ttu-id="2a3c5-175">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="2a3c5-175">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="2a3c5-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a3c5-176">Boolean</span></span>|<span data-ttu-id="2a3c5-177">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2a3c5-177">Not yet documented</span></span>|
|<span data-ttu-id="2a3c5-178">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="2a3c5-178">remotePassportEnabled</span></span>|<span data-ttu-id="2a3c5-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a3c5-179">Boolean</span></span>|<span data-ttu-id="2a3c5-180">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2a3c5-180">Not yet documented</span></span>|
|<span data-ttu-id="2a3c5-181">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="2a3c5-181">pinPreviousBlockCount</span></span>|<span data-ttu-id="2a3c5-182">Int32</span><span class="sxs-lookup"><span data-stu-id="2a3c5-182">Int32</span></span>|<span data-ttu-id="2a3c5-183">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2a3c5-183">Not yet documented</span></span>|
|<span data-ttu-id="2a3c5-184">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="2a3c5-184">pinExpirationInDays</span></span>|<span data-ttu-id="2a3c5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="2a3c5-185">Int32</span></span>|<span data-ttu-id="2a3c5-186">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2a3c5-186">Not yet documented</span></span>|
|<span data-ttu-id="2a3c5-187">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="2a3c5-187">enhancedBiometricsState</span></span>|[<span data-ttu-id="2a3c5-188">Включение</span><span class="sxs-lookup"><span data-stu-id="2a3c5-188">enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="2a3c5-189">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-189">Not yet documented.</span></span> <span data-ttu-id="2a3c5-190">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="2a3c5-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a3c5-191">Response</span></span>
<span data-ttu-id="2a3c5-192">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-192">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a3c5-193">Пример</span><span class="sxs-lookup"><span data-stu-id="2a3c5-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a3c5-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a3c5-194">Request</span></span>
<span data-ttu-id="2a3c5-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a3c5-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="2a3c5-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a3c5-196">Response</span></span>
<span data-ttu-id="2a3c5-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2a3c5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



