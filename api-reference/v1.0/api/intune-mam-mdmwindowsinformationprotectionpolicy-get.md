---
title: Get mdmWindowsInformationProtectionPolicy
description: Чтение свойств и связей объекта mdmWindowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bd72742b2aa3a32adfa3b24fafb793178043f23e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938113"
---
# <a name="get-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="fb806-103">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fb806-103">Get mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="fb806-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fb806-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb806-105">Чтение свойств и связей объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fb806-105">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb806-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fb806-106">Prerequisites</span></span>
<span data-ttu-id="fb806-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb806-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb806-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb806-109">Permission type</span></span>|<span data-ttu-id="fb806-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb806-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb806-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb806-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb806-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb806-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fb806-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb806-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb806-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb806-114">Not supported.</span></span>|
|<span data-ttu-id="fb806-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb806-115">Application</span></span>|<span data-ttu-id="fb806-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb806-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb806-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb806-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb806-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fb806-118">Optional query parameters</span></span>
<span data-ttu-id="fb806-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fb806-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fb806-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb806-120">Request headers</span></span>
|<span data-ttu-id="fb806-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb806-121">Header</span></span>|<span data-ttu-id="fb806-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb806-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb806-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb806-123">Authorization</span></span>|<span data-ttu-id="fb806-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fb806-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb806-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb806-125">Accept</span></span>|<span data-ttu-id="fb806-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb806-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb806-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fb806-127">Request body</span></span>
<span data-ttu-id="fb806-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb806-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb806-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb806-129">Response</span></span>
<span data-ttu-id="fb806-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fb806-130">If successful, this method returns a `200 OK` response code and [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb806-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fb806-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb806-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb806-132">Request</span></span>
<span data-ttu-id="fb806-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb806-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="fb806-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb806-134">Response</span></span>
<span data-ttu-id="fb806-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fb806-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4346

{
  "value": {
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
}
```



