---
title: Список Макосендпоинтпротектионконфигуратионс
description: Список свойств и связей объектов Макосендпоинтпротектионконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b6f0efb78bf5a9f98124d7eb85b52ff93101a15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066014"
---
# <a name="list-macosendpointprotectionconfigurations"></a><span data-ttu-id="647e8-103">Список Макосендпоинтпротектионконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="647e8-103">List macOSEndpointProtectionConfigurations</span></span>

<span data-ttu-id="647e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="647e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="647e8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="647e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="647e8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="647e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="647e8-107">Список свойств и связей объектов [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="647e8-107">List properties and relationships of the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="647e8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="647e8-108">Prerequisites</span></span>
<span data-ttu-id="647e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="647e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="647e8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="647e8-111">Permission type</span></span>|<span data-ttu-id="647e8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="647e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="647e8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="647e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="647e8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="647e8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="647e8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="647e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="647e8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="647e8-116">Not supported.</span></span>|
|<span data-ttu-id="647e8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="647e8-117">Application</span></span>|<span data-ttu-id="647e8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="647e8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="647e8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="647e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="647e8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="647e8-120">Request headers</span></span>
|<span data-ttu-id="647e8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="647e8-121">Header</span></span>|<span data-ttu-id="647e8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="647e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="647e8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="647e8-123">Authorization</span></span>|<span data-ttu-id="647e8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="647e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="647e8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="647e8-125">Accept</span></span>|<span data-ttu-id="647e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="647e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="647e8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="647e8-127">Request body</span></span>
<span data-ttu-id="647e8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="647e8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="647e8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="647e8-129">Response</span></span>
<span data-ttu-id="647e8-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="647e8-130">If successful, this method returns a `200 OK` response code and a collection of [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="647e8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="647e8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="647e8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="647e8-132">Request</span></span>
<span data-ttu-id="647e8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="647e8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="647e8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="647e8-134">Response</span></span>
<span data-ttu-id="647e8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="647e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
      "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "gatekeeperAllowedAppSource": "macAppStore",
      "gatekeeperBlockOverride": true,
      "firewallEnabled": true,
      "firewallBlockAllIncoming": true,
      "firewallEnableStealthMode": true,
      "firewallApplications": [
        {
          "@odata.type": "microsoft.graph.macOSFirewallApplication",
          "bundleId": "Bundle Id value",
          "allowsIncomingConnections": true
        }
      ],
      "fileVaultEnabled": true,
      "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
      "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
      "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
      "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
      "fileVaultAllowDeferralUntilSignOut": true,
      "fileVaultNumberOfTimesUserCanIgnore": 3,
      "fileVaultDisablePromptAtSignOut": true,
      "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
      "fileVaultHidePersonalRecoveryKey": true,
      "advancedThreatProtectionRealTime": "enabled",
      "advancedThreatProtectionCloudDelivered": "enabled",
      "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
      "advancedThreatProtectionDiagnosticDataCollection": "enabled",
      "advancedThreatProtectionExcludedFolders": [
        "Advanced Threat Protection Excluded Folders value"
      ],
      "advancedThreatProtectionExcludedFiles": [
        "Advanced Threat Protection Excluded Files value"
      ],
      "advancedThreatProtectionExcludedExtensions": [
        "Advanced Threat Protection Excluded Extensions value"
      ],
      "advancedThreatProtectionExcludedProcesses": [
        "Advanced Threat Protection Excluded Processes value"
      ]
    }
  ]
}
```






