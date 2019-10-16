---
title: Перечисление объектов managedIOSStoreApp
description: Список свойств и связей объектов managedIOSStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c2b95f9818eb056b3e9f82f5b8f48d5e180c2bbd
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535214"
---
# <a name="list-managediosstoreapps"></a><span data-ttu-id="30f71-103">Перечисление объектов managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="30f71-103">List managedIOSStoreApps</span></span>

> <span data-ttu-id="30f71-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30f71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30f71-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30f71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30f71-106">Список свойств и связей объектов [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="30f71-106">List properties and relationships of the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30f71-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="30f71-107">Prerequisites</span></span>
<span data-ttu-id="30f71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30f71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30f71-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30f71-110">Permission type</span></span>|<span data-ttu-id="30f71-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30f71-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30f71-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30f71-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30f71-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="30f71-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="30f71-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30f71-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30f71-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30f71-115">Not supported.</span></span>|
|<span data-ttu-id="30f71-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="30f71-116">Application</span></span>|<span data-ttu-id="30f71-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="30f71-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30f71-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30f71-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="30f71-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30f71-119">Request headers</span></span>
|<span data-ttu-id="30f71-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30f71-120">Header</span></span>|<span data-ttu-id="30f71-121">Значение</span><span class="sxs-lookup"><span data-stu-id="30f71-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30f71-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30f71-122">Authorization</span></span>|<span data-ttu-id="30f71-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30f71-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30f71-124">Accept</span><span class="sxs-lookup"><span data-stu-id="30f71-124">Accept</span></span>|<span data-ttu-id="30f71-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30f71-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30f71-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30f71-126">Request body</span></span>
<span data-ttu-id="30f71-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30f71-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30f71-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="30f71-128">Response</span></span>
<span data-ttu-id="30f71-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30f71-129">If successful, this method returns a `200 OK` response code and a collection of [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30f71-130">Пример</span><span class="sxs-lookup"><span data-stu-id="30f71-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="30f71-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="30f71-131">Request</span></span>
<span data-ttu-id="30f71-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30f71-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="30f71-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="30f71-133">Response</span></span>
<span data-ttu-id="30f71-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30f71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1615

{
  "value": [
    {
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
  ]
}
```






