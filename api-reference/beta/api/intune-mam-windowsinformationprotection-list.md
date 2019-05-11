---
title: Перечисление объектов windowsInformationProtection
description: Список свойств и связей объектов windowsInformationProtection.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2049f30fc460192161cb175a0c39b451b5067f3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33902922"
---
# <a name="list-windowsinformationprotections"></a><span data-ttu-id="95f62-103">Перечисление объектов windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="95f62-103">List windowsInformationProtections</span></span>

> <span data-ttu-id="95f62-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95f62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95f62-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95f62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95f62-106">Список свойств и связей объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="95f62-106">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95f62-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="95f62-107">Prerequisites</span></span>
<span data-ttu-id="95f62-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95f62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95f62-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95f62-110">Permission type</span></span>|<span data-ttu-id="95f62-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95f62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95f62-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95f62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95f62-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="95f62-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="95f62-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95f62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95f62-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95f62-115">Not supported.</span></span>|
|<span data-ttu-id="95f62-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95f62-116">Application</span></span>|<span data-ttu-id="95f62-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95f62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95f62-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95f62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="95f62-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95f62-119">Request headers</span></span>
|<span data-ttu-id="95f62-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95f62-120">Header</span></span>|<span data-ttu-id="95f62-121">Значение</span><span class="sxs-lookup"><span data-stu-id="95f62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95f62-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95f62-122">Authorization</span></span>|<span data-ttu-id="95f62-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95f62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95f62-124">Accept</span><span class="sxs-lookup"><span data-stu-id="95f62-124">Accept</span></span>|<span data-ttu-id="95f62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95f62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95f62-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95f62-126">Request body</span></span>
<span data-ttu-id="95f62-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95f62-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95f62-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="95f62-128">Response</span></span>
<span data-ttu-id="95f62-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="95f62-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95f62-130">Пример</span><span class="sxs-lookup"><span data-stu-id="95f62-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="95f62-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="95f62-131">Request</span></span>
<span data-ttu-id="95f62-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95f62-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="95f62-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="95f62-133">Response</span></span>
<span data-ttu-id="95f62-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95f62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4675

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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




