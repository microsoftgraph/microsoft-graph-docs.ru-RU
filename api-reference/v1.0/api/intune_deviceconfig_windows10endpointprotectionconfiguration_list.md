# <a name="list-windows10endpointprotectionconfigurations"></a><span data-ttu-id="4fe00-101">Перечисление объектов windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="4fe00-101">List windows10EndpointProtectionConfigurations</span></span>

> <span data-ttu-id="4fe00-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4fe00-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fe00-103">Перечисление свойств и связей объектов [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fe00-103">List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4fe00-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4fe00-104">Prerequisites</span></span>
<span data-ttu-id="4fe00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4fe00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4fe00-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fe00-107">Permission type</span></span>|<span data-ttu-id="4fe00-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fe00-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fe00-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fe00-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4fe00-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fe00-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4fe00-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fe00-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fe00-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fe00-112">Not supported.</span></span>|
|<span data-ttu-id="4fe00-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fe00-113">Application</span></span>|<span data-ttu-id="4fe00-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fe00-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fe00-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fe00-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4fe00-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fe00-116">Request headers</span></span>
|<span data-ttu-id="4fe00-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4fe00-117">Header</span></span>|<span data-ttu-id="4fe00-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4fe00-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fe00-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fe00-119">Authorization</span></span>|<span data-ttu-id="4fe00-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="4fe00-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fe00-121">Принять</span><span class="sxs-lookup"><span data-stu-id="4fe00-121">Accept</span></span>|<span data-ttu-id="4fe00-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4fe00-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fe00-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4fe00-123">Request body</span></span>
<span data-ttu-id="4fe00-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4fe00-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fe00-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fe00-125">Response</span></span>
<span data-ttu-id="4fe00-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4fe00-126">If successful, this method returns a `200 OK` response code and a collection of [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fe00-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4fe00-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="4fe00-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fe00-128">Request</span></span>
<span data-ttu-id="4fe00-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fe00-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4fe00-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4fe00-130">Response</span></span>
<span data-ttu-id="4fe00-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fe00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4834

{
  "value": [
    {
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
  ]
}
```








