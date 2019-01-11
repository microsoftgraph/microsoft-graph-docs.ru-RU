---
title: Перечисление объектов managedAndroidLobApp
description: Список свойств и связей объектов managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8b2a729af3cd197c7ad2f7de46a2e5a39721488b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874643"
---
# <a name="list-managedandroidlobapps"></a><span data-ttu-id="bb0ad-103">Перечисление объектов managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="bb0ad-103">List managedAndroidLobApps</span></span>

> <span data-ttu-id="bb0ad-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb0ad-105">Список свойств и связей объектов [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0ad-105">List properties and relationships of the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb0ad-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bb0ad-106">Prerequisites</span></span>
<span data-ttu-id="bb0ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb0ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb0ad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb0ad-109">Permission type</span></span>|<span data-ttu-id="bb0ad-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb0ad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb0ad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb0ad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb0ad-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb0ad-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bb0ad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb0ad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb0ad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-114">Not supported.</span></span>|
|<span data-ttu-id="bb0ad-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb0ad-115">Application</span></span>|<span data-ttu-id="bb0ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb0ad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb0ad-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bb0ad-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb0ad-118">Request headers</span></span>
|<span data-ttu-id="bb0ad-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb0ad-119">Header</span></span>|<span data-ttu-id="bb0ad-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bb0ad-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb0ad-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb0ad-121">Authorization</span></span>|<span data-ttu-id="bb0ad-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bb0ad-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb0ad-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bb0ad-123">Accept</span></span>|<span data-ttu-id="bb0ad-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb0ad-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb0ad-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bb0ad-125">Request body</span></span>
<span data-ttu-id="bb0ad-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb0ad-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb0ad-127">Response</span></span>
<span data-ttu-id="bb0ad-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-128">If successful, this method returns a `200 OK` response code and a collection of [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb0ad-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bb0ad-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb0ad-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb0ad-130">Request</span></span>
<span data-ttu-id="bb0ad-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="bb0ad-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb0ad-132">Response</span></span>
<span data-ttu-id="bb0ad-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1510

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAndroidLobApp",
      "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "packageId": "Package Id value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
        "v4_0": true,
        "v4_0_3": true,
        "v4_1": true,
        "v4_2": true,
        "v4_3": true,
        "v4_4": true,
        "v5_0": true,
        "v5_1": true
      },
      "versionName": "Version Name value",
      "versionCode": "Version Code value"
    }
  ]
}
```



