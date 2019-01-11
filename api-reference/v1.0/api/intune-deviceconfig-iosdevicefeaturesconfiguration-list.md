---
title: Перечисление объектов iosDeviceFeaturesConfiguration
description: Список свойств и связей объектов iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 31a903c3d938b2f85227e7a5d0e51d3003f64727
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884114"
---
# <a name="list-iosdevicefeaturesconfigurations"></a><span data-ttu-id="7b53d-103">Перечисление объектов iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b53d-103">List iosDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="7b53d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7b53d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b53d-105">Список свойств и связей объектов [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b53d-105">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b53d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7b53d-106">Prerequisites</span></span>
<span data-ttu-id="7b53d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b53d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b53d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b53d-109">Permission type</span></span>|<span data-ttu-id="7b53d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b53d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b53d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b53d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7b53d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b53d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7b53d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b53d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b53d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b53d-114">Not supported.</span></span>|
|<span data-ttu-id="7b53d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b53d-115">Application</span></span>|<span data-ttu-id="7b53d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b53d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b53d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b53d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7b53d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b53d-118">Request headers</span></span>
|<span data-ttu-id="7b53d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b53d-119">Header</span></span>|<span data-ttu-id="7b53d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7b53d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b53d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b53d-121">Authorization</span></span>|<span data-ttu-id="7b53d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7b53d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b53d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7b53d-123">Accept</span></span>|<span data-ttu-id="7b53d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7b53d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b53d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b53d-125">Request body</span></span>
<span data-ttu-id="7b53d-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b53d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b53d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b53d-127">Response</span></span>
<span data-ttu-id="7b53d-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b53d-128">If successful, this method returns a `200 OK` response code and a collection of [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b53d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7b53d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b53d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b53d-130">Request</span></span>
<span data-ttu-id="7b53d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b53d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="7b53d-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b53d-132">Response</span></span>
<span data-ttu-id="7b53d-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7b53d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2461

{
  "value": [
    {
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
  ]
}
```



