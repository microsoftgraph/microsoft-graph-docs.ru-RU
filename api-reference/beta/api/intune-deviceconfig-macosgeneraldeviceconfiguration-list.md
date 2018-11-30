---
title: Перечисление объектов macOSGeneralDeviceConfiguration
description: Список свойств и связей объектов macOSGeneralDeviceConfiguration.
ms.openlocfilehash: a1d0bb60b5a75af5d65f7debb6141ac7c5dfee0a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078822"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="ec05e-103">Перечисление объектов macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec05e-103">List macOSGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="ec05e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ec05e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec05e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec05e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec05e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ec05e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec05e-107">Список свойств и связей объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec05e-107">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec05e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ec05e-108">Prerequisites</span></span>
<span data-ttu-id="ec05e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec05e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec05e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec05e-111">Permission type</span></span>|<span data-ttu-id="ec05e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec05e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec05e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec05e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec05e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec05e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ec05e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec05e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec05e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec05e-116">Not supported.</span></span>|
|<span data-ttu-id="ec05e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec05e-117">Application</span></span>|<span data-ttu-id="ec05e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec05e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec05e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec05e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ec05e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec05e-120">Request headers</span></span>
|<span data-ttu-id="ec05e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec05e-121">Header</span></span>|<span data-ttu-id="ec05e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ec05e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec05e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec05e-123">Authorization</span></span>|<span data-ttu-id="ec05e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ec05e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec05e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ec05e-125">Accept</span></span>|<span data-ttu-id="ec05e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec05e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec05e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec05e-127">Request body</span></span>
<span data-ttu-id="ec05e-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec05e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec05e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec05e-129">Response</span></span>
<span data-ttu-id="ec05e-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec05e-130">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec05e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ec05e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec05e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec05e-132">Request</span></span>
<span data-ttu-id="ec05e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec05e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ec05e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec05e-134">Response</span></span>
<span data-ttu-id="ec05e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ec05e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2178

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
      "passwordBlockFingerprintUnlock": true
    }
  ]
}
```





