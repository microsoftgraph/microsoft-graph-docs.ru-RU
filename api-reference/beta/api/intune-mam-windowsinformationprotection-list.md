---
title: Перечисление объектов windowsInformationProtection
description: Список свойств и связей объектов windowsInformationProtection.
author: tfitzmac
ms.openlocfilehash: 34491a305124cf4d9f31ed6dcb1529f2c7b88e5b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348177"
---
# <a name="list-windowsinformationprotections"></a><span data-ttu-id="dc88a-103">Перечисление объектов windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="dc88a-103">List windowsInformationProtections</span></span>

> <span data-ttu-id="dc88a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc88a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc88a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc88a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc88a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dc88a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc88a-107">Список свойств и связей объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md).</span><span class="sxs-lookup"><span data-stu-id="dc88a-107">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc88a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dc88a-108">Prerequisites</span></span>
<span data-ttu-id="dc88a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc88a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc88a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc88a-111">Permission type</span></span>|<span data-ttu-id="dc88a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc88a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc88a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc88a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc88a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc88a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dc88a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc88a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc88a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc88a-116">Not supported.</span></span>|
|<span data-ttu-id="dc88a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc88a-117">Application</span></span>|<span data-ttu-id="dc88a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc88a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc88a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc88a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="dc88a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc88a-120">Request headers</span></span>
|<span data-ttu-id="dc88a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc88a-121">Header</span></span>|<span data-ttu-id="dc88a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dc88a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc88a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc88a-123">Authorization</span></span>|<span data-ttu-id="dc88a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dc88a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc88a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dc88a-125">Accept</span></span>|<span data-ttu-id="dc88a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc88a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc88a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc88a-127">Request body</span></span>
<span data-ttu-id="dc88a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc88a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc88a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc88a-129">Response</span></span>
<span data-ttu-id="dc88a-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dc88a-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc88a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dc88a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc88a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc88a-132">Request</span></span>
<span data-ttu-id="dc88a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc88a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="dc88a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc88a-134">Response</span></span>
<span data-ttu-id="dc88a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dc88a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





