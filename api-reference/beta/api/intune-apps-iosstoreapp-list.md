---
title: Перечисление объектов iosStoreApp
description: Список свойств и связей объектов iosStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aab0914c94767bf0705dcac38d377c27d5a47007
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445633"
---
# <a name="list-iosstoreapps"></a><span data-ttu-id="45d58-103">Перечисление объектов iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="45d58-103">List iosStoreApps</span></span>

<span data-ttu-id="45d58-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="45d58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45d58-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45d58-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45d58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45d58-107">Список свойств и связей объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="45d58-107">List properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45d58-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="45d58-108">Prerequisites</span></span>
<span data-ttu-id="45d58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45d58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45d58-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45d58-111">Permission type</span></span>|<span data-ttu-id="45d58-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45d58-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45d58-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45d58-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45d58-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45d58-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="45d58-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45d58-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45d58-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d58-116">Not supported.</span></span>|
|<span data-ttu-id="45d58-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45d58-117">Application</span></span>|<span data-ttu-id="45d58-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45d58-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45d58-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45d58-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="45d58-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45d58-120">Request headers</span></span>
|<span data-ttu-id="45d58-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45d58-121">Header</span></span>|<span data-ttu-id="45d58-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45d58-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45d58-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45d58-123">Authorization</span></span>|<span data-ttu-id="45d58-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45d58-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45d58-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45d58-125">Accept</span></span>|<span data-ttu-id="45d58-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45d58-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45d58-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45d58-127">Request body</span></span>
<span data-ttu-id="45d58-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45d58-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45d58-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="45d58-129">Response</span></span>
<span data-ttu-id="45d58-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45d58-130">If successful, this method returns a `200 OK` response code and a collection of [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45d58-131">Пример</span><span class="sxs-lookup"><span data-stu-id="45d58-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="45d58-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="45d58-132">Request</span></span>
<span data-ttu-id="45d58-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45d58-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="45d58-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="45d58-134">Response</span></span>
<span data-ttu-id="45d58-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45d58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1529

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosStoreApp",
      "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "dependentAppCount": 1,
      "bundleId": "Bundle Id value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
        "v8_0": true,
        "v9_0": true,
        "v10_0": true,
        "v11_0": true,
        "v12_0": true,
        "v13_0": true
      }
    }
  ]
}
```





