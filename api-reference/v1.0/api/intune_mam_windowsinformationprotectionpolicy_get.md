# <a name="get-windowsinformationprotectionpolicy"></a><span data-ttu-id="21b8b-101">Получение объекта windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="21b8b-101">Get windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="21b8b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21b8b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21b8b-103">Чтение свойств и связей объекта [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="21b8b-103">Read properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21b8b-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="21b8b-104">Prerequisites</span></span>
<span data-ttu-id="21b8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="21b8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="21b8b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21b8b-107">Permission type</span></span>|<span data-ttu-id="21b8b-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21b8b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21b8b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21b8b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="21b8b-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="21b8b-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="21b8b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21b8b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21b8b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21b8b-112">Not supported.</span></span>|
|<span data-ttu-id="21b8b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21b8b-113">Application</span></span>|<span data-ttu-id="21b8b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21b8b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21b8b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21b8b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21b8b-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="21b8b-116">Optional query parameters</span></span>
<span data-ttu-id="21b8b-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="21b8b-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="21b8b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21b8b-118">Request headers</span></span>
|<span data-ttu-id="21b8b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21b8b-119">Header</span></span>|<span data-ttu-id="21b8b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="21b8b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21b8b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21b8b-121">Authorization</span></span>|<span data-ttu-id="21b8b-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="21b8b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21b8b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="21b8b-123">Accept</span></span>|<span data-ttu-id="21b8b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="21b8b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21b8b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21b8b-125">Request body</span></span>
<span data-ttu-id="21b8b-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21b8b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21b8b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="21b8b-127">Response</span></span>
<span data-ttu-id="21b8b-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="21b8b-128">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21b8b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="21b8b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="21b8b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="21b8b-130">Request</span></span>
<span data-ttu-id="21b8b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21b8b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="21b8b-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="21b8b-132">Response</span></span>
<span data-ttu-id="21b8b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21b8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4867

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "6397be61-be61-6397-61be-976361be9763",
    "version": "Version value",
    "enforcementLevel": "encryptAndAuditOnly",
    "enterpriseDomain": "Enterprise Domain value",
    "enterpriseProtectedDomainNames": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "protectionUnderLockConfigRequired": true,
    "dataRecoveryCertificate": {
      "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
      "subjectName": "Subject Name value",
      "description": "Description value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "certificate": "Y2VydGlmaWNhdGU="
    },
    "revokeOnUnenrollDisabled": true,
    "rightsManagementServicesTemplateId": "79199ed9-e50b-4257-8de4-70b9c8685061",
    "azureRightsManagementServicesAllowed": true,
    "iconsVisible": true,
    "protectedApps": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
        "displayName": "Display Name value",
        "description": "Description value",
        "publisherName": "Publisher Name value",
        "productName": "Product Name value",
        "denied": true
      }
    ],
    "exemptApps": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
        "displayName": "Display Name value",
        "description": "Description value",
        "publisherName": "Publisher Name value",
        "productName": "Product Name value",
        "denied": true
      }
    ],
    "enterpriseNetworkDomainNames": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseProxiedDomains": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
        "displayName": "Display Name value",
        "proxiedDomains": [
          {
            "@odata.type": "microsoft.graph.proxiedDomain",
            "ipAddressOrFQDN": "Ip Address Or FQDN value",
            "proxy": "Proxy value"
          }
        ]
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
        "displayName": "Display Name value",
        "ranges": [
          {
            "@odata.type": "microsoft.graph.iPv6Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ]
      }
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseInternalProxyServers": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "indexingEncryptedStoresOrItemsBlocked": true,
    "smbAutoEncryptedFileExtensions": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "isAssigned": true,
    "revokeOnMdmHandoffDisabled": true,
    "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
    "windowsHelloForBusinessBlocked": true,
    "pinMinimumLength": 0,
    "pinUppercaseLetters": "requireAtLeastOne",
    "pinLowercaseLetters": "requireAtLeastOne",
    "pinSpecialCharacters": "requireAtLeastOne",
    "pinExpirationDays": 1,
    "numberOfPastPinsRemembered": 10,
    "passwordMaximumAttemptCount": 11,
    "minutesOfInactivityBeforeDeviceLock": 3,
    "daysWithoutContactBeforeUnenroll": 0
  }
}
```



