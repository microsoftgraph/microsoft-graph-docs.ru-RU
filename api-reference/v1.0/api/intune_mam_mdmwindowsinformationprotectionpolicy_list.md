# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="c3c01-101">Перечисление объектов mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c3c01-101">List mdmWindowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="c3c01-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c3c01-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3c01-103">Перечисление свойств и связей объектов [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c3c01-103">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3c01-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c3c01-104">Prerequisites</span></span>
<span data-ttu-id="c3c01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c3c01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c3c01-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3c01-107">Permission type</span></span>|<span data-ttu-id="c3c01-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3c01-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3c01-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3c01-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c3c01-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3c01-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c3c01-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3c01-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3c01-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3c01-112">Not supported.</span></span>|
|<span data-ttu-id="c3c01-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3c01-113">Application</span></span>|<span data-ttu-id="c3c01-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3c01-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3c01-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3c01-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c3c01-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3c01-116">Request headers</span></span>
|<span data-ttu-id="c3c01-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3c01-117">Header</span></span>|<span data-ttu-id="c3c01-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c3c01-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3c01-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3c01-119">Authorization</span></span>|<span data-ttu-id="c3c01-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="c3c01-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3c01-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c3c01-121">Accept</span></span>|<span data-ttu-id="c3c01-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c3c01-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3c01-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3c01-123">Request body</span></span>
<span data-ttu-id="c3c01-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3c01-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3c01-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3c01-125">Response</span></span>
<span data-ttu-id="c3c01-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c3c01-126">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3c01-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c3c01-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3c01-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3c01-128">Request</span></span>
<span data-ttu-id="c3c01-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3c01-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="c3c01-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3c01-130">Response</span></span>
<span data-ttu-id="c3c01-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3c01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4607

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "8efb0c35-0c35-8efb-350c-fb8e350cfb8e",
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
      "isAssigned": true
    }
  ]
}
```



