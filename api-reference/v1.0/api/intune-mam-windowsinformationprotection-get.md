---
title: Получение windowsInformationProtection
description: Чтение свойств и связей объекта windowsInformationProtection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2634dc67096a0ce00d0992e4285a98c8544d0f2e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758068"
---
# <a name="get-windowsinformationprotection"></a><span data-ttu-id="0c6fb-103">Получение windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="0c6fb-103">Get windowsInformationProtection</span></span>

<span data-ttu-id="0c6fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c6fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c6fb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c6fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c6fb-106">Чтение свойств и связей объекта [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="0c6fb-106">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c6fb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0c6fb-107">Prerequisites</span></span>
<span data-ttu-id="0c6fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c6fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c6fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c6fb-110">Permission type</span></span>|<span data-ttu-id="0c6fb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c6fb-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c6fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c6fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c6fb-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c6fb-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c6fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c6fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c6fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c6fb-115">Not supported.</span></span>|
|<span data-ttu-id="0c6fb-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c6fb-116">Application</span></span>|<span data-ttu-id="0c6fb-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c6fb-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c6fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c6fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c6fb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0c6fb-119">Optional query parameters</span></span>
<span data-ttu-id="0c6fb-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0c6fb-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c6fb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c6fb-121">Request headers</span></span>
|<span data-ttu-id="0c6fb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c6fb-122">Header</span></span>|<span data-ttu-id="0c6fb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0c6fb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c6fb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c6fb-124">Authorization</span></span>|<span data-ttu-id="0c6fb-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c6fb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c6fb-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0c6fb-126">Accept</span></span>|<span data-ttu-id="0c6fb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0c6fb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c6fb-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c6fb-128">Request body</span></span>
<span data-ttu-id="0c6fb-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c6fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c6fb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c6fb-130">Response</span></span>
<span data-ttu-id="0c6fb-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0c6fb-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c6fb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0c6fb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c6fb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c6fb-133">Request</span></span>
<span data-ttu-id="0c6fb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c6fb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="0c6fb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c6fb-135">Response</span></span>
<span data-ttu-id="0c6fb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c6fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4231

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
}
```




