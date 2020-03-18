---
title: Перечисление объектов windows81GeneralConfiguration
description: Перечисление свойств и связей объектов windows81GeneralConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d023342eb8491fa92cf763953c9b5c33bef9ab43
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42737247"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="0721f-103">Перечисление объектов windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="0721f-103">List windows81GeneralConfigurations</span></span>

> <span data-ttu-id="0721f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0721f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0721f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0721f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0721f-106">Перечисление свойств и связей объектов [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0721f-106">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0721f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0721f-107">Prerequisites</span></span>
<span data-ttu-id="0721f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0721f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0721f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0721f-110">Permission type</span></span>|<span data-ttu-id="0721f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0721f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0721f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0721f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0721f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0721f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0721f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0721f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0721f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0721f-115">Not supported.</span></span>|
|<span data-ttu-id="0721f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0721f-116">Application</span></span>|<span data-ttu-id="0721f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0721f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0721f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0721f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0721f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0721f-119">Request headers</span></span>
|<span data-ttu-id="0721f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0721f-120">Header</span></span>|<span data-ttu-id="0721f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0721f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0721f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0721f-122">Authorization</span></span>|<span data-ttu-id="0721f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0721f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0721f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0721f-124">Accept</span></span>|<span data-ttu-id="0721f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0721f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0721f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0721f-126">Request body</span></span>
<span data-ttu-id="0721f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0721f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0721f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0721f-128">Response</span></span>
<span data-ttu-id="0721f-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0721f-129">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0721f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0721f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0721f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0721f-131">Request</span></span>
<span data-ttu-id="0721f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0721f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0721f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0721f-133">Response</span></span>
<span data-ttu-id="0721f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0721f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3170

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
      "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
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
      "accountsBlockAddingNonMicrosoftAccountEmail": true,
      "applyOnlyToWindows81": true,
      "browserBlockAutofill": true,
      "browserBlockAutomaticDetectionOfIntranetSites": true,
      "browserBlockEnterpriseModeAccess": true,
      "browserBlockJavaScript": true,
      "browserBlockPlugins": true,
      "browserBlockPopups": true,
      "browserBlockSendingDoNotTrackHeader": true,
      "browserBlockSingleWordEntryOnIntranetSites": true,
      "browserRequireSmartScreen": true,
      "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
      "browserInternetSecurityLevel": "medium",
      "browserIntranetSecurityLevel": "low",
      "browserLoggingReportLocation": "Browser Logging Report Location value",
      "browserRequireHighSecurityForRestrictedSites": true,
      "browserRequireFirewall": true,
      "browserRequireFraudWarning": true,
      "browserTrustedSitesSecurityLevel": "low",
      "cellularBlockDataRoaming": true,
      "diagnosticsBlockDataSubmission": true,
      "passwordBlockPicturePasswordAndPin": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequiredType": "alphanumeric",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "storageRequireDeviceEncryption": true,
      "minimumAutoInstallClassification": "recommendedAndImportant",
      "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
      "updatesRequireAutomaticUpdates": true,
      "userAccountControlSettings": "alwaysNotify",
      "workFoldersUrl": "https://example.com/workFoldersUrl/"
    }
  ]
}
```




