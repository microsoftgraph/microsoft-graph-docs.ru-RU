---
title: Перечисление объектов mdmWindowsInformationProtectionPolicy
description: Перечисление свойств и связей объектов mdmWindowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0433740e2bfd37de9596c873c786cf307fd97ff6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963032"
---
# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="82a7f-103">Перечисление объектов mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="82a7f-103">List mdmWindowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="82a7f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82a7f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82a7f-105">Перечисление свойств и связей объектов [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="82a7f-105">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82a7f-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="82a7f-106">Prerequisites</span></span>
<span data-ttu-id="82a7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82a7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82a7f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82a7f-109">Permission type</span></span>|<span data-ttu-id="82a7f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82a7f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82a7f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82a7f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82a7f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="82a7f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="82a7f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82a7f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82a7f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82a7f-114">Not supported.</span></span>|
|<span data-ttu-id="82a7f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82a7f-115">Application</span></span>|<span data-ttu-id="82a7f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82a7f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82a7f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82a7f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="82a7f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82a7f-118">Request headers</span></span>
|<span data-ttu-id="82a7f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82a7f-119">Header</span></span>|<span data-ttu-id="82a7f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="82a7f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82a7f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82a7f-121">Authorization</span></span>|<span data-ttu-id="82a7f-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82a7f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82a7f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="82a7f-123">Accept</span></span>|<span data-ttu-id="82a7f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="82a7f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82a7f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82a7f-125">Request body</span></span>
<span data-ttu-id="82a7f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82a7f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82a7f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="82a7f-127">Response</span></span>
<span data-ttu-id="82a7f-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="82a7f-128">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82a7f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="82a7f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="82a7f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="82a7f-130">Request</span></span>
<span data-ttu-id="82a7f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82a7f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="82a7f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="82a7f-132">Response</span></span>
<span data-ttu-id="82a7f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82a7f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4610

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



