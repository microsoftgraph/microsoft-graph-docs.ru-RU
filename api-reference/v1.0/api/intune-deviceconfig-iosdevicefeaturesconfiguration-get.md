---
title: Get iosDeviceFeaturesConfiguration
description: Чтение свойств и связей объекта iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a05faa3c6c9fe91797e52a69c63231cff5c9958a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985867"
---
# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="084f5-103">Get iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="084f5-103">Get iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="084f5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="084f5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="084f5-105">Чтение свойств и связей объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="084f5-105">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="084f5-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="084f5-106">Prerequisites</span></span>
<span data-ttu-id="084f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="084f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="084f5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="084f5-109">Permission type</span></span>|<span data-ttu-id="084f5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="084f5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="084f5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="084f5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="084f5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="084f5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="084f5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="084f5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="084f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="084f5-114">Not supported.</span></span>|
|<span data-ttu-id="084f5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="084f5-115">Application</span></span>|<span data-ttu-id="084f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="084f5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="084f5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="084f5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="084f5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="084f5-118">Optional query parameters</span></span>
<span data-ttu-id="084f5-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="084f5-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="084f5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="084f5-120">Request headers</span></span>
|<span data-ttu-id="084f5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="084f5-121">Header</span></span>|<span data-ttu-id="084f5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="084f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="084f5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="084f5-123">Authorization</span></span>|<span data-ttu-id="084f5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="084f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="084f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="084f5-125">Accept</span></span>|<span data-ttu-id="084f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="084f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="084f5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="084f5-127">Request body</span></span>
<span data-ttu-id="084f5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="084f5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="084f5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="084f5-129">Response</span></span>
<span data-ttu-id="084f5-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="084f5-130">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="084f5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="084f5-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="084f5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="084f5-132">Request</span></span>
<span data-ttu-id="084f5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="084f5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="084f5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="084f5-134">Response</span></span>
<span data-ttu-id="084f5-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="084f5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": {
    "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
    "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "assetTagTemplate": "Asset Tag Template value",
    "lockScreenFootnote": "Lock Screen Footnote value",
    "homeScreenDockIcons": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenFolder",
        "displayName": "Display Name value",
        "pages": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
            "displayName": "Display Name value",
            "apps": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenApp",
                "displayName": "Display Name value",
                "bundleID": "Bundle ID value"
              }
            ]
          }
        ]
      }
    ],
    "homeScreenPages": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenPage",
        "displayName": "Display Name value",
        "icons": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolder",
            "displayName": "Display Name value",
            "pages": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
                "displayName": "Display Name value",
                "apps": [
                  {
                    "@odata.type": "microsoft.graph.iosHomeScreenApp",
                    "displayName": "Display Name value",
                    "bundleID": "Bundle ID value"
                  }
                ]
              }
            ]
          }
        ]
      }
    ],
    "notificationSettings": [
      {
        "@odata.type": "microsoft.graph.iosNotificationSettings",
        "bundleID": "Bundle ID value",
        "appName": "App Name value",
        "publisher": "Publisher value",
        "enabled": true,
        "showInNotificationCenter": true,
        "showOnLockScreen": true,
        "alertType": "banner",
        "badgesEnabled": true,
        "soundsEnabled": true
      }
    ]
  }
}
```



