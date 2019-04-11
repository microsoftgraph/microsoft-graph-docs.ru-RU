---
title: Get macOSGeneralDeviceConfiguration
description: Чтение свойств и связей объекта macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71cb75ee1fa1c862a30171f81cfd1000c77dfe77
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771518"
---
# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="feee4-103">Get macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="feee4-103">Get macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="feee4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="feee4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="feee4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="feee4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feee4-106">Чтение свойств и связей объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="feee4-106">Read properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="feee4-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="feee4-107">Prerequisites</span></span>
<span data-ttu-id="feee4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="feee4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="feee4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="feee4-110">Permission type</span></span>|<span data-ttu-id="feee4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="feee4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="feee4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="feee4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="feee4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="feee4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="feee4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="feee4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="feee4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="feee4-115">Not supported.</span></span>|
|<span data-ttu-id="feee4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="feee4-116">Application</span></span>|<span data-ttu-id="feee4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="feee4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="feee4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="feee4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="feee4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="feee4-119">Optional query parameters</span></span>
<span data-ttu-id="feee4-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="feee4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="feee4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="feee4-121">Request headers</span></span>
|<span data-ttu-id="feee4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="feee4-122">Header</span></span>|<span data-ttu-id="feee4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="feee4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="feee4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="feee4-124">Authorization</span></span>|<span data-ttu-id="feee4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="feee4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="feee4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="feee4-126">Accept</span></span>|<span data-ttu-id="feee4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="feee4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="feee4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="feee4-128">Request body</span></span>
<span data-ttu-id="feee4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="feee4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="feee4-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="feee4-130">Response</span></span>
<span data-ttu-id="feee4-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="feee4-131">If successful, this method returns a `200 OK` response code and [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="feee4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="feee4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="feee4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="feee4-133">Request</span></span>
<span data-ttu-id="feee4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="feee4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="feee4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="feee4-135">Response</span></span>
<span data-ttu-id="feee4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="feee4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2301

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
    "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "emailInDomainSuffixes": [
      "Email In Domain Suffixes value"
    ],
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumCharacterSetCount": 0,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequiredType": "alphanumeric",
    "passwordRequired": true,
    "keychainBlockCloudSync": true,
    "airPrintBlocked": true,
    "airPrintForceTrustedTLS": true,
    "airPrintBlockiBeaconDiscovery": true,
    "safariBlockAutofill": true,
    "cameraBlocked": true,
    "iTunesBlockMusicService": true,
    "spotlightBlockInternetResults": true,
    "keyboardBlockDictation": true,
    "definitionLookupBlocked": true,
    "appleWatchBlockAutoUnlock": true,
    "iTunesBlockFileSharing": true,
    "iCloudBlockDocumentSync": true,
    "iCloudBlockMail": true,
    "iCloudBlockAddressBook": true,
    "iCloudBlockCalendar": true,
    "iCloudBlockReminders": true,
    "iCloudBlockBookmarks": true,
    "iCloudBlockNotes": true,
    "airDropBlocked": true,
    "passwordBlockModification": true,
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockAutoFill": true,
    "passwordBlockProximityRequests": true,
    "passwordBlockAirDropSharing": true,
    "softwareUpdatesEnforcedDelayInDays": 2,
    "softwareUpdatesForceDelayed": true,
    "contentCachingBlocked": true
  }
}
```





