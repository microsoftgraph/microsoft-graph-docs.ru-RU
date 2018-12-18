---
title: Получение объекта windows81GeneralConfiguration
description: Чтение свойств и связей объекта windows81GeneralConfiguration.
author: tfitzmac
ms.openlocfilehash: 2a7977a83cbd84326142940962c01de948beb6f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356492"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="d7973-103">Получение объекта windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="d7973-103">Get windows81GeneralConfiguration</span></span>

> <span data-ttu-id="d7973-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7973-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7973-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7973-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7973-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d7973-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7973-107">Чтение свойств и связей объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7973-107">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7973-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d7973-108">Prerequisites</span></span>
<span data-ttu-id="d7973-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7973-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7973-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7973-111">Permission type</span></span>|<span data-ttu-id="d7973-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7973-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7973-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7973-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7973-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7973-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d7973-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7973-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7973-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7973-116">Not supported.</span></span>|
|<span data-ttu-id="d7973-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7973-117">Application</span></span>|<span data-ttu-id="d7973-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7973-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7973-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7973-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7973-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d7973-120">Optional query parameters</span></span>
<span data-ttu-id="d7973-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d7973-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d7973-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7973-122">Request headers</span></span>
|<span data-ttu-id="d7973-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7973-123">Header</span></span>|<span data-ttu-id="d7973-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d7973-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7973-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7973-125">Authorization</span></span>|<span data-ttu-id="d7973-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d7973-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7973-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d7973-127">Accept</span></span>|<span data-ttu-id="d7973-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d7973-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7973-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7973-129">Request body</span></span>
<span data-ttu-id="d7973-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7973-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7973-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7973-131">Response</span></span>
<span data-ttu-id="d7973-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d7973-132">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7973-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d7973-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7973-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7973-134">Request</span></span>
<span data-ttu-id="d7973-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7973-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d7973-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7973-136">Response</span></span>
<span data-ttu-id="d7973-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d7973-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





