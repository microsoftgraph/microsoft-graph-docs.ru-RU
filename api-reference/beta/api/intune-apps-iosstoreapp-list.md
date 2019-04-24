---
title: Перечисление объектов iosStoreApp
description: Список свойств и связей объектов iosStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32b8a5fdd7305cd1187d52a43997430c7a633815
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32495654"
---
# <a name="list-iosstoreapps"></a><span data-ttu-id="4928e-103">Перечисление объектов iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="4928e-103">List iosStoreApps</span></span>

> <span data-ttu-id="4928e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4928e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4928e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4928e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4928e-106">Список свойств и связей объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4928e-106">List properties and relationships of the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4928e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4928e-107">Prerequisites</span></span>
<span data-ttu-id="4928e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4928e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4928e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4928e-110">Permission type</span></span>|<span data-ttu-id="4928e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4928e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4928e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4928e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4928e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4928e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4928e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4928e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4928e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4928e-115">Not supported.</span></span>|
|<span data-ttu-id="4928e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4928e-116">Application</span></span>|<span data-ttu-id="4928e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4928e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4928e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4928e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4928e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4928e-119">Request headers</span></span>
|<span data-ttu-id="4928e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4928e-120">Header</span></span>|<span data-ttu-id="4928e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4928e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4928e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4928e-122">Authorization</span></span>|<span data-ttu-id="4928e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4928e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4928e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4928e-124">Accept</span></span>|<span data-ttu-id="4928e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4928e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4928e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4928e-126">Request body</span></span>
<span data-ttu-id="4928e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4928e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4928e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4928e-128">Response</span></span>
<span data-ttu-id="4928e-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4928e-129">If successful, this method returns a `200 OK` response code and a collection of [iosStoreApp](../resources/intune-apps-iosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4928e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4928e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4928e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4928e-131">Request</span></span>
<span data-ttu-id="4928e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4928e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="4928e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4928e-133">Response</span></span>
<span data-ttu-id="4928e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4928e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1505

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
  ]
}
```





