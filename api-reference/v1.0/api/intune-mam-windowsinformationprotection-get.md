---
title: Получение windowsInformationProtection
description: Чтение свойств и связей объекта windowsInformationProtection.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a3f1e77bc5d9a2c0f43d987b98fc1798e416f547
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871577"
---
# <a name="get-windowsinformationprotection"></a><span data-ttu-id="fcff6-103">Получение windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="fcff6-103">Get windowsInformationProtection</span></span>

> <span data-ttu-id="fcff6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fcff6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcff6-105">Чтение свойств и связей объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="fcff6-105">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fcff6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fcff6-106">Prerequisites</span></span>
<span data-ttu-id="fcff6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcff6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcff6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcff6-109">Permission type</span></span>|<span data-ttu-id="fcff6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcff6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcff6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcff6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fcff6-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcff6-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fcff6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcff6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcff6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcff6-114">Not supported.</span></span>|
|<span data-ttu-id="fcff6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcff6-115">Application</span></span>|<span data-ttu-id="fcff6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcff6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcff6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcff6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcff6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fcff6-118">Optional query parameters</span></span>
<span data-ttu-id="fcff6-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fcff6-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fcff6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcff6-120">Request headers</span></span>
|<span data-ttu-id="fcff6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcff6-121">Header</span></span>|<span data-ttu-id="fcff6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fcff6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcff6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcff6-123">Authorization</span></span>|<span data-ttu-id="fcff6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fcff6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcff6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fcff6-125">Accept</span></span>|<span data-ttu-id="fcff6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcff6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcff6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fcff6-127">Request body</span></span>
<span data-ttu-id="fcff6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcff6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcff6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcff6-129">Response</span></span>
<span data-ttu-id="fcff6-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fcff6-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcff6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fcff6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fcff6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcff6-132">Request</span></span>
<span data-ttu-id="fcff6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcff6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="fcff6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcff6-134">Response</span></span>
<span data-ttu-id="fcff6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fcff6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4337

{
  "value": {
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
}
```



