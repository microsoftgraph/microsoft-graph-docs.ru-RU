---
title: Get windowsPhone81GeneralConfiguration
description: Чтение свойств и связей объекта windowsPhone81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1df03cde711a4b4fe13d9eeee424b305de25679a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009655"
---
# <a name="get-windowsphone81generalconfiguration"></a><span data-ttu-id="73663-103">Get windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="73663-103">Get windowsPhone81GeneralConfiguration</span></span>

<span data-ttu-id="73663-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73663-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73663-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73663-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73663-106">Чтение свойств и связей объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="73663-106">Read properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73663-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="73663-107">Prerequisites</span></span>
<span data-ttu-id="73663-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73663-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73663-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73663-110">Permission type</span></span>|<span data-ttu-id="73663-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73663-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73663-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73663-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73663-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73663-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73663-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73663-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73663-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73663-115">Not supported.</span></span>|
|<span data-ttu-id="73663-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73663-116">Application</span></span>|<span data-ttu-id="73663-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73663-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73663-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73663-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73663-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="73663-119">Optional query parameters</span></span>
<span data-ttu-id="73663-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="73663-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73663-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73663-121">Request headers</span></span>
|<span data-ttu-id="73663-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73663-122">Header</span></span>|<span data-ttu-id="73663-123">Значение</span><span class="sxs-lookup"><span data-stu-id="73663-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73663-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="73663-124">Authorization</span></span>|<span data-ttu-id="73663-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73663-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73663-126">Accept</span><span class="sxs-lookup"><span data-stu-id="73663-126">Accept</span></span>|<span data-ttu-id="73663-127">application/json</span><span class="sxs-lookup"><span data-stu-id="73663-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73663-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73663-128">Request body</span></span>
<span data-ttu-id="73663-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73663-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73663-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="73663-130">Response</span></span>
<span data-ttu-id="73663-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="73663-131">If successful, this method returns a `200 OK` response code and [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73663-132">Пример</span><span class="sxs-lookup"><span data-stu-id="73663-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="73663-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="73663-133">Request</span></span>
<span data-ttu-id="73663-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73663-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="73663-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="73663-135">Response</span></span>
<span data-ttu-id="73663-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73663-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1740

{
  "value": {
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
}
```









