---
title: Список Андроидфорворкженералдевицеконфигуратионс
description: Список свойств и связей объектов androidForWorkGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 222097a7bbc2bd0670e303c536bff8df12749b87
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436003"
---
# <a name="list-androidforworkgeneraldeviceconfigurations"></a><span data-ttu-id="35381-103">Список Андроидфорворкженералдевицеконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="35381-103">List androidForWorkGeneralDeviceConfigurations</span></span>

<span data-ttu-id="35381-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35381-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35381-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35381-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35381-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35381-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35381-107">Список свойств и связей объектов [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="35381-107">List properties and relationships of the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35381-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="35381-108">Prerequisites</span></span>
<span data-ttu-id="35381-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35381-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35381-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35381-111">Permission type</span></span>|<span data-ttu-id="35381-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35381-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35381-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35381-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35381-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="35381-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="35381-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35381-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35381-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35381-116">Not supported.</span></span>|
|<span data-ttu-id="35381-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="35381-117">Application</span></span>|<span data-ttu-id="35381-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="35381-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35381-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35381-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="35381-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="35381-120">Request headers</span></span>
|<span data-ttu-id="35381-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35381-121">Header</span></span>|<span data-ttu-id="35381-122">Значение</span><span class="sxs-lookup"><span data-stu-id="35381-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35381-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35381-123">Authorization</span></span>|<span data-ttu-id="35381-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35381-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35381-125">Accept</span><span class="sxs-lookup"><span data-stu-id="35381-125">Accept</span></span>|<span data-ttu-id="35381-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35381-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35381-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35381-127">Request body</span></span>
<span data-ttu-id="35381-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35381-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35381-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="35381-129">Response</span></span>
<span data-ttu-id="35381-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35381-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35381-131">Пример</span><span class="sxs-lookup"><span data-stu-id="35381-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="35381-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="35381-132">Request</span></span>
<span data-ttu-id="35381-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35381-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="35381-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="35381-134">Response</span></span>
<span data-ttu-id="35381-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35381-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3398

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
      "id": "a931a366-a366-a931-66a3-31a966a331a9",
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
      "passwordBlockFingerprintUnlock": true,
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
      "workProfilePasswordBlockFingerprintUnlock": true,
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



