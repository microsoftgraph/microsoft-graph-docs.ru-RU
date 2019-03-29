---
title: Get windows10EndpointProtectionConfiguration
description: Чтение свойств и связей объекта windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f63c53b1a68ad8d4397243ed6d0350a7bcbea258
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965531"
---
# <a name="get-windows10endpointprotectionconfiguration"></a><span data-ttu-id="19d5a-103">Get windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="19d5a-103">Get windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="19d5a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19d5a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19d5a-105">Чтение свойств и связей объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19d5a-105">Read properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19d5a-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="19d5a-106">Prerequisites</span></span>
<span data-ttu-id="19d5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19d5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19d5a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19d5a-109">Permission type</span></span>|<span data-ttu-id="19d5a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19d5a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19d5a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19d5a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="19d5a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="19d5a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="19d5a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19d5a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19d5a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19d5a-114">Not supported.</span></span>|
|<span data-ttu-id="19d5a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19d5a-115">Application</span></span>|<span data-ttu-id="19d5a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19d5a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19d5a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19d5a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19d5a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19d5a-118">Optional query parameters</span></span>
<span data-ttu-id="19d5a-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="19d5a-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19d5a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19d5a-120">Request headers</span></span>
|<span data-ttu-id="19d5a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19d5a-121">Header</span></span>|<span data-ttu-id="19d5a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="19d5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19d5a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19d5a-123">Authorization</span></span>|<span data-ttu-id="19d5a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19d5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19d5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="19d5a-125">Accept</span></span>|<span data-ttu-id="19d5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19d5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19d5a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19d5a-127">Request body</span></span>
<span data-ttu-id="19d5a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19d5a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19d5a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="19d5a-129">Response</span></span>
<span data-ttu-id="19d5a-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19d5a-130">If successful, this method returns a `200 OK` response code and [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19d5a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="19d5a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="19d5a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="19d5a-132">Request</span></span>
<span data-ttu-id="19d5a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19d5a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="19d5a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="19d5a-134">Response</span></span>
<span data-ttu-id="19d5a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19d5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4628

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
    "id": "09709403-9403-0970-0394-700903947009",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "firewallBlockStatefulFTP": true,
    "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
    "firewallPreSharedKeyEncodingMethod": "none",
    "firewallIPSecExemptionsAllowNeighborDiscovery": true,
    "firewallIPSecExemptionsAllowICMP": true,
    "firewallIPSecExemptionsAllowRouterDiscovery": true,
    "firewallIPSecExemptionsAllowDHCP": true,
    "firewallCertificateRevocationListCheckMethod": "none",
    "firewallMergeKeyingModuleSettings": true,
    "firewallPacketQueueingMethod": "disabled",
    "firewallProfileDomain": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeBlocked": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "policyRulesFromGroupPolicyMerged": true
    },
    "firewallProfilePublic": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeBlocked": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "policyRulesFromGroupPolicyMerged": true
    },
    "firewallProfilePrivate": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeBlocked": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "policyRulesFromGroupPolicyMerged": true
    },
    "defenderAttackSurfaceReductionExcludedPaths": [
      "Defender Attack Surface Reduction Excluded Paths value"
    ],
    "defenderGuardedFoldersAllowedAppPaths": [
      "Defender Guarded Folders Allowed App Paths value"
    ],
    "defenderAdditionalGuardedFolders": [
      "Defender Additional Guarded Folders value"
    ],
    "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
    "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
    "defenderSecurityCenterBlockExploitProtectionOverride": true,
    "appLockerApplicationControl": "enforceComponentsAndStoreApps",
    "smartScreenEnableInShell": true,
    "smartScreenBlockOverrideForFiles": true,
    "applicationGuardEnabled": true,
    "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
    "applicationGuardBlockNonEnterpriseContent": true,
    "applicationGuardAllowPersistence": true,
    "applicationGuardForceAuditing": true,
    "applicationGuardBlockClipboardSharing": "blockBoth",
    "applicationGuardAllowPrintToPDF": true,
    "applicationGuardAllowPrintToXPS": true,
    "applicationGuardAllowPrintToLocalPrinters": true,
    "applicationGuardAllowPrintToNetworkPrinters": true,
    "bitLockerDisableWarningForOtherDiskEncryption": true,
    "bitLockerEnableStorageCardEncryptionOnMobile": true,
    "bitLockerEncryptDevice": true,
    "bitLockerRemovableDrivePolicy": {
      "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
      "encryptionMethod": "aesCbc256",
      "requireEncryptionForWriteAccess": true,
      "blockCrossOrganizationWriteAccess": true
    }
  }
}
```



