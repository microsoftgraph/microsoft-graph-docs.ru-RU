---
title: Перечисление объектов windowsInformationProtection
description: Список свойств и связей объектов windowsInformationProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4dd7fecbf40eb277fe0960f5a3e678f94772cb34
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752562"
---
# <a name="list-windowsinformationprotections"></a><span data-ttu-id="1df07-103">Перечисление объектов windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="1df07-103">List windowsInformationProtections</span></span>

<span data-ttu-id="1df07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1df07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1df07-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1df07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1df07-106">Список свойств и связей объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="1df07-106">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1df07-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1df07-107">Prerequisites</span></span>
<span data-ttu-id="1df07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1df07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1df07-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1df07-110">Permission type</span></span>|<span data-ttu-id="1df07-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1df07-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1df07-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1df07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1df07-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1df07-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1df07-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1df07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1df07-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1df07-115">Not supported.</span></span>|
|<span data-ttu-id="1df07-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1df07-116">Application</span></span>|<span data-ttu-id="1df07-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1df07-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1df07-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1df07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="1df07-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1df07-119">Request headers</span></span>
|<span data-ttu-id="1df07-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1df07-120">Header</span></span>|<span data-ttu-id="1df07-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1df07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1df07-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1df07-122">Authorization</span></span>|<span data-ttu-id="1df07-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1df07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1df07-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1df07-124">Accept</span></span>|<span data-ttu-id="1df07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1df07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1df07-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1df07-126">Request body</span></span>
<span data-ttu-id="1df07-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1df07-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1df07-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1df07-128">Response</span></span>
<span data-ttu-id="1df07-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1df07-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1df07-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1df07-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1df07-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1df07-131">Request</span></span>
<span data-ttu-id="1df07-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1df07-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="1df07-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1df07-133">Response</span></span>
<span data-ttu-id="1df07-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1df07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4491

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
      "isAssigned": true
    }
  ]
}
```




