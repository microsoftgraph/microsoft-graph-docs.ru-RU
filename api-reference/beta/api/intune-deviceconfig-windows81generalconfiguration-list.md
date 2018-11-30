---
title: Перечисление объектов windows81GeneralConfiguration
description: Перечисление свойств и связей объектов windows81GeneralConfiguration.
ms.openlocfilehash: 09ebff265df940360eb6484be4da94949a975ae0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082356"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="6aedd-103">Перечисление объектов windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="6aedd-103">List windows81GeneralConfigurations</span></span>

> <span data-ttu-id="6aedd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6aedd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6aedd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aedd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6aedd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6aedd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6aedd-107">Перечисление свойств и связей объектов [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6aedd-107">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6aedd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6aedd-108">Prerequisites</span></span>
<span data-ttu-id="6aedd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aedd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aedd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aedd-111">Permission type</span></span>|<span data-ttu-id="6aedd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aedd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aedd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aedd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6aedd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6aedd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6aedd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aedd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aedd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aedd-116">Not supported.</span></span>|
|<span data-ttu-id="6aedd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6aedd-117">Application</span></span>|<span data-ttu-id="6aedd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aedd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aedd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6aedd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6aedd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6aedd-120">Request headers</span></span>
|<span data-ttu-id="6aedd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6aedd-121">Header</span></span>|<span data-ttu-id="6aedd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6aedd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aedd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aedd-123">Authorization</span></span>|<span data-ttu-id="6aedd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6aedd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aedd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6aedd-125">Accept</span></span>|<span data-ttu-id="6aedd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6aedd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aedd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6aedd-127">Request body</span></span>
<span data-ttu-id="6aedd-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6aedd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6aedd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6aedd-129">Response</span></span>
<span data-ttu-id="6aedd-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6aedd-130">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aedd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6aedd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6aedd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6aedd-132">Request</span></span>
<span data-ttu-id="6aedd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6aedd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6aedd-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6aedd-134">Response</span></span>
<span data-ttu-id="6aedd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6aedd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

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





