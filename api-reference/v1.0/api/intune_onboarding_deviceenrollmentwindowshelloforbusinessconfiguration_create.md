# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="ce88f-101">Создание deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce88f-101">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="ce88f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ce88f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce88f-103">Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce88f-103">Create a new [plannerBucket](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce88f-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ce88f-104">Prerequisites</span></span>
<span data-ttu-id="ce88f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce88f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce88f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce88f-107">Permission type</span></span>|<span data-ttu-id="ce88f-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce88f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce88f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce88f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ce88f-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce88f-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ce88f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce88f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce88f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce88f-112">Not supported.</span></span>|
|<span data-ttu-id="ce88f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce88f-113">Application</span></span>|<span data-ttu-id="ce88f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce88f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce88f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce88f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ce88f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce88f-116">Request headers</span></span>
|<span data-ttu-id="ce88f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce88f-117">Header</span></span>|<span data-ttu-id="ce88f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ce88f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce88f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce88f-119">Authorization</span></span>|<span data-ttu-id="ce88f-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce88f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ce88f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ce88f-121">Accept</span></span>|<span data-ttu-id="ce88f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ce88f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce88f-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ce88f-123">Request body</span></span>
<span data-ttu-id="ce88f-124">В теле запроса добавьте представление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce88f-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="ce88f-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ce88f-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ce88f-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce88f-126">Property</span></span>|<span data-ttu-id="ce88f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ce88f-127">Type</span></span>|<span data-ttu-id="ce88f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ce88f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce88f-129">id</span><span class="sxs-lookup"><span data-stu-id="ce88f-129">id</span></span>|<span data-ttu-id="ce88f-130">String</span><span class="sxs-lookup"><span data-stu-id="ce88f-130">String</span></span>|<span data-ttu-id="ce88f-131">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce88f-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ce88f-132">displayName</span></span>|<span data-ttu-id="ce88f-133">String</span><span class="sxs-lookup"><span data-stu-id="ce88f-133">String</span></span>|<span data-ttu-id="ce88f-134">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce88f-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-135">description</span><span class="sxs-lookup"><span data-stu-id="ce88f-135">description</span></span>|<span data-ttu-id="ce88f-136">String</span><span class="sxs-lookup"><span data-stu-id="ce88f-136">String</span></span>|<span data-ttu-id="ce88f-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce88f-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-138">priority</span><span class="sxs-lookup"><span data-stu-id="ce88f-138">priority</span></span>|<span data-ttu-id="ce88f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ce88f-139">Int32</span></span>|<span data-ttu-id="ce88f-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce88f-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce88f-141">createdDateTime</span></span>|<span data-ttu-id="ce88f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce88f-142">DateTimeOffset</span></span>|<span data-ttu-id="ce88f-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce88f-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce88f-144">lastModifiedDateTime</span></span>|<span data-ttu-id="ce88f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce88f-145">DateTimeOffset</span></span>|<span data-ttu-id="ce88f-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce88f-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-147">version</span><span class="sxs-lookup"><span data-stu-id="ce88f-147">version</span></span>|<span data-ttu-id="ce88f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ce88f-148">Int32</span></span>|<span data-ttu-id="ce88f-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce88f-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce88f-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ce88f-150">pinMinimumLength</span></span>|<span data-ttu-id="ce88f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ce88f-151">Int32</span></span>|<span data-ttu-id="ce88f-152">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="ce88f-152">Not yet documented</span></span>|
|<span data-ttu-id="ce88f-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="ce88f-153">pinMaximumLength</span></span>|<span data-ttu-id="ce88f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ce88f-154">Int32</span></span>|<span data-ttu-id="ce88f-155">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="ce88f-155">Not yet documented</span></span>|
|<span data-ttu-id="ce88f-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ce88f-156">pinUppercaseCharactersUsage</span></span>|<span data-ttu-id="ce88f-157">String</span><span class="sxs-lookup"><span data-stu-id="ce88f-157">String</span></span>|<span data-ttu-id="ce88f-158">Еще не задокументировано. Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="ce88f-158">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ce88f-159">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ce88f-159">pinLowercaseCharactersUsage</span></span>|<span data-ttu-id="ce88f-160">String</span><span class="sxs-lookup"><span data-stu-id="ce88f-160">String</span></span>|<span data-ttu-id="ce88f-161">Еще не задокументировано. Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="ce88f-161">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ce88f-162">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ce88f-162">pinSpecialCharactersUsage</span></span>|<span data-ttu-id="ce88f-163">String</span><span class="sxs-lookup"><span data-stu-id="ce88f-163">String</span></span>|<span data-ttu-id="ce88f-164">Еще не задокументировано. Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="ce88f-164">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ce88f-165">state</span><span class="sxs-lookup"><span data-stu-id="ce88f-165">state</span></span>|<span data-ttu-id="ce88f-166">String</span><span class="sxs-lookup"><span data-stu-id="ce88f-166">String</span></span>|<span data-ttu-id="ce88f-167">Еще не задокументировано. Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ce88f-167">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ce88f-168">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="ce88f-168">securityDeviceRequired</span></span>|<span data-ttu-id="ce88f-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce88f-169">Boolean</span></span>|<span data-ttu-id="ce88f-170">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="ce88f-170">Not yet documented</span></span>|
|<span data-ttu-id="ce88f-171">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="ce88f-171">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="ce88f-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce88f-172">Boolean</span></span>|<span data-ttu-id="ce88f-173">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="ce88f-173">Not yet documented</span></span>|
|<span data-ttu-id="ce88f-174">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="ce88f-174">remotePassportEnabled</span></span>|<span data-ttu-id="ce88f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce88f-175">Boolean</span></span>|<span data-ttu-id="ce88f-176">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="ce88f-176">Not yet documented</span></span>|
|<span data-ttu-id="ce88f-177">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="ce88f-177">pinPreviousBlockCount</span></span>|<span data-ttu-id="ce88f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="ce88f-178">Int32</span></span>|<span data-ttu-id="ce88f-179">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="ce88f-179">Not yet documented</span></span>|
|<span data-ttu-id="ce88f-180">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="ce88f-180">pinExpirationInDays</span></span>|<span data-ttu-id="ce88f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="ce88f-181">Int32</span></span>|<span data-ttu-id="ce88f-182">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="ce88f-182">Not yet documented</span></span>|
|<span data-ttu-id="ce88f-183">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="ce88f-183">enhancedBiometricsState</span></span>|<span data-ttu-id="ce88f-184">String</span><span class="sxs-lookup"><span data-stu-id="ce88f-184">String</span></span>|<span data-ttu-id="ce88f-185">Еще не задокументировано. Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ce88f-185">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="ce88f-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce88f-186">Response</span></span>
<span data-ttu-id="ce88f-187">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ce88f-187">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce88f-188">Пример</span><span class="sxs-lookup"><span data-stu-id="ce88f-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce88f-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce88f-189">Request</span></span>
<span data-ttu-id="ce88f-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce88f-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ce88f-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce88f-191">Response</span></span>
<span data-ttu-id="ce88f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ce88f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



