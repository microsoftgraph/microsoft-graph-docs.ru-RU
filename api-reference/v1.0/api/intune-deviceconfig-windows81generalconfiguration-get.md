---
title: Получение объекта windows81GeneralConfiguration
description: Чтение свойств и связей объекта windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7bf197363579dcf07e5c62252503f6358ccb81b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753806"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="bfae4-103">Получение объекта windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfae4-103">Get windows81GeneralConfiguration</span></span>

<span data-ttu-id="bfae4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfae4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bfae4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfae4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfae4-106">Чтение свойств и связей объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bfae4-106">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfae4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bfae4-107">Prerequisites</span></span>
<span data-ttu-id="bfae4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfae4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfae4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfae4-110">Permission type</span></span>|<span data-ttu-id="bfae4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfae4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfae4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfae4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bfae4-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfae4-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bfae4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfae4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfae4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfae4-115">Not supported.</span></span>|
|<span data-ttu-id="bfae4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bfae4-116">Application</span></span>|<span data-ttu-id="bfae4-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfae4-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfae4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfae4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bfae4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bfae4-119">Optional query parameters</span></span>
<span data-ttu-id="bfae4-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bfae4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfae4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfae4-121">Request headers</span></span>
|<span data-ttu-id="bfae4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bfae4-122">Header</span></span>|<span data-ttu-id="bfae4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bfae4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfae4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfae4-124">Authorization</span></span>|<span data-ttu-id="bfae4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfae4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfae4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="bfae4-126">Accept</span></span>|<span data-ttu-id="bfae4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bfae4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfae4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfae4-128">Request body</span></span>
<span data-ttu-id="bfae4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bfae4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfae4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfae4-130">Response</span></span>
<span data-ttu-id="bfae4-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bfae4-131">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfae4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bfae4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfae4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfae4-133">Request</span></span>
<span data-ttu-id="bfae4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfae4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bfae4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfae4-135">Response</span></span>
<span data-ttu-id="bfae4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfae4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




