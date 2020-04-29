---
title: Перечисление объектов windows81GeneralConfiguration
description: Перечисление свойств и связей объектов windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 019fa10da452c2671c4f568e6e88ce5a3f3c2131
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441880"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="90652-103">Перечисление объектов windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="90652-103">List windows81GeneralConfigurations</span></span>

<span data-ttu-id="90652-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90652-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90652-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90652-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90652-106">Перечисление свойств и связей объектов [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90652-106">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90652-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="90652-107">Prerequisites</span></span>
<span data-ttu-id="90652-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90652-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90652-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90652-110">Permission type</span></span>|<span data-ttu-id="90652-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90652-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90652-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90652-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90652-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90652-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="90652-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90652-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90652-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90652-115">Not supported.</span></span>|
|<span data-ttu-id="90652-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90652-116">Application</span></span>|<span data-ttu-id="90652-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90652-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90652-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90652-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="90652-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90652-119">Request headers</span></span>
|<span data-ttu-id="90652-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90652-120">Header</span></span>|<span data-ttu-id="90652-121">Значение</span><span class="sxs-lookup"><span data-stu-id="90652-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90652-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90652-122">Authorization</span></span>|<span data-ttu-id="90652-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90652-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90652-124">Accept</span><span class="sxs-lookup"><span data-stu-id="90652-124">Accept</span></span>|<span data-ttu-id="90652-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90652-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90652-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90652-126">Request body</span></span>
<span data-ttu-id="90652-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90652-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90652-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="90652-128">Response</span></span>
<span data-ttu-id="90652-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="90652-129">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90652-130">Пример</span><span class="sxs-lookup"><span data-stu-id="90652-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="90652-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="90652-131">Request</span></span>
<span data-ttu-id="90652-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90652-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="90652-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="90652-133">Response</span></span>
<span data-ttu-id="90652-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90652-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2058

{
  "value": [
    {
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
  ]
}
```






