# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="00264-101">Получение androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="00264-101">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="00264-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00264-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00264-103">Чтение свойства и связи объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="00264-103">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00264-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="00264-104">Prerequisites</span></span>
<span data-ttu-id="00264-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="00264-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00264-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00264-107">Permission type</span></span>|<span data-ttu-id="00264-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00264-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00264-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00264-109">Delegated (work or school account)</span></span>|<span data-ttu-id="00264-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="00264-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="00264-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00264-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00264-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00264-112">Not supported.</span></span>|
|<span data-ttu-id="00264-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00264-113">Application</span></span>|<span data-ttu-id="00264-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00264-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00264-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00264-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00264-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="00264-116">Optional query parameters</span></span>
<span data-ttu-id="00264-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="00264-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="00264-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00264-118">Request headers</span></span>
|<span data-ttu-id="00264-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00264-119">Header</span></span>|<span data-ttu-id="00264-120">Значение</span><span class="sxs-lookup"><span data-stu-id="00264-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00264-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="00264-121">Authorization</span></span>|<span data-ttu-id="00264-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="00264-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00264-123">Accept</span><span class="sxs-lookup"><span data-stu-id="00264-123">Accept</span></span>|<span data-ttu-id="00264-124">application/json</span><span class="sxs-lookup"><span data-stu-id="00264-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00264-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00264-125">Request body</span></span>
<span data-ttu-id="00264-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00264-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00264-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="00264-127">Response</span></span>
<span data-ttu-id="00264-128">Успешно завершена, этот метод возвращает `200 OK` объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="00264-128">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00264-129">Пример</span><span class="sxs-lookup"><span data-stu-id="00264-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="00264-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="00264-130">Request</span></span>
<span data-ttu-id="00264-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00264-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="00264-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="00264-132">Response</span></span>
<span data-ttu-id="00264-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="00264-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2104

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
    "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockTrustAgents": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "lowSecurityBiometric",
    "workProfileDataSharingType": "preventAny",
    "workProfileBlockNotificationsWhileDeviceLocked": true,
    "workProfileBlockAddingAccounts": true,
    "workProfileBluetoothEnableContactSharing": true,
    "workProfileBlockScreenCapture": true,
    "workProfileBlockCrossProfileCallerId": true,
    "workProfileBlockCamera": true,
    "workProfileBlockCrossProfileContactsSearch": true,
    "workProfileBlockCrossProfileCopyPaste": true,
    "workProfileDefaultAppPermissionPolicy": "prompt",
    "workProfilePasswordBlockFingerprintUnlock": true,
    "workProfilePasswordBlockTrustAgents": true,
    "workProfilePasswordExpirationDays": 1,
    "workProfilePasswordMinimumLength": 0,
    "workProfilePasswordMinNumericCharacters": 7,
    "workProfilePasswordMinNonLetterCharacters": 9,
    "workProfilePasswordMinLetterCharacters": 6,
    "workProfilePasswordMinLowerCaseCharacters": 9,
    "workProfilePasswordMinUpperCaseCharacters": 9,
    "workProfilePasswordMinSymbolCharacters": 6,
    "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
    "workProfilePasswordPreviousPasswordBlockCount": 13,
    "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
    "workProfilePasswordRequiredType": "lowSecurityBiometric",
    "workProfileRequirePassword": true,
    "securityRequireVerifyApps": true
  }
}
```



