---
title: Перечисление объектов windows81GeneralConfiguration
description: Перечисление свойств и связей объектов windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0f9e7886b3bb9ce16442162d3c797ba087db042
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262652"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="ba611-103">Перечисление объектов windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba611-103">List windows81GeneralConfigurations</span></span>

> <span data-ttu-id="ba611-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba611-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba611-105">Перечисление свойств и связей объектов [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba611-105">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba611-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ba611-106">Prerequisites</span></span>
<span data-ttu-id="ba611-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba611-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ba611-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba611-109">Permission type</span></span>|<span data-ttu-id="ba611-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba611-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba611-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba611-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba611-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba611-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ba611-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba611-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba611-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba611-114">Not supported.</span></span>|
|<span data-ttu-id="ba611-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba611-115">Application</span></span>|<span data-ttu-id="ba611-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba611-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba611-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba611-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ba611-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba611-118">Request headers</span></span>
|<span data-ttu-id="ba611-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba611-119">Header</span></span>|<span data-ttu-id="ba611-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ba611-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba611-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba611-121">Authorization</span></span>|<span data-ttu-id="ba611-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ba611-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba611-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ba611-123">Accept</span></span>|<span data-ttu-id="ba611-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ba611-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba611-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba611-125">Request body</span></span>
<span data-ttu-id="ba611-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba611-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba611-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba611-127">Response</span></span>
<span data-ttu-id="ba611-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba611-128">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba611-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ba611-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba611-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba611-130">Request</span></span>
<span data-ttu-id="ba611-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba611-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ba611-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba611-132">Response</span></span>
<span data-ttu-id="ba611-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ba611-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



