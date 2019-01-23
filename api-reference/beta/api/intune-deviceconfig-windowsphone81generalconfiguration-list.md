---
title: Перечисление объектов windowsPhone81GeneralConfiguration
description: Список свойств и связей объектов windowsPhone81GeneralConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cb5b2b40fcb587bb0f7b9515263517534701278
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423253"
---
# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="87bb3-103">Перечисление объектов windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="87bb3-103">List windowsPhone81GeneralConfigurations</span></span>

> <span data-ttu-id="87bb3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="87bb3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="87bb3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87bb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87bb3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87bb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87bb3-107">Список свойств и связей объектов [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87bb3-107">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87bb3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="87bb3-108">Prerequisites</span></span>
<span data-ttu-id="87bb3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="87bb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87bb3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87bb3-111">Permission type</span></span>|<span data-ttu-id="87bb3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87bb3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87bb3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87bb3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87bb3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87bb3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87bb3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87bb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87bb3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87bb3-116">Not supported.</span></span>|
|<span data-ttu-id="87bb3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87bb3-117">Application</span></span>|<span data-ttu-id="87bb3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87bb3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87bb3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87bb3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="87bb3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87bb3-120">Request headers</span></span>
|<span data-ttu-id="87bb3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87bb3-121">Header</span></span>|<span data-ttu-id="87bb3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87bb3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87bb3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87bb3-123">Authorization</span></span>|<span data-ttu-id="87bb3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="87bb3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87bb3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87bb3-125">Accept</span></span>|<span data-ttu-id="87bb3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87bb3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87bb3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87bb3-127">Request body</span></span>
<span data-ttu-id="87bb3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87bb3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87bb3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="87bb3-129">Response</span></span>
<span data-ttu-id="87bb3-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="87bb3-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87bb3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="87bb3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87bb3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="87bb3-132">Request</span></span>
<span data-ttu-id="87bb3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87bb3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="87bb3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="87bb3-134">Response</span></span>
<span data-ttu-id="87bb3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87bb3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1950

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
      "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "applyOnlyToWindowsPhone81": true,
      "appsBlockCopyPaste": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "cellularBlockWifiTethering": true,
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
      "diagnosticDataBlockSubmission": true,
      "emailBlockAddingAccounts": true,
      "locationServicesBlocked": true,
      "microsoftAccountBlocked": true,
      "nfcBlocked": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true,
      "screenCaptureBlocked": true,
      "storageBlockRemovableStorage": true,
      "storageRequireEncryption": true,
      "webBrowserBlocked": true,
      "wifiBlocked": true,
      "wifiBlockAutomaticConnectHotspots": true,
      "wifiBlockHotspotReporting": true,
      "windowsStoreBlocked": true
    }
  ]
}
```




