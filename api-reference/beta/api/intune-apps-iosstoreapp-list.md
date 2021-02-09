---
title: Перечисление объектов iosStoreApp
description: Список свойств и связей объектов iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2e3243daa9711b3a9e97f455f76d47011903c3fd
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157367"
---
# <a name="list-iosstoreapps"></a><span data-ttu-id="6b224-103">Перечисление объектов iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="6b224-103">List iosStoreApps</span></span>

<span data-ttu-id="6b224-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b224-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b224-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b224-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b224-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b224-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b224-107">Список свойств и связей объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="6b224-107">List properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b224-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6b224-108">Prerequisites</span></span>
<span data-ttu-id="6b224-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b224-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b224-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b224-111">Permission type</span></span>|<span data-ttu-id="6b224-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b224-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b224-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b224-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b224-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b224-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6b224-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b224-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b224-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b224-116">Not supported.</span></span>|
|<span data-ttu-id="6b224-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b224-117">Application</span></span>|<span data-ttu-id="6b224-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b224-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b224-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b224-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6b224-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6b224-120">Request headers</span></span>
|<span data-ttu-id="6b224-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b224-121">Header</span></span>|<span data-ttu-id="6b224-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6b224-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b224-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b224-123">Authorization</span></span>|<span data-ttu-id="6b224-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b224-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b224-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6b224-125">Accept</span></span>|<span data-ttu-id="6b224-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b224-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b224-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b224-127">Request body</span></span>
<span data-ttu-id="6b224-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b224-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b224-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b224-129">Response</span></span>
<span data-ttu-id="6b224-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b224-130">If successful, this method returns a `200 OK` response code and a collection of [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b224-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6b224-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b224-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b224-132">Request</span></span>
<span data-ttu-id="6b224-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b224-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="6b224-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b224-134">Response</span></span>
<span data-ttu-id="6b224-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b224-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1618

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosStoreApp",
      "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
      "supersedingAppCount": 3,
      "supersededAppCount": 2,
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
        "v13_0": true,
        "v14_0": true
      }
    }
  ]
}
```




