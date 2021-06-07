---
title: Get windows10EndpointProtectionConfiguration
description: Чтение свойств и связей объекта windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cb138e10a85719d74e78b206ddb40f2d81830ba
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753827"
---
# <a name="get-windows10endpointprotectionconfiguration"></a><span data-ttu-id="bf7ae-103">Get windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="bf7ae-103">Get windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="bf7ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf7ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf7ae-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf7ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf7ae-106">Чтение свойств и связей объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bf7ae-106">Read properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf7ae-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bf7ae-107">Prerequisites</span></span>
<span data-ttu-id="bf7ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf7ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf7ae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf7ae-110">Permission type</span></span>|<span data-ttu-id="bf7ae-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf7ae-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf7ae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf7ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf7ae-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf7ae-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf7ae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf7ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf7ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf7ae-115">Not supported.</span></span>|
|<span data-ttu-id="bf7ae-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bf7ae-116">Application</span></span>|<span data-ttu-id="bf7ae-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf7ae-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf7ae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf7ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf7ae-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bf7ae-119">Optional query parameters</span></span>
<span data-ttu-id="bf7ae-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bf7ae-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf7ae-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf7ae-121">Request headers</span></span>
|<span data-ttu-id="bf7ae-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf7ae-122">Header</span></span>|<span data-ttu-id="bf7ae-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bf7ae-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf7ae-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf7ae-124">Authorization</span></span>|<span data-ttu-id="bf7ae-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf7ae-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf7ae-126">Accept</span><span class="sxs-lookup"><span data-stu-id="bf7ae-126">Accept</span></span>|<span data-ttu-id="bf7ae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bf7ae-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf7ae-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf7ae-128">Request body</span></span>
<span data-ttu-id="bf7ae-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf7ae-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf7ae-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf7ae-130">Response</span></span>
<span data-ttu-id="bf7ae-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bf7ae-131">If successful, this method returns a `200 OK` response code and [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf7ae-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bf7ae-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf7ae-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf7ae-133">Request</span></span>
<span data-ttu-id="bf7ae-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf7ae-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bf7ae-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf7ae-135">Response</span></span>
<span data-ttu-id="bf7ae-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf7ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




