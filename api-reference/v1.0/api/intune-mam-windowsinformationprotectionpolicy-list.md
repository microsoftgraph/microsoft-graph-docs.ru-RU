---
title: Перечисление объектов WindowsInformationProtectionPolicy
description: Перечисление свойств и связей объектов windowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82e092133389b218d323d2dfd678ae764f6e76ae
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758054"
---
# <a name="list-windowsinformationprotectionpolicies"></a><span data-ttu-id="bfcaa-103">Перечисление объектов WindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="bfcaa-103">List windowsInformationProtectionPolicies</span></span>

<span data-ttu-id="bfcaa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfcaa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bfcaa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfcaa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfcaa-106">Перечисление свойств и связей объектов [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bfcaa-106">List properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfcaa-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bfcaa-107">Prerequisites</span></span>
<span data-ttu-id="bfcaa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfcaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfcaa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfcaa-110">Permission type</span></span>|<span data-ttu-id="bfcaa-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfcaa-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfcaa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfcaa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bfcaa-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfcaa-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bfcaa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfcaa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfcaa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfcaa-115">Not supported.</span></span>|
|<span data-ttu-id="bfcaa-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bfcaa-116">Application</span></span>|<span data-ttu-id="bfcaa-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfcaa-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfcaa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfcaa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="bfcaa-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bfcaa-119">Request headers</span></span>
|<span data-ttu-id="bfcaa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bfcaa-120">Header</span></span>|<span data-ttu-id="bfcaa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bfcaa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfcaa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfcaa-122">Authorization</span></span>|<span data-ttu-id="bfcaa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfcaa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfcaa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bfcaa-124">Accept</span></span>|<span data-ttu-id="bfcaa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bfcaa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfcaa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfcaa-126">Request body</span></span>
<span data-ttu-id="bfcaa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bfcaa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfcaa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfcaa-128">Response</span></span>
<span data-ttu-id="bfcaa-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bfcaa-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfcaa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bfcaa-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfcaa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfcaa-131">Request</span></span>
<span data-ttu-id="bfcaa-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfcaa-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="bfcaa-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfcaa-133">Response</span></span>
<span data-ttu-id="bfcaa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfcaa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5048

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
              "@odata.type": "microsoft.graph.ipRange"
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




