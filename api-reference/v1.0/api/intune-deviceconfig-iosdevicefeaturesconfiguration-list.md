---
title: Перечисление объектов iosDeviceFeaturesConfiguration
description: Список свойств и связей объектов iosDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 57e7a5f12cdb8176bbc99c4fd06befd5657c667f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756353"
---
# <a name="list-iosdevicefeaturesconfigurations"></a><span data-ttu-id="d8d64-103">Перечисление объектов iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8d64-103">List iosDeviceFeaturesConfigurations</span></span>

<span data-ttu-id="d8d64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8d64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8d64-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8d64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8d64-106">Список свойств и связей объектов [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8d64-106">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8d64-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d8d64-107">Prerequisites</span></span>
<span data-ttu-id="d8d64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8d64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8d64-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8d64-110">Permission type</span></span>|<span data-ttu-id="d8d64-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8d64-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8d64-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8d64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8d64-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8d64-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8d64-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8d64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8d64-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8d64-115">Not supported.</span></span>|
|<span data-ttu-id="d8d64-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d8d64-116">Application</span></span>|<span data-ttu-id="d8d64-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8d64-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8d64-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8d64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d8d64-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d8d64-119">Request headers</span></span>
|<span data-ttu-id="d8d64-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8d64-120">Header</span></span>|<span data-ttu-id="d8d64-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d8d64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8d64-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8d64-122">Authorization</span></span>|<span data-ttu-id="d8d64-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8d64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8d64-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d8d64-124">Accept</span></span>|<span data-ttu-id="d8d64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8d64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8d64-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8d64-126">Request body</span></span>
<span data-ttu-id="d8d64-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8d64-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8d64-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8d64-128">Response</span></span>
<span data-ttu-id="d8d64-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8d64-129">If successful, this method returns a `200 OK` response code and a collection of [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8d64-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d8d64-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8d64-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8d64-131">Request</span></span>
<span data-ttu-id="d8d64-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8d64-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d8d64-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8d64-133">Response</span></span>
<span data-ttu-id="d8d64-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8d64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




