---
title: Получение объекта windows81GeneralConfiguration
description: Чтение свойств и связей объекта windows81GeneralConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20d66276d5655e5d723d00b0da77356c924b6cc5
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365105"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="be789-103">Получение объекта windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="be789-103">Get windows81GeneralConfiguration</span></span>

> <span data-ttu-id="be789-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be789-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be789-105">Чтение свойств и связей объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be789-105">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be789-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="be789-106">Prerequisites</span></span>
<span data-ttu-id="be789-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be789-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be789-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be789-109">Permission type</span></span>|<span data-ttu-id="be789-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be789-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be789-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be789-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be789-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="be789-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="be789-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be789-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be789-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be789-114">Not supported.</span></span>|
|<span data-ttu-id="be789-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be789-115">Application</span></span>|<span data-ttu-id="be789-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be789-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be789-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be789-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be789-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be789-118">Optional query parameters</span></span>
<span data-ttu-id="be789-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="be789-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be789-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be789-120">Request headers</span></span>
|<span data-ttu-id="be789-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be789-121">Header</span></span>|<span data-ttu-id="be789-122">Значение</span><span class="sxs-lookup"><span data-stu-id="be789-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be789-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be789-123">Authorization</span></span>|<span data-ttu-id="be789-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be789-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be789-125">Accept</span><span class="sxs-lookup"><span data-stu-id="be789-125">Accept</span></span>|<span data-ttu-id="be789-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be789-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be789-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be789-127">Request body</span></span>
<span data-ttu-id="be789-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be789-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be789-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="be789-129">Response</span></span>
<span data-ttu-id="be789-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be789-130">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be789-131">Пример</span><span class="sxs-lookup"><span data-stu-id="be789-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="be789-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="be789-132">Request</span></span>
<span data-ttu-id="be789-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be789-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="be789-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="be789-134">Response</span></span>
<span data-ttu-id="be789-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be789-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1964

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
    "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "updatesRequireAutomaticUpdates": true,
    "userAccountControlSettings": "alwaysNotify",
    "workFoldersUrl": "https://example.com/workFoldersUrl/"
  }
}
```




