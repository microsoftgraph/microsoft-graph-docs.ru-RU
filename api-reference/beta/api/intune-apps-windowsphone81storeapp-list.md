---
title: Список windowsPhone81StoreApps
description: Список свойств и связей объектов windowsPhone81StoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 748ba568c959e2007fc0d7cf86b59c448cac265d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806267"
---
# <a name="list-windowsphone81storeapps"></a><span data-ttu-id="f8fc3-103">Список windowsPhone81StoreApps</span><span class="sxs-lookup"><span data-stu-id="f8fc3-103">List windowsPhone81StoreApps</span></span>

> <span data-ttu-id="f8fc3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8fc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8fc3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8fc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8fc3-106">Список свойств и связей объектов [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f8fc3-106">List properties and relationships of the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8fc3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f8fc3-107">Prerequisites</span></span>
<span data-ttu-id="f8fc3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8fc3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8fc3-110">Permission type</span></span>|<span data-ttu-id="f8fc3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8fc3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8fc3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8fc3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8fc3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8fc3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f8fc3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8fc3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8fc3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8fc3-115">Not supported.</span></span>|
|<span data-ttu-id="f8fc3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8fc3-116">Application</span></span>|<span data-ttu-id="f8fc3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8fc3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8fc3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8fc3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f8fc3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8fc3-119">Request headers</span></span>
|<span data-ttu-id="f8fc3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8fc3-120">Header</span></span>|<span data-ttu-id="f8fc3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f8fc3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8fc3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8fc3-122">Authorization</span></span>|<span data-ttu-id="f8fc3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8fc3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8fc3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f8fc3-124">Accept</span></span>|<span data-ttu-id="f8fc3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8fc3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8fc3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8fc3-126">Request body</span></span>
<span data-ttu-id="f8fc3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8fc3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8fc3-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8fc3-128">Response</span></span>
<span data-ttu-id="f8fc3-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8fc3-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8fc3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f8fc3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8fc3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8fc3-131">Request</span></span>
<span data-ttu-id="f8fc3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8fc3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f8fc3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8fc3-133">Response</span></span>
<span data-ttu-id="f8fc3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8fc3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1084

{
  "value": [
    {
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
  ]
}
```





