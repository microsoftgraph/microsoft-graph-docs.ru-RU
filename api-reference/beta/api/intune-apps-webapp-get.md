---
title: Get webApp
description: Чтение свойств и связей объекта webApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2b575190ba9df1525fc7851c44f7d3c2d643bc1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960337"
---
# <a name="get-webapp"></a><span data-ttu-id="b0218-103">Get webApp</span><span class="sxs-lookup"><span data-stu-id="b0218-103">Get webApp</span></span>

> <span data-ttu-id="b0218-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0218-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0218-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0218-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0218-106">Чтение свойств и связей объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0218-106">Read properties and relationships of the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0218-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b0218-107">Prerequisites</span></span>
<span data-ttu-id="b0218-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0218-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0218-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0218-110">Permission type</span></span>|<span data-ttu-id="b0218-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0218-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0218-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0218-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0218-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0218-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b0218-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0218-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0218-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0218-115">Not supported.</span></span>|
|<span data-ttu-id="b0218-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0218-116">Application</span></span>|<span data-ttu-id="b0218-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0218-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0218-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0218-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0218-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0218-119">Optional query parameters</span></span>
<span data-ttu-id="b0218-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b0218-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0218-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0218-121">Request headers</span></span>
|<span data-ttu-id="b0218-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0218-122">Header</span></span>|<span data-ttu-id="b0218-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b0218-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0218-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0218-124">Authorization</span></span>|<span data-ttu-id="b0218-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0218-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0218-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b0218-126">Accept</span></span>|<span data-ttu-id="b0218-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b0218-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0218-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0218-128">Request body</span></span>
<span data-ttu-id="b0218-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0218-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0218-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0218-130">Response</span></span>
<span data-ttu-id="b0218-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [webApp](../resources/intune-apps-webapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b0218-131">If successful, this method returns a `200 OK` response code and [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0218-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b0218-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0218-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0218-133">Request</span></span>
<span data-ttu-id="b0218-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0218-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="b0218-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0218-135">Response</span></span>
<span data-ttu-id="b0218-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0218-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1024

{
  "value": {
    "@odata.type": "#microsoft.graph.webApp",
    "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
    "appUrl": "https://example.com/appUrl/",
    "useManagedBrowser": true
  }
}
```





