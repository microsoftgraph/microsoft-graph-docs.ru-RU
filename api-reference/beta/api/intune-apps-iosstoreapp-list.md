---
title: Перечисление объектов iosStoreApp
description: Список свойств и связей объектов iosStoreApp.
author: tfitzmac
ms.openlocfilehash: 298925323466290945798f3a99a1433ed65f14d3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341512"
---
# <a name="list-iosstoreapps"></a><span data-ttu-id="8f515-103">Перечисление объектов iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="8f515-103">List iosStoreApps</span></span>

> <span data-ttu-id="8f515-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f515-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f515-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f515-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f515-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8f515-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f515-107">Список свойств и связей объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f515-107">List properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f515-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8f515-108">Prerequisites</span></span>
<span data-ttu-id="8f515-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f515-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f515-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f515-111">Permission type</span></span>|<span data-ttu-id="8f515-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f515-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f515-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f515-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f515-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f515-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8f515-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f515-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f515-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f515-116">Not supported.</span></span>|
|<span data-ttu-id="8f515-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f515-117">Application</span></span>|<span data-ttu-id="8f515-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f515-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f515-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f515-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8f515-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f515-120">Request headers</span></span>
|<span data-ttu-id="8f515-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f515-121">Header</span></span>|<span data-ttu-id="8f515-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8f515-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f515-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f515-123">Authorization</span></span>|<span data-ttu-id="8f515-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8f515-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f515-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f515-125">Accept</span></span>|<span data-ttu-id="8f515-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f515-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f515-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f515-127">Request body</span></span>
<span data-ttu-id="8f515-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f515-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f515-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f515-129">Response</span></span>
<span data-ttu-id="8f515-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f515-130">If successful, this method returns a `200 OK` response code and a collection of [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f515-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8f515-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f515-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f515-132">Request</span></span>
<span data-ttu-id="8f515-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f515-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="8f515-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f515-134">Response</span></span>
<span data-ttu-id="8f515-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8f515-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1373

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





