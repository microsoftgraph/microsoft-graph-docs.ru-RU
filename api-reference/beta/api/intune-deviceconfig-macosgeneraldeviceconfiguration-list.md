---
title: Перечисление объектов macOSGeneralDeviceConfiguration
description: Список свойств и связей объектов macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63ec36b6db40f6b4f05525fe7441407931af55f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518466"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="a2cf9-103">Перечисление объектов macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2cf9-103">List macOSGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="a2cf9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2cf9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2cf9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2cf9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2cf9-106">Список свойств и связей объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2cf9-106">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2cf9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a2cf9-107">Prerequisites</span></span>
<span data-ttu-id="a2cf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2cf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2cf9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2cf9-110">Permission type</span></span>|<span data-ttu-id="a2cf9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2cf9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2cf9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2cf9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2cf9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2cf9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a2cf9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2cf9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2cf9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2cf9-115">Not supported.</span></span>|
|<span data-ttu-id="a2cf9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2cf9-116">Application</span></span>|<span data-ttu-id="a2cf9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2cf9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2cf9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2cf9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a2cf9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2cf9-119">Request headers</span></span>
|<span data-ttu-id="a2cf9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2cf9-120">Header</span></span>|<span data-ttu-id="a2cf9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a2cf9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2cf9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2cf9-122">Authorization</span></span>|<span data-ttu-id="a2cf9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2cf9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2cf9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a2cf9-124">Accept</span></span>|<span data-ttu-id="a2cf9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2cf9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2cf9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2cf9-126">Request body</span></span>
<span data-ttu-id="a2cf9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2cf9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2cf9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2cf9-128">Response</span></span>
<span data-ttu-id="a2cf9-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2cf9-129">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2cf9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a2cf9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2cf9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2cf9-131">Request</span></span>
<span data-ttu-id="a2cf9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2cf9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a2cf9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2cf9-133">Response</span></span>
<span data-ttu-id="a2cf9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2cf9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2437

{
  "value": [
    {
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
  ]
}
```





