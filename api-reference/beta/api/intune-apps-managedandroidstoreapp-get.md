---
title: Get managedAndroidStoreApp
description: Чтение свойств и связей объекта managedAndroidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d03e9fa741251cc77e1717757f70418813bd46bc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153286"
---
# <a name="get-managedandroidstoreapp"></a><span data-ttu-id="3451c-103">Get managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="3451c-103">Get managedAndroidStoreApp</span></span>

> <span data-ttu-id="3451c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3451c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3451c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3451c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3451c-106">Чтение свойств и связей объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="3451c-106">Read properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3451c-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3451c-107">Prerequisites</span></span>
<span data-ttu-id="3451c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3451c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3451c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3451c-110">Permission type</span></span>|<span data-ttu-id="3451c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3451c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3451c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3451c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3451c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3451c-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3451c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3451c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3451c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3451c-115">Not supported.</span></span>|
|<span data-ttu-id="3451c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3451c-116">Application</span></span>|<span data-ttu-id="3451c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3451c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3451c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3451c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3451c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3451c-119">Optional query parameters</span></span>
<span data-ttu-id="3451c-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3451c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3451c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3451c-121">Request headers</span></span>
|<span data-ttu-id="3451c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3451c-122">Header</span></span>|<span data-ttu-id="3451c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3451c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3451c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3451c-124">Authorization</span></span>|<span data-ttu-id="3451c-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3451c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3451c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3451c-126">Accept</span></span>|<span data-ttu-id="3451c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3451c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3451c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3451c-128">Request body</span></span>
<span data-ttu-id="3451c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3451c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3451c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3451c-130">Response</span></span>
<span data-ttu-id="3451c-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3451c-131">If successful, this method returns a `200 OK` response code and [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3451c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3451c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3451c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3451c-133">Request</span></span>
<span data-ttu-id="3451c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3451c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="3451c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3451c-135">Response</span></span>
<span data-ttu-id="3451c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3451c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1518

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
    "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
    "packageId": "Package Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
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
    }
  }
}
```




