---
title: Получение Виндовсстореапп
description: Чтение свойств и связей объекта Виндовсстореапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 247ecd6d93b854b88934a1374c16ddd175006e1e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972804"
---
# <a name="get-windowsstoreapp"></a><span data-ttu-id="51fae-103">Получение Виндовсстореапп</span><span class="sxs-lookup"><span data-stu-id="51fae-103">Get windowsStoreApp</span></span>

> <span data-ttu-id="51fae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51fae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51fae-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51fae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51fae-106">Чтение свойств и связей объекта [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="51fae-106">Read properties and relationships of the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51fae-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51fae-107">Prerequisites</span></span>
<span data-ttu-id="51fae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51fae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51fae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51fae-110">Permission type</span></span>|<span data-ttu-id="51fae-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51fae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51fae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51fae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51fae-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51fae-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="51fae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51fae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51fae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51fae-115">Not supported.</span></span>|
|<span data-ttu-id="51fae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51fae-116">Application</span></span>|<span data-ttu-id="51fae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51fae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51fae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51fae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51fae-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51fae-119">Optional query parameters</span></span>
<span data-ttu-id="51fae-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51fae-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51fae-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51fae-121">Request headers</span></span>
|<span data-ttu-id="51fae-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51fae-122">Header</span></span>|<span data-ttu-id="51fae-123">Значение</span><span class="sxs-lookup"><span data-stu-id="51fae-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51fae-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51fae-124">Authorization</span></span>|<span data-ttu-id="51fae-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51fae-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51fae-126">Accept</span><span class="sxs-lookup"><span data-stu-id="51fae-126">Accept</span></span>|<span data-ttu-id="51fae-127">application/json</span><span class="sxs-lookup"><span data-stu-id="51fae-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51fae-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51fae-128">Request body</span></span>
<span data-ttu-id="51fae-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51fae-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51fae-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="51fae-130">Response</span></span>
<span data-ttu-id="51fae-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51fae-131">If successful, this method returns a `200 OK` response code and [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51fae-132">Пример</span><span class="sxs-lookup"><span data-stu-id="51fae-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="51fae-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="51fae-133">Request</span></span>
<span data-ttu-id="51fae-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51fae-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="51fae-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="51fae-135">Response</span></span>
<span data-ttu-id="51fae-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51fae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1011

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsStoreApp",
    "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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





