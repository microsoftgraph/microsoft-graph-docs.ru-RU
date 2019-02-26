---
title: Перечисление объектов managedAndroidLobApp
description: Список свойств и связей объектов managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d0a6a8c0459cea3d408b8e535263bc182be2dc6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254641"
---
# <a name="list-managedandroidlobapps"></a><span data-ttu-id="08dca-103">Перечисление объектов managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="08dca-103">List managedAndroidLobApps</span></span>

> <span data-ttu-id="08dca-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08dca-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08dca-105">Список свойств и связей объектов [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="08dca-105">List properties and relationships of the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08dca-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="08dca-106">Prerequisites</span></span>
<span data-ttu-id="08dca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="08dca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="08dca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08dca-109">Permission type</span></span>|<span data-ttu-id="08dca-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08dca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08dca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08dca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="08dca-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="08dca-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="08dca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08dca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08dca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08dca-114">Not supported.</span></span>|
|<span data-ttu-id="08dca-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08dca-115">Application</span></span>|<span data-ttu-id="08dca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08dca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08dca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08dca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="08dca-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08dca-118">Request headers</span></span>
|<span data-ttu-id="08dca-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08dca-119">Header</span></span>|<span data-ttu-id="08dca-120">Значение</span><span class="sxs-lookup"><span data-stu-id="08dca-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08dca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="08dca-121">Authorization</span></span>|<span data-ttu-id="08dca-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="08dca-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08dca-123">Accept</span><span class="sxs-lookup"><span data-stu-id="08dca-123">Accept</span></span>|<span data-ttu-id="08dca-124">application/json</span><span class="sxs-lookup"><span data-stu-id="08dca-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08dca-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08dca-125">Request body</span></span>
<span data-ttu-id="08dca-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08dca-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08dca-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="08dca-127">Response</span></span>
<span data-ttu-id="08dca-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08dca-128">If successful, this method returns a `200 OK` response code and a collection of [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08dca-129">Пример</span><span class="sxs-lookup"><span data-stu-id="08dca-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="08dca-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="08dca-130">Request</span></span>
<span data-ttu-id="08dca-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08dca-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="08dca-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="08dca-132">Response</span></span>
<span data-ttu-id="08dca-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="08dca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



