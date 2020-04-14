---
title: Получение объекта windows81GeneralConfiguration
description: Чтение свойств и связей объекта windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af77b74c8b8d13a1f032d7daf2703ed6c057712a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43430426"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="7060d-103">Получение объекта windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="7060d-103">Get windows81GeneralConfiguration</span></span>

<span data-ttu-id="7060d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7060d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7060d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7060d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7060d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7060d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7060d-107">Чтение свойств и связей объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7060d-107">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7060d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7060d-108">Prerequisites</span></span>
<span data-ttu-id="7060d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7060d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7060d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7060d-111">Permission type</span></span>|<span data-ttu-id="7060d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7060d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7060d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7060d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7060d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7060d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7060d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7060d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7060d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7060d-116">Not supported.</span></span>|
|<span data-ttu-id="7060d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7060d-117">Application</span></span>|<span data-ttu-id="7060d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7060d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7060d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7060d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7060d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7060d-120">Optional query parameters</span></span>
<span data-ttu-id="7060d-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7060d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7060d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7060d-122">Request headers</span></span>
|<span data-ttu-id="7060d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7060d-123">Header</span></span>|<span data-ttu-id="7060d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7060d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7060d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7060d-125">Authorization</span></span>|<span data-ttu-id="7060d-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7060d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7060d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7060d-127">Accept</span></span>|<span data-ttu-id="7060d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7060d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7060d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7060d-129">Request body</span></span>
<span data-ttu-id="7060d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7060d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7060d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7060d-131">Response</span></span>
<span data-ttu-id="7060d-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7060d-132">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7060d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7060d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7060d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7060d-134">Request</span></span>
<span data-ttu-id="7060d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7060d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7060d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7060d-136">Response</span></span>
<span data-ttu-id="7060d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7060d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3022

{
  "value": {
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
}
```



