---
title: Get androidLobApp
description: Чтение свойств и связей объекта androidLobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 526364fbc71ed844d99adb0455348fe136c42f24
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414405"
---
# <a name="get-androidlobapp"></a><span data-ttu-id="5287e-103">Get androidLobApp</span><span class="sxs-lookup"><span data-stu-id="5287e-103">Get androidLobApp</span></span>

> <span data-ttu-id="5287e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5287e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5287e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5287e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5287e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5287e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5287e-107">Чтение свойств и связей объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5287e-107">Read properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5287e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5287e-108">Prerequisites</span></span>
<span data-ttu-id="5287e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5287e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5287e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5287e-111">Permission type</span></span>|<span data-ttu-id="5287e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5287e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5287e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5287e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5287e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5287e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5287e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5287e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5287e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5287e-116">Not supported.</span></span>|
|<span data-ttu-id="5287e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5287e-117">Application</span></span>|<span data-ttu-id="5287e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5287e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5287e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5287e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5287e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5287e-120">Optional query parameters</span></span>
<span data-ttu-id="5287e-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5287e-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5287e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5287e-122">Request headers</span></span>
|<span data-ttu-id="5287e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5287e-123">Header</span></span>|<span data-ttu-id="5287e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5287e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5287e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5287e-125">Authorization</span></span>|<span data-ttu-id="5287e-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5287e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5287e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5287e-127">Accept</span></span>|<span data-ttu-id="5287e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5287e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5287e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5287e-129">Request body</span></span>
<span data-ttu-id="5287e-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5287e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5287e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5287e-131">Response</span></span>
<span data-ttu-id="5287e-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5287e-132">If successful, this method returns a `200 OK` response code and [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5287e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5287e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5287e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5287e-134">Request</span></span>
<span data-ttu-id="5287e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5287e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="5287e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5287e-136">Response</span></span>
<span data-ttu-id="5287e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5287e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1675

{
  "value": {
    "@odata.type": "#microsoft.graph.androidLobApp",
    "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "packageId": "Package Id value",
    "identityName": "Identity Name value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true,
      "v6_0": true,
      "v7_0": true,
      "v7_1": true,
      "v8_0": true,
      "v8_1": true,
      "v9_0": true
    },
    "versionName": "Version Name value",
    "versionCode": "Version Code value",
    "identityVersion": "Identity Version value"
  }
}
```




