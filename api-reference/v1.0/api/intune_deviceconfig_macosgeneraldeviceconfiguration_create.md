# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="1813a-101">Создание macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1813a-101">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="1813a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1813a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1813a-103">Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1813a-103">Create a new [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1813a-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1813a-104">Prerequisites</span></span>
<span data-ttu-id="1813a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1813a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1813a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1813a-107">Permission type</span></span>|<span data-ttu-id="1813a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1813a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1813a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1813a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1813a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1813a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1813a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1813a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1813a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1813a-112">Not supported.</span></span>|
|<span data-ttu-id="1813a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1813a-113">Application</span></span>|<span data-ttu-id="1813a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1813a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1813a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1813a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1813a-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1813a-116">Request headers</span></span>
|<span data-ttu-id="1813a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1813a-117">Header</span></span>|<span data-ttu-id="1813a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1813a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1813a-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1813a-119">Authorization</span></span>|<span data-ttu-id="1813a-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="1813a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1813a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1813a-121">Accept</span></span>|<span data-ttu-id="1813a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1813a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1813a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1813a-123">Request body</span></span>
<span data-ttu-id="1813a-124">В тексте запроса добавьте представление объекта macOSGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1813a-124">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="1813a-125">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1813a-125">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="1813a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="1813a-126">Property</span></span>|<span data-ttu-id="1813a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1813a-127">Type</span></span>|<span data-ttu-id="1813a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1813a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1813a-129">id</span><span class="sxs-lookup"><span data-stu-id="1813a-129">id</span></span>|<span data-ttu-id="1813a-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="1813a-130">String</span></span>|<span data-ttu-id="1813a-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1813a-131">Key of the entity.</span></span> <span data-ttu-id="1813a-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1813a-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1813a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1813a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="1813a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1813a-134">DateTimeOffset</span></span>|<span data-ttu-id="1813a-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1813a-135">DateTime the object was last modified.</span></span> <span data-ttu-id="1813a-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1813a-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1813a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1813a-137">createdDateTime</span></span>|<span data-ttu-id="1813a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1813a-138">DateTimeOffset</span></span>|<span data-ttu-id="1813a-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1813a-139">DateTime the object was created.</span></span> <span data-ttu-id="1813a-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1813a-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1813a-141">description</span><span class="sxs-lookup"><span data-stu-id="1813a-141">description</span></span>|<span data-ttu-id="1813a-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="1813a-142">String</span></span>|<span data-ttu-id="1813a-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1813a-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1813a-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1813a-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1813a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1813a-145">displayName</span></span>|<span data-ttu-id="1813a-146">String (строка)</span><span class="sxs-lookup"><span data-stu-id="1813a-146">String</span></span>|<span data-ttu-id="1813a-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1813a-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1813a-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1813a-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1813a-149">version</span><span class="sxs-lookup"><span data-stu-id="1813a-149">version</span></span>|<span data-ttu-id="1813a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1813a-150">Int32</span></span>|<span data-ttu-id="1813a-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1813a-151">Version of the device configuration.</span></span> <span data-ttu-id="1813a-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1813a-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1813a-153">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="1813a-153">compliantAppsList</span></span>|<span data-ttu-id="1813a-154">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1813a-154">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="1813a-155">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="1813a-155">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="1813a-156">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="1813a-156">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="1813a-157">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="1813a-157">compliantAppListType</span></span>|[<span data-ttu-id="1813a-158">appListType</span><span class="sxs-lookup"><span data-stu-id="1813a-158">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="1813a-159">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="1813a-159">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="1813a-160">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="1813a-160">The possible values are `none`, `appsInListCompliant`, `appsNotInListCompliant`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="1813a-161">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="1813a-161">emailInDomainSuffixes</span></span>|<span data-ttu-id="1813a-162">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1813a-162">String collection</span></span>|<span data-ttu-id="1813a-163">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="1813a-163">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="1813a-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1813a-164">passwordBlockSimple</span></span>|<span data-ttu-id="1813a-165">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="1813a-165">Boolean</span></span>|<span data-ttu-id="1813a-166">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="1813a-166">Block simple passwords.</span></span>|
|<span data-ttu-id="1813a-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1813a-167">passwordExpirationDays</span></span>|<span data-ttu-id="1813a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="1813a-168">Int32</span></span>|<span data-ttu-id="1813a-169">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="1813a-169">Number of days before the password expires.</span></span>|
|<span data-ttu-id="1813a-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1813a-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="1813a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="1813a-171">Int32</span></span>|<span data-ttu-id="1813a-172">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="1813a-172">Number of character sets a password must contain.</span></span> <span data-ttu-id="1813a-173">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="1813a-173">Valid values 0 to 4</span></span>|
|<span data-ttu-id="1813a-174">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1813a-174">passwordMinimumLength</span></span>|<span data-ttu-id="1813a-175">Int32</span><span class="sxs-lookup"><span data-stu-id="1813a-175">Int32</span></span>|<span data-ttu-id="1813a-176">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="1813a-176">Minimum length of passwords.</span></span>|
|<span data-ttu-id="1813a-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1813a-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1813a-178">Int32</span><span class="sxs-lookup"><span data-stu-id="1813a-178">Int32</span></span>|<span data-ttu-id="1813a-179">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="1813a-179">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="1813a-180">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1813a-180">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1813a-181">Int32</span><span class="sxs-lookup"><span data-stu-id="1813a-181">Int32</span></span>|<span data-ttu-id="1813a-182">Период бездействия (в минутах), по истечении которого гаснет экран.</span><span class="sxs-lookup"><span data-stu-id="1813a-182">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="1813a-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1813a-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1813a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1813a-184">Int32</span></span>|<span data-ttu-id="1813a-185">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="1813a-185">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="1813a-186">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1813a-186">passwordRequiredType</span></span>|[<span data-ttu-id="1813a-187">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1813a-187">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="1813a-188">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="1813a-188">Type of password that is required.</span></span> <span data-ttu-id="1813a-189">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="1813a-189">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="1813a-190">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1813a-190">passwordRequired</span></span>|<span data-ttu-id="1813a-191">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="1813a-191">Boolean</span></span>|<span data-ttu-id="1813a-192">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="1813a-192">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="1813a-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="1813a-193">Response</span></span>
<span data-ttu-id="1813a-194">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1813a-194">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1813a-195">Пример</span><span class="sxs-lookup"><span data-stu-id="1813a-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="1813a-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="1813a-196">Request</span></span>
<span data-ttu-id="1813a-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1813a-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 970

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```

### <a name="response"></a><span data-ttu-id="1813a-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="1813a-198">Response</span></span>
<span data-ttu-id="1813a-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1813a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1078

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```



