# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="59275-101">Список androidWorkProfileGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="59275-101">List androidWorkProfileGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="59275-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="59275-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59275-103">Свойства списка и связи объектов [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="59275-103">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59275-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="59275-104">Prerequisites</span></span>
<span data-ttu-id="59275-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="59275-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="59275-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59275-107">Permission type</span></span>|<span data-ttu-id="59275-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59275-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59275-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59275-109">Delegated (work or school account)</span></span>|<span data-ttu-id="59275-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="59275-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="59275-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59275-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59275-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59275-112">Not supported.</span></span>|
|<span data-ttu-id="59275-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59275-113">Application</span></span>|<span data-ttu-id="59275-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59275-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59275-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59275-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="59275-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59275-116">Request headers</span></span>
|<span data-ttu-id="59275-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59275-117">Header</span></span>|<span data-ttu-id="59275-118">Значение</span><span class="sxs-lookup"><span data-stu-id="59275-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59275-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59275-119">Authorization</span></span>|<span data-ttu-id="59275-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="59275-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59275-121">Принять</span><span class="sxs-lookup"><span data-stu-id="59275-121">Accept</span></span>|<span data-ttu-id="59275-122">application/json</span><span class="sxs-lookup"><span data-stu-id="59275-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59275-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59275-123">Request body</span></span>
<span data-ttu-id="59275-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59275-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59275-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="59275-125">Response</span></span>
<span data-ttu-id="59275-126">При успешном выполнении этот метод возвращает код отклика  и коллекцию объектов androidWorkProfileGeneralDeviceConfiguration в тексте отклика.`200 OK` [ ](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59275-126">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59275-127">Пример</span><span class="sxs-lookup"><span data-stu-id="59275-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="59275-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="59275-128">Request</span></span>
<span data-ttu-id="59275-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59275-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="59275-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="59275-130">Response</span></span>
<span data-ttu-id="59275-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59275-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2200

{
  "value": [
    {
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
  ]
}
```








