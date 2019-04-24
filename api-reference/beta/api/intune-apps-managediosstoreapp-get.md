---
title: Get managedIOSStoreApp
description: Чтение свойств и связей объекта managedIOSStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a64ca7b2a7d1c20ef824cf6b98ca103208ac3c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32491657"
---
# <a name="get-managediosstoreapp"></a><span data-ttu-id="64e81-103">Get managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="64e81-103">Get managedIOSStoreApp</span></span>

> <span data-ttu-id="64e81-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64e81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64e81-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64e81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64e81-106">Чтение свойств и связей объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="64e81-106">Read properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64e81-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="64e81-107">Prerequisites</span></span>
<span data-ttu-id="64e81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64e81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64e81-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64e81-110">Permission type</span></span>|<span data-ttu-id="64e81-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64e81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64e81-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64e81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64e81-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64e81-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="64e81-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64e81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64e81-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64e81-115">Not supported.</span></span>|
|<span data-ttu-id="64e81-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64e81-116">Application</span></span>|<span data-ttu-id="64e81-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64e81-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64e81-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64e81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64e81-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64e81-119">Optional query parameters</span></span>
<span data-ttu-id="64e81-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64e81-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64e81-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64e81-121">Request headers</span></span>
|<span data-ttu-id="64e81-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64e81-122">Header</span></span>|<span data-ttu-id="64e81-123">Значение</span><span class="sxs-lookup"><span data-stu-id="64e81-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64e81-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64e81-124">Authorization</span></span>|<span data-ttu-id="64e81-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64e81-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64e81-126">Accept</span><span class="sxs-lookup"><span data-stu-id="64e81-126">Accept</span></span>|<span data-ttu-id="64e81-127">application/json</span><span class="sxs-lookup"><span data-stu-id="64e81-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64e81-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64e81-128">Request body</span></span>
<span data-ttu-id="64e81-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64e81-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64e81-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="64e81-130">Response</span></span>
<span data-ttu-id="64e81-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="64e81-131">If successful, this method returns a `200 OK` response code and [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64e81-132">Пример</span><span class="sxs-lookup"><span data-stu-id="64e81-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="64e81-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="64e81-133">Request</span></span>
<span data-ttu-id="64e81-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64e81-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="64e81-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="64e81-135">Response</span></span>
<span data-ttu-id="64e81-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64e81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1493

{
  "value": {
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
    "dependentAppCount": 1,
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
}
```





