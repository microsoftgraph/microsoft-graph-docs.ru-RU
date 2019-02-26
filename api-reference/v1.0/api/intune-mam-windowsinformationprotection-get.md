---
title: Получение windowsInformationProtection
description: Чтение свойств и связей объекта windowsInformationProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76a591ac19fb82a54f7efb7c13399dba1dcaf4a1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262582"
---
# <a name="get-windowsinformationprotection"></a><span data-ttu-id="96d2a-103">Получение windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="96d2a-103">Get windowsInformationProtection</span></span>

> <span data-ttu-id="96d2a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96d2a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96d2a-105">Чтение свойств и связей объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="96d2a-105">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96d2a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="96d2a-106">Prerequisites</span></span>
<span data-ttu-id="96d2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="96d2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="96d2a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96d2a-109">Permission type</span></span>|<span data-ttu-id="96d2a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96d2a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96d2a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96d2a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96d2a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="96d2a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="96d2a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96d2a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96d2a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96d2a-114">Not supported.</span></span>|
|<span data-ttu-id="96d2a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96d2a-115">Application</span></span>|<span data-ttu-id="96d2a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96d2a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96d2a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96d2a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96d2a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="96d2a-118">Optional query parameters</span></span>
<span data-ttu-id="96d2a-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="96d2a-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96d2a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96d2a-120">Request headers</span></span>
|<span data-ttu-id="96d2a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96d2a-121">Header</span></span>|<span data-ttu-id="96d2a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="96d2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96d2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96d2a-123">Authorization</span></span>|<span data-ttu-id="96d2a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="96d2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96d2a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96d2a-125">Accept</span></span>|<span data-ttu-id="96d2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96d2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96d2a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96d2a-127">Request body</span></span>
<span data-ttu-id="96d2a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96d2a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96d2a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="96d2a-129">Response</span></span>
<span data-ttu-id="96d2a-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="96d2a-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96d2a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="96d2a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="96d2a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="96d2a-132">Request</span></span>
<span data-ttu-id="96d2a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96d2a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="96d2a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="96d2a-134">Response</span></span>
<span data-ttu-id="96d2a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="96d2a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



