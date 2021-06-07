---
title: Get iosDeviceFeaturesConfiguration
description: Чтение свойств и связей объекта iosDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d61486a55731e74da88553e3d73ec53c8a90685
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747965"
---
# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="3db63-103">Get iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="3db63-103">Get iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="3db63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3db63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3db63-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3db63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3db63-106">Чтение свойств и связей объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3db63-106">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3db63-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3db63-107">Prerequisites</span></span>
<span data-ttu-id="3db63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3db63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3db63-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3db63-110">Permission type</span></span>|<span data-ttu-id="3db63-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3db63-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3db63-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3db63-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3db63-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3db63-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3db63-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3db63-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3db63-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3db63-115">Not supported.</span></span>|
|<span data-ttu-id="3db63-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3db63-116">Application</span></span>|<span data-ttu-id="3db63-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3db63-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3db63-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3db63-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3db63-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3db63-119">Optional query parameters</span></span>
<span data-ttu-id="3db63-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3db63-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3db63-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3db63-121">Request headers</span></span>
|<span data-ttu-id="3db63-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3db63-122">Header</span></span>|<span data-ttu-id="3db63-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3db63-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3db63-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3db63-124">Authorization</span></span>|<span data-ttu-id="3db63-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3db63-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3db63-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3db63-126">Accept</span></span>|<span data-ttu-id="3db63-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3db63-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3db63-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3db63-128">Request body</span></span>
<span data-ttu-id="3db63-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3db63-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3db63-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3db63-130">Response</span></span>
<span data-ttu-id="3db63-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3db63-131">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3db63-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3db63-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3db63-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3db63-133">Request</span></span>
<span data-ttu-id="3db63-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3db63-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3db63-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3db63-135">Response</span></span>
<span data-ttu-id="3db63-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3db63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




