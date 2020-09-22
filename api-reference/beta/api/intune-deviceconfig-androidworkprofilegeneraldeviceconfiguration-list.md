---
title: Список Андроидворкпрофилеженералдевицеконфигуратионс
description: Список свойств и связей объектов androidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4faae483a8e55cbe3408ea52f7ee7c7b8e83969d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990300"
---
# <a name="list-androidworkprofilegeneraldeviceconfigurations"></a><span data-ttu-id="7f9cd-103">Список Андроидворкпрофилеженералдевицеконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="7f9cd-103">List androidWorkProfileGeneralDeviceConfigurations</span></span>

<span data-ttu-id="7f9cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f9cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f9cd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f9cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f9cd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f9cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f9cd-107">Список свойств и связей объектов [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7f9cd-107">List properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f9cd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7f9cd-108">Prerequisites</span></span>
<span data-ttu-id="7f9cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f9cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f9cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f9cd-111">Permission type</span></span>|<span data-ttu-id="7f9cd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f9cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f9cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f9cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f9cd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f9cd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7f9cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f9cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f9cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f9cd-116">Not supported.</span></span>|
|<span data-ttu-id="7f9cd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f9cd-117">Application</span></span>|<span data-ttu-id="7f9cd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f9cd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f9cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f9cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7f9cd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7f9cd-120">Request headers</span></span>
|<span data-ttu-id="7f9cd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f9cd-121">Header</span></span>|<span data-ttu-id="7f9cd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7f9cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f9cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f9cd-123">Authorization</span></span>|<span data-ttu-id="7f9cd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f9cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f9cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f9cd-125">Accept</span></span>|<span data-ttu-id="7f9cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f9cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f9cd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f9cd-127">Request body</span></span>
<span data-ttu-id="7f9cd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f9cd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f9cd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f9cd-129">Response</span></span>
<span data-ttu-id="7f9cd-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f9cd-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f9cd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7f9cd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f9cd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f9cd-132">Request</span></span>
<span data-ttu-id="7f9cd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f9cd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="7f9cd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f9cd-134">Response</span></span>
<span data-ttu-id="7f9cd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f9cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3584

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
      "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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
      "passwordBlockFaceUnlock": true,
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockIrisUnlock": true,
      "passwordBlockTrustAgents": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "lowSecurityBiometric",
      "workProfileDataSharingType": "preventAny",
      "workProfileBlockNotificationsWhileDeviceLocked": true,
      "workProfileBlockAddingAccounts": true,
      "workProfileBluetoothEnableContactSharing": true,
      "workProfileBlockScreenCapture": true,
      "workProfileBlockCrossProfileCallerId": true,
      "workProfileBlockCamera": true,
      "workProfileBlockCrossProfileContactsSearch": true,
      "workProfileBlockCrossProfileCopyPaste": true,
      "workProfileDefaultAppPermissionPolicy": "prompt",
      "workProfilePasswordBlockFaceUnlock": true,
      "workProfilePasswordBlockFingerprintUnlock": true,
      "workProfilePasswordBlockIrisUnlock": true,
      "workProfilePasswordBlockTrustAgents": true,
      "workProfilePasswordExpirationDays": 1,
      "workProfilePasswordMinimumLength": 0,
      "workProfilePasswordMinNumericCharacters": 7,
      "workProfilePasswordMinNonLetterCharacters": 9,
      "workProfilePasswordMinLetterCharacters": 6,
      "workProfilePasswordMinLowerCaseCharacters": 9,
      "workProfilePasswordMinUpperCaseCharacters": 9,
      "workProfilePasswordMinSymbolCharacters": 6,
      "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
      "workProfilePasswordPreviousPasswordBlockCount": 13,
      "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
      "workProfilePasswordRequiredType": "lowSecurityBiometric",
      "workProfileRequirePassword": true,
      "securityRequireVerifyApps": true,
      "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
      "vpnEnableAlwaysOnLockdownMode": true,
      "workProfileAllowWidgets": true,
      "workProfileBlockPersonalAppInstallsFromUnknownSources": true
    }
  ]
}
```






