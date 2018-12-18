---
title: Перечисление объектов windowsPhone81GeneralConfiguration
description: Список свойств и связей объектов windowsPhone81GeneralConfiguration.
author: tfitzmac
ms.openlocfilehash: 9b6bd1faa1a6c4460c97374d90967b8fc7b18e25
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346881"
---
# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="626af-103">Перечисление объектов windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="626af-103">List windowsPhone81GeneralConfigurations</span></span>

> <span data-ttu-id="626af-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="626af-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="626af-105">Список свойств и связей объектов [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="626af-105">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="626af-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="626af-106">Prerequisites</span></span>
<span data-ttu-id="626af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="626af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="626af-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="626af-109">Permission type</span></span>|<span data-ttu-id="626af-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="626af-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="626af-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="626af-111">Delegated (work or school account)</span></span>|<span data-ttu-id="626af-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="626af-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="626af-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="626af-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="626af-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="626af-114">Not supported.</span></span>|
|<span data-ttu-id="626af-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="626af-115">Application</span></span>|<span data-ttu-id="626af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="626af-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="626af-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="626af-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="626af-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="626af-118">Request headers</span></span>
|<span data-ttu-id="626af-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="626af-119">Header</span></span>|<span data-ttu-id="626af-120">Значение</span><span class="sxs-lookup"><span data-stu-id="626af-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="626af-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="626af-121">Authorization</span></span>|<span data-ttu-id="626af-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="626af-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="626af-123">Accept</span><span class="sxs-lookup"><span data-stu-id="626af-123">Accept</span></span>|<span data-ttu-id="626af-124">application/json</span><span class="sxs-lookup"><span data-stu-id="626af-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="626af-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="626af-125">Request body</span></span>
<span data-ttu-id="626af-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="626af-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="626af-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="626af-127">Response</span></span>
<span data-ttu-id="626af-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="626af-128">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="626af-129">Пример</span><span class="sxs-lookup"><span data-stu-id="626af-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="626af-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="626af-130">Request</span></span>
<span data-ttu-id="626af-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="626af-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="626af-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="626af-132">Response</span></span>
<span data-ttu-id="626af-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="626af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1842

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
      "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



