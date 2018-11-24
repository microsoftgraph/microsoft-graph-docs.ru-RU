# <a name="get-windows10endpointprotectionconfiguration"></a><span data-ttu-id="51ec0-101">Get windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="51ec0-101">Get windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="51ec0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51ec0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51ec0-103">Чтение свойств и связей объекта [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51ec0-103">Read properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51ec0-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="51ec0-104">Prerequisites</span></span>
<span data-ttu-id="51ec0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="51ec0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="51ec0-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51ec0-107">Permission type</span></span>|<span data-ttu-id="51ec0-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51ec0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51ec0-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51ec0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="51ec0-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51ec0-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="51ec0-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51ec0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51ec0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51ec0-112">Not supported.</span></span>|
|<span data-ttu-id="51ec0-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51ec0-113">Application</span></span>|<span data-ttu-id="51ec0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51ec0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51ec0-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51ec0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51ec0-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51ec0-116">Optional query parameters</span></span>
<span data-ttu-id="51ec0-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51ec0-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51ec0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51ec0-118">Request headers</span></span>
|<span data-ttu-id="51ec0-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51ec0-119">Header</span></span>|<span data-ttu-id="51ec0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="51ec0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51ec0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51ec0-121">Authorization</span></span>|<span data-ttu-id="51ec0-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51ec0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51ec0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="51ec0-123">Accept</span></span>|<span data-ttu-id="51ec0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51ec0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51ec0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51ec0-125">Request body</span></span>
<span data-ttu-id="51ec0-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51ec0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51ec0-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="51ec0-127">Response</span></span>
<span data-ttu-id="51ec0-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="51ec0-128">If successful, this method returns a `200 OK` response code and [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51ec0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="51ec0-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="51ec0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="51ec0-130">Request</span></span>
<span data-ttu-id="51ec0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51ec0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="51ec0-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="51ec0-132">Response</span></span>
<span data-ttu-id="51ec0-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51ec0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



