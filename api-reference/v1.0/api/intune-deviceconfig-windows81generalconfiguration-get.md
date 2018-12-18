---
title: Получение объекта windows81GeneralConfiguration
description: Чтение свойств и связей объекта windows81GeneralConfiguration.
author: tfitzmac
ms.openlocfilehash: fd35bee5e035317dd67b3eb2bb0ec20676e9a4d1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354021"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="51105-103">Получение объекта windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="51105-103">Get windows81GeneralConfiguration</span></span>

> <span data-ttu-id="51105-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51105-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51105-105">Чтение свойств и связей объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51105-105">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51105-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="51105-106">Prerequisites</span></span>
<span data-ttu-id="51105-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51105-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51105-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51105-109">Permission type</span></span>|<span data-ttu-id="51105-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51105-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51105-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51105-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51105-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51105-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="51105-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51105-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51105-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51105-114">Not supported.</span></span>|
|<span data-ttu-id="51105-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51105-115">Application</span></span>|<span data-ttu-id="51105-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51105-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51105-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51105-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51105-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51105-118">Optional query parameters</span></span>
<span data-ttu-id="51105-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51105-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="51105-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51105-120">Request headers</span></span>
|<span data-ttu-id="51105-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51105-121">Header</span></span>|<span data-ttu-id="51105-122">Значение</span><span class="sxs-lookup"><span data-stu-id="51105-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51105-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51105-123">Authorization</span></span>|<span data-ttu-id="51105-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="51105-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51105-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51105-125">Accept</span></span>|<span data-ttu-id="51105-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51105-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51105-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51105-127">Request body</span></span>
<span data-ttu-id="51105-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51105-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51105-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="51105-129">Response</span></span>
<span data-ttu-id="51105-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51105-130">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51105-131">Пример</span><span class="sxs-lookup"><span data-stu-id="51105-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="51105-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="51105-132">Request</span></span>
<span data-ttu-id="51105-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51105-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="51105-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="51105-134">Response</span></span>
<span data-ttu-id="51105-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51105-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



