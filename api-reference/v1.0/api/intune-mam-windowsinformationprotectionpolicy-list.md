---
title: Перечисление объектов WindowsInformationProtectionPolicy
description: Перечисление свойств и связей объектов windowsInformationProtectionPolicy.
author: tfitzmac
ms.openlocfilehash: 8912cf4e4453ff542d15bde2eb9e280b976ed93d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323732"
---
# <a name="list-windowsinformationprotectionpolicies"></a><span data-ttu-id="f7501-103">Перечисление объектов WindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="f7501-103">List windowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="f7501-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f7501-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7501-105">Перечисление свойств и связей объектов [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f7501-105">List properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f7501-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7501-106">Prerequisites</span></span>
<span data-ttu-id="f7501-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7501-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7501-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7501-109">Permission type</span></span>|<span data-ttu-id="f7501-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7501-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7501-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7501-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f7501-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7501-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f7501-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7501-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7501-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7501-114">Not supported.</span></span>|
|<span data-ttu-id="f7501-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7501-115">Application</span></span>|<span data-ttu-id="f7501-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7501-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7501-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7501-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f7501-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7501-118">Request headers</span></span>
|<span data-ttu-id="f7501-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7501-119">Header</span></span>|<span data-ttu-id="f7501-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f7501-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7501-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7501-121">Authorization</span></span>|<span data-ttu-id="f7501-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f7501-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7501-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f7501-123">Accept</span></span>|<span data-ttu-id="f7501-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f7501-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7501-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7501-125">Request body</span></span>
<span data-ttu-id="f7501-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7501-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7501-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7501-127">Response</span></span>
<span data-ttu-id="f7501-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f7501-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7501-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f7501-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f7501-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7501-130">Request</span></span>
<span data-ttu-id="f7501-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7501-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="f7501-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7501-132">Response</span></span>
<span data-ttu-id="f7501-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f7501-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5158

{
  "value": [
    {
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
      "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
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
  ]
}
```



