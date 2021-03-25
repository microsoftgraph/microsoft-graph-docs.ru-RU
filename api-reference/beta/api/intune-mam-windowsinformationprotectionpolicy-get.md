---
title: Получение объекта windowsInformationProtectionPolicy
description: Чтение свойств и связей объекта windowsInformationProtectionPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a311e6a7fb7e72b5bdfb0fd1459d9230090f77a8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153113"
---
# <a name="get-windowsinformationprotectionpolicy"></a><span data-ttu-id="b3969-103">Получение объекта windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b3969-103">Get windowsInformationProtectionPolicy</span></span>

<span data-ttu-id="b3969-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3969-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3969-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3969-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3969-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3969-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3969-107">Чтение свойств и связей объекта [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b3969-107">Read properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3969-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b3969-108">Prerequisites</span></span>
<span data-ttu-id="b3969-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3969-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3969-111">Permission type</span></span>|<span data-ttu-id="b3969-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3969-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3969-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3969-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3969-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3969-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3969-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3969-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3969-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3969-116">Not supported.</span></span>|
|<span data-ttu-id="b3969-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b3969-117">Application</span></span>|<span data-ttu-id="b3969-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3969-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3969-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3969-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3969-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b3969-120">Optional query parameters</span></span>
<span data-ttu-id="b3969-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b3969-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3969-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3969-122">Request headers</span></span>
|<span data-ttu-id="b3969-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3969-123">Header</span></span>|<span data-ttu-id="b3969-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b3969-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3969-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3969-125">Authorization</span></span>|<span data-ttu-id="b3969-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3969-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3969-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b3969-127">Accept</span></span>|<span data-ttu-id="b3969-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b3969-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3969-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3969-129">Request body</span></span>
<span data-ttu-id="b3969-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3969-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3969-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3969-131">Response</span></span>
<span data-ttu-id="b3969-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b3969-132">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3969-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b3969-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3969-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3969-134">Request</span></span>
<span data-ttu-id="b3969-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3969-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="b3969-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3969-136">Response</span></span>
<span data-ttu-id="b3969-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3969-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4832

{
  "value": {
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
}
```




