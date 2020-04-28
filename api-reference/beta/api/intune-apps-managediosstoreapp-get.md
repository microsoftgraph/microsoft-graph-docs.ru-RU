---
title: Get managedIOSStoreApp
description: Чтение свойств и связей объекта managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7196d055eadabfddc7f0f160afaab61fa4ddaa14
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43405618"
---
# <a name="get-managediosstoreapp"></a><span data-ttu-id="52422-103">Get managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="52422-103">Get managedIOSStoreApp</span></span>

<span data-ttu-id="52422-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52422-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52422-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52422-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52422-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52422-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52422-107">Чтение свойств и связей объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="52422-107">Read properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52422-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="52422-108">Prerequisites</span></span>
<span data-ttu-id="52422-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52422-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52422-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52422-111">Permission type</span></span>|<span data-ttu-id="52422-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52422-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52422-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52422-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52422-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="52422-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="52422-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52422-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52422-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52422-116">Not supported.</span></span>|
|<span data-ttu-id="52422-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52422-117">Application</span></span>|<span data-ttu-id="52422-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="52422-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52422-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52422-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52422-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="52422-120">Optional query parameters</span></span>
<span data-ttu-id="52422-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="52422-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52422-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52422-122">Request headers</span></span>
|<span data-ttu-id="52422-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52422-123">Header</span></span>|<span data-ttu-id="52422-124">Значение</span><span class="sxs-lookup"><span data-stu-id="52422-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52422-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52422-125">Authorization</span></span>|<span data-ttu-id="52422-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52422-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52422-127">Accept</span><span class="sxs-lookup"><span data-stu-id="52422-127">Accept</span></span>|<span data-ttu-id="52422-128">application/json</span><span class="sxs-lookup"><span data-stu-id="52422-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52422-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="52422-129">Request body</span></span>
<span data-ttu-id="52422-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52422-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52422-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="52422-131">Response</span></span>
<span data-ttu-id="52422-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="52422-132">If successful, this method returns a `200 OK` response code and [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52422-133">Пример</span><span class="sxs-lookup"><span data-stu-id="52422-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="52422-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="52422-134">Request</span></span>
<span data-ttu-id="52422-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52422-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="52422-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="52422-136">Response</span></span>
<span data-ttu-id="52422-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52422-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1515

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
      "v12_0": true,
      "v13_0": true
    }
  }
}
```



