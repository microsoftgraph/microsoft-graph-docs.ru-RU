---
title: Получение windowsPhone81StoreApp
description: Чтение свойств и связей объекта windowsPhone81StoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 001a0448c5a6bd3a17b3bc56af30aae0e5b22191
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322319"
---
# <a name="get-windowsphone81storeapp"></a><span data-ttu-id="e77e4-103">Получение windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="e77e4-103">Get windowsPhone81StoreApp</span></span>

> <span data-ttu-id="e77e4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e77e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e77e4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e77e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e77e4-106">Чтение свойств и связей объекта [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e77e4-106">Read properties and relationships of the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e77e4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e77e4-107">Prerequisites</span></span>
<span data-ttu-id="e77e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e77e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e77e4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e77e4-110">Permission type</span></span>|<span data-ttu-id="e77e4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e77e4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e77e4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e77e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e77e4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e77e4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e77e4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e77e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e77e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e77e4-115">Not supported.</span></span>|
|<span data-ttu-id="e77e4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e77e4-116">Application</span></span>|<span data-ttu-id="e77e4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e77e4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e77e4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e77e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e77e4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e77e4-119">Optional query parameters</span></span>
<span data-ttu-id="e77e4-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e77e4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e77e4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e77e4-121">Request headers</span></span>
|<span data-ttu-id="e77e4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e77e4-122">Header</span></span>|<span data-ttu-id="e77e4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e77e4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e77e4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e77e4-124">Authorization</span></span>|<span data-ttu-id="e77e4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e77e4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e77e4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e77e4-126">Accept</span></span>|<span data-ttu-id="e77e4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e77e4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e77e4-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e77e4-128">Request body</span></span>
<span data-ttu-id="e77e4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e77e4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e77e4-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e77e4-130">Response</span></span>
<span data-ttu-id="e77e4-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e77e4-131">If successful, this method returns a `200 OK` response code and [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e77e4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e77e4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e77e4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e77e4-133">Request</span></span>
<span data-ttu-id="e77e4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e77e4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="e77e4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e77e4-135">Response</span></span>
<span data-ttu-id="e77e4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e77e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1018

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
    "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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
    "appStoreUrl": "https://example.com/appStoreUrl/"
  }
}
```






