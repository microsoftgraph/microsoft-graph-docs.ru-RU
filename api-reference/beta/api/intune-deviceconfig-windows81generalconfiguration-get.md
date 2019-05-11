---
title: Получение объекта windows81GeneralConfiguration
description: Чтение свойств и связей объекта windows81GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12e7b8c9dc4c08d5a60747150c0ae4150a7c0fb2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918257"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="ef280-103">Получение объекта windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef280-103">Get windows81GeneralConfiguration</span></span>

> <span data-ttu-id="ef280-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef280-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef280-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef280-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef280-106">Чтение свойств и связей объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef280-106">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef280-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ef280-107">Prerequisites</span></span>
<span data-ttu-id="ef280-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef280-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef280-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef280-110">Permission type</span></span>|<span data-ttu-id="ef280-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef280-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef280-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef280-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef280-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef280-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ef280-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef280-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef280-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef280-115">Not supported.</span></span>|
|<span data-ttu-id="ef280-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef280-116">Application</span></span>|<span data-ttu-id="ef280-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef280-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef280-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef280-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef280-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef280-119">Optional query parameters</span></span>
<span data-ttu-id="ef280-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ef280-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef280-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef280-121">Request headers</span></span>
|<span data-ttu-id="ef280-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef280-122">Header</span></span>|<span data-ttu-id="ef280-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ef280-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef280-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef280-124">Authorization</span></span>|<span data-ttu-id="ef280-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef280-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef280-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ef280-126">Accept</span></span>|<span data-ttu-id="ef280-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ef280-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef280-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef280-128">Request body</span></span>
<span data-ttu-id="ef280-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef280-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef280-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef280-130">Response</span></span>
<span data-ttu-id="ef280-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ef280-131">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef280-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ef280-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef280-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef280-133">Request</span></span>
<span data-ttu-id="ef280-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef280-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ef280-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef280-135">Response</span></span>
<span data-ttu-id="ef280-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef280-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2207

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
    "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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




