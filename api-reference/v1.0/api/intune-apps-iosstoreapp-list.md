---
title: Перечисление объектов iosStoreApp
description: Список свойств и связей объектов iosStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2ded7142459f8b0b211ed757c64e9bc0157f911
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577373"
---
# <a name="list-iosstoreapps"></a><span data-ttu-id="fb51a-103">Перечисление объектов iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="fb51a-103">List iosStoreApps</span></span>

> <span data-ttu-id="fb51a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb51a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb51a-105">Список свойств и связей объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb51a-105">List properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb51a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fb51a-106">Prerequisites</span></span>
<span data-ttu-id="fb51a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb51a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb51a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb51a-109">Permission type</span></span>|<span data-ttu-id="fb51a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb51a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb51a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb51a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb51a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb51a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fb51a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb51a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb51a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb51a-114">Not supported.</span></span>|
|<span data-ttu-id="fb51a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb51a-115">Application</span></span>|<span data-ttu-id="fb51a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb51a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb51a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb51a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fb51a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb51a-118">Request headers</span></span>
|<span data-ttu-id="fb51a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb51a-119">Header</span></span>|<span data-ttu-id="fb51a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fb51a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb51a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb51a-121">Authorization</span></span>|<span data-ttu-id="fb51a-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb51a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb51a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fb51a-123">Accept</span></span>|<span data-ttu-id="fb51a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fb51a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb51a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb51a-125">Request body</span></span>
<span data-ttu-id="fb51a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb51a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb51a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb51a-127">Response</span></span>
<span data-ttu-id="fb51a-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb51a-128">If successful, this method returns a `200 OK` response code and a collection of [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb51a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fb51a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb51a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb51a-130">Request</span></span>
<span data-ttu-id="fb51a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb51a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="fb51a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb51a-132">Response</span></span>
<span data-ttu-id="fb51a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb51a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1347

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
      "publishingState": "processing",
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



