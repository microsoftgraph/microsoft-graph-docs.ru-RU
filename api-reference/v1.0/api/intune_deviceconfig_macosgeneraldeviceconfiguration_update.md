# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="fc783-101">Update macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="fc783-101">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="fc783-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fc783-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc783-103">Обновление свойств объекта [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc783-103">Update the properties of a [calendar](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc783-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fc783-104">Prerequisites</span></span>
<span data-ttu-id="fc783-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fc783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fc783-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc783-107">Permission type</span></span>|<span data-ttu-id="fc783-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc783-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc783-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc783-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fc783-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc783-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc783-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc783-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc783-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc783-112">Not supported.</span></span>|
|<span data-ttu-id="fc783-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc783-113">Application</span></span>|<span data-ttu-id="fc783-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc783-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc783-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc783-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fc783-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fc783-116">Request headers</span></span>
|<span data-ttu-id="fc783-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc783-117">Header</span></span>|<span data-ttu-id="fc783-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fc783-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc783-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc783-119">Authorization</span></span>|<span data-ttu-id="fc783-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc783-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fc783-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fc783-121">Accept</span></span>|<span data-ttu-id="fc783-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fc783-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc783-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc783-123">Request body</span></span>
<span data-ttu-id="fc783-124">В теле запроса добавьте представление объекта [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc783-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="fc783-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc783-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="fc783-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc783-126">Property</span></span>|<span data-ttu-id="fc783-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fc783-127">Type</span></span>|<span data-ttu-id="fc783-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fc783-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc783-129">id</span><span class="sxs-lookup"><span data-stu-id="fc783-129">id</span></span>|<span data-ttu-id="fc783-130">String</span><span class="sxs-lookup"><span data-stu-id="fc783-130">String</span></span>|<span data-ttu-id="fc783-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc783-131">Key of the setting.</span></span> <span data-ttu-id="fc783-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc783-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc783-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc783-133">lastModifiedDateTime</span></span>|<span data-ttu-id="fc783-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc783-134">DateTimeOffset</span></span>|<span data-ttu-id="fc783-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fc783-135">DateTime the object was last modified.</span></span> <span data-ttu-id="fc783-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc783-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc783-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc783-137">createdDateTime</span></span>|<span data-ttu-id="fc783-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc783-138">DateTimeOffset</span></span>|<span data-ttu-id="fc783-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fc783-139">DateTime the object was created.</span></span> <span data-ttu-id="fc783-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc783-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc783-141">description</span><span class="sxs-lookup"><span data-stu-id="fc783-141">description</span></span>|<span data-ttu-id="fc783-142">String</span><span class="sxs-lookup"><span data-stu-id="fc783-142">String</span></span>|<span data-ttu-id="fc783-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc783-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fc783-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc783-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc783-145">displayName</span><span class="sxs-lookup"><span data-stu-id="fc783-145">displayName</span></span>|<span data-ttu-id="fc783-146">String</span><span class="sxs-lookup"><span data-stu-id="fc783-146">String</span></span>|<span data-ttu-id="fc783-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc783-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fc783-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc783-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc783-149">version</span><span class="sxs-lookup"><span data-stu-id="fc783-149">version</span></span>|<span data-ttu-id="fc783-150">Int32</span><span class="sxs-lookup"><span data-stu-id="fc783-150">Int32</span></span>|<span data-ttu-id="fc783-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc783-151">Version of the device configuration.</span></span> <span data-ttu-id="fc783-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc783-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc783-153">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="fc783-153">compliantAppsList</span></span>|<span data-ttu-id="fc783-154">Коллекция [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="fc783-154">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="fc783-155">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="fc783-155">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="fc783-156">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="fc783-156">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="fc783-157">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="fc783-157">compliantAppListType</span></span>|<span data-ttu-id="fc783-158">String</span><span class="sxs-lookup"><span data-stu-id="fc783-158">String</span></span>|<span data-ttu-id="fc783-159">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="fc783-159">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="fc783-160">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="fc783-160">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="fc783-161">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="fc783-161">emailInDomainSuffixes</span></span>|<span data-ttu-id="fc783-162">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc783-162">String collection</span></span>|<span data-ttu-id="fc783-163">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="fc783-163">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="fc783-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="fc783-164">passwordBlockSimple</span></span>|<span data-ttu-id="fc783-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc783-165">Boolean</span></span>|<span data-ttu-id="fc783-166">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="fc783-166">Block simple passwords.</span></span>|
|<span data-ttu-id="fc783-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fc783-167">passwordExpirationDays</span></span>|<span data-ttu-id="fc783-168">Int32</span><span class="sxs-lookup"><span data-stu-id="fc783-168">Int32</span></span>|<span data-ttu-id="fc783-169">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="fc783-169">Number of days before the password expires.</span></span>|
|<span data-ttu-id="fc783-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="fc783-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="fc783-171">Int32</span><span class="sxs-lookup"><span data-stu-id="fc783-171">Int32</span></span>|<span data-ttu-id="fc783-172">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="fc783-172">Number of character sets a password must contain.</span></span> <span data-ttu-id="fc783-173">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="fc783-173">Valid values 0 to 4</span></span>|
|<span data-ttu-id="fc783-174">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fc783-174">passwordMinimumLength</span></span>|<span data-ttu-id="fc783-175">Int32</span><span class="sxs-lookup"><span data-stu-id="fc783-175">Int32</span></span>|<span data-ttu-id="fc783-176">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="fc783-176">Minimum length of passwords.</span></span>|
|<span data-ttu-id="fc783-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="fc783-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="fc783-178">Int32</span><span class="sxs-lookup"><span data-stu-id="fc783-178">Int32</span></span>|<span data-ttu-id="fc783-179">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="fc783-179">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="fc783-180">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="fc783-180">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="fc783-181">Int32</span><span class="sxs-lookup"><span data-stu-id="fc783-181">Int32</span></span>|<span data-ttu-id="fc783-182">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="fc783-182">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="fc783-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="fc783-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="fc783-184">Int32</span><span class="sxs-lookup"><span data-stu-id="fc783-184">Int32</span></span>|<span data-ttu-id="fc783-185">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="fc783-185">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="fc783-186">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="fc783-186">passwordRequiredType</span></span>|<span data-ttu-id="fc783-187">String</span><span class="sxs-lookup"><span data-stu-id="fc783-187">String</span></span>|<span data-ttu-id="fc783-188">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="fc783-188">Type of password that is required.</span></span> <span data-ttu-id="fc783-189">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="fc783-189">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="fc783-190">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="fc783-190">passwordRequired</span></span>|<span data-ttu-id="fc783-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc783-191">Boolean</span></span>|<span data-ttu-id="fc783-192">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="fc783-192">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="fc783-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc783-193">Response</span></span>
<span data-ttu-id="fc783-194">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fc783-194">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc783-195">Пример</span><span class="sxs-lookup"><span data-stu-id="fc783-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc783-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc783-196">Request</span></span>
<span data-ttu-id="fc783-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc783-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 900

{
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

### <a name="response"></a><span data-ttu-id="fc783-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc783-198">Response</span></span>
<span data-ttu-id="fc783-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fc783-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



