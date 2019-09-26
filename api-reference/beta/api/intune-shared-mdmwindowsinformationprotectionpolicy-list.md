---
title: Перечисление объектов mdmWindowsInformationProtectionPolicy
description: Перечисление свойств и связей объектов mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1025238efc379a78af837ad8ee27ab395686ae8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201017"
---
# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="c3b1a-103">Перечисление объектов mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c3b1a-103">List mdmWindowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="c3b1a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3b1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3b1a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3b1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3b1a-106">Перечисление свойств и связей объектов [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c3b1a-106">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3b1a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c3b1a-107">Prerequisites</span></span>
<span data-ttu-id="c3b1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3b1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3b1a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3b1a-110">Permission type</span></span>|<span data-ttu-id="c3b1a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3b1a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3b1a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3b1a-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c3b1a-113">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="c3b1a-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c3b1a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3b1a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c3b1a-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="c3b1a-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c3b1a-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3b1a-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c3b1a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3b1a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3b1a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3b1a-118">Not supported.</span></span>|
|<span data-ttu-id="c3b1a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3b1a-119">Application</span></span>||
| <span data-ttu-id="c3b1a-120">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="c3b1a-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="c3b1a-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3b1a-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="c3b1a-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="c3b1a-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c3b1a-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3b1a-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3b1a-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3b1a-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c3b1a-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3b1a-125">Request headers</span></span>
|<span data-ttu-id="c3b1a-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3b1a-126">Header</span></span>|<span data-ttu-id="c3b1a-127">Значение</span><span class="sxs-lookup"><span data-stu-id="c3b1a-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3b1a-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3b1a-128">Authorization</span></span>|<span data-ttu-id="c3b1a-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3b1a-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3b1a-130">Accept</span><span class="sxs-lookup"><span data-stu-id="c3b1a-130">Accept</span></span>|<span data-ttu-id="c3b1a-131">application/json</span><span class="sxs-lookup"><span data-stu-id="c3b1a-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3b1a-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3b1a-132">Request body</span></span>
<span data-ttu-id="c3b1a-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3b1a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3b1a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3b1a-134">Response</span></span>
<span data-ttu-id="c3b1a-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c3b1a-135">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3b1a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c3b1a-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3b1a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3b1a-137">Request</span></span>
<span data-ttu-id="c3b1a-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3b1a-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="c3b1a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3b1a-139">Response</span></span>
<span data-ttu-id="c3b1a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3b1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4684

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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




