---
title: Перечисление объектов WindowsInformationProtectionPolicy
description: Перечисление свойств и связей объектов windowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a7ca65e4d95b02ae71476e47a3186086fc007f3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145733"
---
# <a name="list-windowsinformationprotectionpolicies"></a><span data-ttu-id="eda3d-103">Перечисление объектов WindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="eda3d-103">List windowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="eda3d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eda3d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eda3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eda3d-106">Перечисление свойств и связей объектов [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="eda3d-106">List properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eda3d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eda3d-107">Prerequisites</span></span>
<span data-ttu-id="eda3d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="eda3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eda3d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eda3d-110">Permission type</span></span>|<span data-ttu-id="eda3d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eda3d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eda3d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eda3d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eda3d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eda3d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="eda3d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eda3d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eda3d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda3d-115">Not supported.</span></span>|
|<span data-ttu-id="eda3d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eda3d-116">Application</span></span>|<span data-ttu-id="eda3d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda3d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eda3d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eda3d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="eda3d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eda3d-119">Request headers</span></span>
|<span data-ttu-id="eda3d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eda3d-120">Header</span></span>|<span data-ttu-id="eda3d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eda3d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eda3d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eda3d-122">Authorization</span></span>|<span data-ttu-id="eda3d-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="eda3d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eda3d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eda3d-124">Accept</span></span>|<span data-ttu-id="eda3d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eda3d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eda3d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eda3d-126">Request body</span></span>
<span data-ttu-id="eda3d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eda3d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eda3d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="eda3d-128">Response</span></span>
<span data-ttu-id="eda3d-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eda3d-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eda3d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="eda3d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="eda3d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eda3d-131">Request</span></span>
<span data-ttu-id="eda3d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eda3d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="eda3d-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="eda3d-133">Response</span></span>
<span data-ttu-id="eda3d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eda3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5232

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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




