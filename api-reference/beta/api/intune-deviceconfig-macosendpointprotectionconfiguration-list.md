---
title: Список Макосендпоинтпротектионконфигуратионс
description: Список свойств и связей объектов Макосендпоинтпротектионконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b424e5dab85fcdeaca67adc5ddba551149be5eb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42746670"
---
# <a name="list-macosendpointprotectionconfigurations"></a><span data-ttu-id="18340-103">Список Макосендпоинтпротектионконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="18340-103">List macOSEndpointProtectionConfigurations</span></span>

> <span data-ttu-id="18340-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18340-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18340-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18340-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18340-106">Список свойств и связей объектов [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="18340-106">List properties and relationships of the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18340-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18340-107">Prerequisites</span></span>
<span data-ttu-id="18340-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18340-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18340-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18340-110">Permission type</span></span>|<span data-ttu-id="18340-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18340-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18340-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18340-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18340-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18340-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="18340-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18340-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18340-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18340-115">Not supported.</span></span>|
|<span data-ttu-id="18340-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="18340-116">Application</span></span>|<span data-ttu-id="18340-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18340-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18340-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18340-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18340-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18340-119">Request headers</span></span>
|<span data-ttu-id="18340-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18340-120">Header</span></span>|<span data-ttu-id="18340-121">Значение</span><span class="sxs-lookup"><span data-stu-id="18340-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18340-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18340-122">Authorization</span></span>|<span data-ttu-id="18340-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18340-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18340-124">Accept</span><span class="sxs-lookup"><span data-stu-id="18340-124">Accept</span></span>|<span data-ttu-id="18340-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18340-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18340-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18340-126">Request body</span></span>
<span data-ttu-id="18340-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18340-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18340-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="18340-128">Response</span></span>
<span data-ttu-id="18340-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18340-129">If successful, this method returns a `200 OK` response code and a collection of [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18340-130">Пример</span><span class="sxs-lookup"><span data-stu-id="18340-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="18340-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="18340-131">Request</span></span>
<span data-ttu-id="18340-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18340-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="18340-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="18340-133">Response</span></span>
<span data-ttu-id="18340-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18340-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




