---
title: Получение объекта windowsInformationProtectionPolicy
description: Чтение свойств и связей объекта windowsInformationProtectionPolicy.
ms.openlocfilehash: aeef25f6ef285bec993fd1fc68799a83f9931328
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025614"
---
# <a name="get-windowsinformationprotectionpolicy"></a><span data-ttu-id="85d97-103">Получение объекта windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="85d97-103">Get windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="85d97-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="85d97-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85d97-105">Чтение свойств и связей объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="85d97-105">Read properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85d97-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="85d97-106">Prerequisites</span></span>
<span data-ttu-id="85d97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85d97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85d97-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85d97-109">Permission type</span></span>|<span data-ttu-id="85d97-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85d97-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85d97-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85d97-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85d97-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="85d97-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="85d97-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85d97-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85d97-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85d97-114">Not supported.</span></span>|
|<span data-ttu-id="85d97-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85d97-115">Application</span></span>|<span data-ttu-id="85d97-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85d97-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85d97-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85d97-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85d97-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85d97-118">Optional query parameters</span></span>
<span data-ttu-id="85d97-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="85d97-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="85d97-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85d97-120">Request headers</span></span>
|<span data-ttu-id="85d97-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85d97-121">Header</span></span>|<span data-ttu-id="85d97-122">Значение</span><span class="sxs-lookup"><span data-stu-id="85d97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85d97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85d97-123">Authorization</span></span>|<span data-ttu-id="85d97-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="85d97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85d97-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85d97-125">Accept</span></span>|<span data-ttu-id="85d97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85d97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85d97-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85d97-127">Request body</span></span>
<span data-ttu-id="85d97-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85d97-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85d97-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="85d97-129">Response</span></span>
<span data-ttu-id="85d97-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="85d97-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85d97-131">Пример</span><span class="sxs-lookup"><span data-stu-id="85d97-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="85d97-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="85d97-132">Request</span></span>
<span data-ttu-id="85d97-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85d97-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="85d97-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="85d97-134">Response</span></span>
<span data-ttu-id="85d97-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="85d97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4870

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
}
```



