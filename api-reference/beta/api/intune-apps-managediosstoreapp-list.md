---
title: Перечисление объектов managedIOSStoreApp
description: Список свойств и связей объектов managedIOSStoreApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: db180363c26a0f12b5bf336ca1938522c3eeeb4a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405151"
---
# <a name="list-managediosstoreapps"></a><span data-ttu-id="bb747-103">Перечисление объектов managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="bb747-103">List managedIOSStoreApps</span></span>

> <span data-ttu-id="bb747-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bb747-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bb747-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb747-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb747-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb747-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb747-107">Список свойств и связей объектов [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb747-107">List properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb747-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bb747-108">Prerequisites</span></span>
<span data-ttu-id="bb747-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb747-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bb747-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb747-111">Permission type</span></span>|<span data-ttu-id="bb747-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb747-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb747-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb747-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb747-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb747-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bb747-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb747-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb747-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb747-116">Not supported.</span></span>|
|<span data-ttu-id="bb747-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb747-117">Application</span></span>|<span data-ttu-id="bb747-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb747-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb747-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb747-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bb747-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb747-120">Request headers</span></span>
|<span data-ttu-id="bb747-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb747-121">Header</span></span>|<span data-ttu-id="bb747-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bb747-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb747-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb747-123">Authorization</span></span>|<span data-ttu-id="bb747-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bb747-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb747-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bb747-125">Accept</span></span>|<span data-ttu-id="bb747-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb747-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb747-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb747-127">Request body</span></span>
<span data-ttu-id="bb747-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb747-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb747-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb747-129">Response</span></span>
<span data-ttu-id="bb747-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb747-130">If successful, this method returns a `200 OK` response code and a collection of [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb747-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bb747-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb747-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb747-132">Request</span></span>
<span data-ttu-id="bb747-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb747-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="bb747-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb747-134">Response</span></span>
<span data-ttu-id="bb747-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bb747-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1560

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedIOSStoreApp",
      "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
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
        "v12_0": true
      }
    }
  ]
}
```




