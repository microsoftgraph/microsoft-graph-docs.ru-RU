---
title: Перечисление объектов windowsInformationProtection
description: Список свойств и связей объектов windowsInformationProtection.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39d1be555c6e853f6a6ab02b9071109bd2899249
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512876"
---
# <a name="list-windowsinformationprotections"></a><span data-ttu-id="f4e14-103">Перечисление объектов windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="f4e14-103">List windowsInformationProtections</span></span>

<span data-ttu-id="f4e14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4e14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4e14-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4e14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4e14-106">Список свойств и связей объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="f4e14-106">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4e14-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f4e14-107">Prerequisites</span></span>
<span data-ttu-id="f4e14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4e14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4e14-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4e14-110">Permission type</span></span>|<span data-ttu-id="f4e14-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4e14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4e14-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4e14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4e14-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4e14-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f4e14-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4e14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4e14-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4e14-115">Not supported.</span></span>|
|<span data-ttu-id="f4e14-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4e14-116">Application</span></span>|<span data-ttu-id="f4e14-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4e14-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4e14-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4e14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f4e14-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f4e14-119">Request headers</span></span>
|<span data-ttu-id="f4e14-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4e14-120">Header</span></span>|<span data-ttu-id="f4e14-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f4e14-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4e14-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4e14-122">Authorization</span></span>|<span data-ttu-id="f4e14-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4e14-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4e14-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f4e14-124">Accept</span></span>|<span data-ttu-id="f4e14-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4e14-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4e14-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4e14-126">Request body</span></span>
<span data-ttu-id="f4e14-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4e14-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4e14-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4e14-128">Response</span></span>
<span data-ttu-id="f4e14-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f4e14-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4e14-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f4e14-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4e14-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4e14-131">Request</span></span>
<span data-ttu-id="f4e14-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4e14-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="f4e14-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4e14-133">Response</span></span>
<span data-ttu-id="f4e14-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4e14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4601

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "ca339419-9419-ca33-1994-33ca199433ca",
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
      "isAssigned": true
    }
  ]
}
```




