---
title: Get mdmWindowsInformationProtectionPolicy
description: Чтение свойств и связей объекта mdmWindowsInformationProtectionPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6193a8b4561c4b775fd5d5c752dbc1bbc18dc109
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401294"
---
# <a name="get-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="fb55a-103">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fb55a-103">Get mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="fb55a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb55a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fb55a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb55a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb55a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb55a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb55a-107">Чтение свойств и связей объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fb55a-107">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb55a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fb55a-108">Prerequisites</span></span>
<span data-ttu-id="fb55a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb55a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fb55a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb55a-111">Permission type</span></span>|<span data-ttu-id="fb55a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb55a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb55a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb55a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb55a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb55a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fb55a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb55a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb55a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb55a-116">Not supported.</span></span>|
|<span data-ttu-id="fb55a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb55a-117">Application</span></span>|<span data-ttu-id="fb55a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb55a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb55a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb55a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb55a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fb55a-120">Optional query parameters</span></span>
<span data-ttu-id="fb55a-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fb55a-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb55a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb55a-122">Request headers</span></span>
|<span data-ttu-id="fb55a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb55a-123">Header</span></span>|<span data-ttu-id="fb55a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fb55a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb55a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb55a-125">Authorization</span></span>|<span data-ttu-id="fb55a-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fb55a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb55a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fb55a-127">Accept</span></span>|<span data-ttu-id="fb55a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fb55a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb55a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb55a-129">Request body</span></span>
<span data-ttu-id="fb55a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb55a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb55a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb55a-131">Response</span></span>
<span data-ttu-id="fb55a-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fb55a-132">If successful, this method returns a `200 OK` response code and [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb55a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fb55a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb55a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb55a-134">Request</span></span>
<span data-ttu-id="fb55a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb55a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="fb55a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb55a-136">Response</span></span>
<span data-ttu-id="fb55a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fb55a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4414

{
  "value": {
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
}
```




