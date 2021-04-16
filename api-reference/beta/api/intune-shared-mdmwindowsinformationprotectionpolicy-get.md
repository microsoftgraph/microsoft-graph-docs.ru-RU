---
title: Get mdmWindowsInformationProtectionPolicy
description: Чтение свойств и связей объекта mdmWindowsInformationProtectionPolicy.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca55cae17366d5c0ffd79e4e70ffbd66b59417c7
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865490"
---
# <a name="get-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="3ea7c-103">Get mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="3ea7c-103">Get mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="3ea7c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ea7c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ea7c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ea7c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ea7c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ea7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ea7c-107">Чтение свойств и связей объекта [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3ea7c-107">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ea7c-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea7c-108">Prerequisites</span></span>
<span data-ttu-id="3ea7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ea7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ea7c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea7c-111">Permission type</span></span>|<span data-ttu-id="3ea7c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ea7c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ea7c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ea7c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3ea7c-114">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="3ea7c-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="3ea7c-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ea7c-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="3ea7c-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="3ea7c-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="3ea7c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ea7c-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3ea7c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ea7c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ea7c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ea7c-119">Not supported.</span></span>|
|<span data-ttu-id="3ea7c-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3ea7c-120">Application</span></span>||
| <span data-ttu-id="3ea7c-121">&nbsp; &nbsp; **Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="3ea7c-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="3ea7c-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ea7c-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="3ea7c-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="3ea7c-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="3ea7c-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ea7c-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ea7c-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ea7c-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ea7c-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3ea7c-126">Optional query parameters</span></span>
<span data-ttu-id="3ea7c-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3ea7c-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ea7c-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ea7c-128">Request headers</span></span>
|<span data-ttu-id="3ea7c-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ea7c-129">Header</span></span>|<span data-ttu-id="3ea7c-130">Значение</span><span class="sxs-lookup"><span data-stu-id="3ea7c-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ea7c-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ea7c-131">Authorization</span></span>|<span data-ttu-id="3ea7c-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ea7c-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ea7c-133">Accept</span><span class="sxs-lookup"><span data-stu-id="3ea7c-133">Accept</span></span>|<span data-ttu-id="3ea7c-134">application/json</span><span class="sxs-lookup"><span data-stu-id="3ea7c-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ea7c-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ea7c-135">Request body</span></span>
<span data-ttu-id="3ea7c-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ea7c-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ea7c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea7c-137">Response</span></span>
<span data-ttu-id="3ea7c-138">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3ea7c-138">If successful, this method returns a `200 OK` response code and [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ea7c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="3ea7c-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ea7c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ea7c-140">Request</span></span>
<span data-ttu-id="3ea7c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ea7c-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="3ea7c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea7c-142">Response</span></span>
<span data-ttu-id="3ea7c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ea7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







