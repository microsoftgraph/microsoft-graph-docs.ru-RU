---
title: Перечисление объектов webApp
description: Список свойств и связей объектов webApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e0f5897a2efb0d31578021c4a69f7e2453d48f7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257815"
---
# <a name="list-webapps"></a><span data-ttu-id="19f02-103">Перечисление объектов webApp</span><span class="sxs-lookup"><span data-stu-id="19f02-103">List webApps</span></span>

> <span data-ttu-id="19f02-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19f02-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19f02-105">Список свойств и связей объектов [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="19f02-105">List properties and relationships of the [webApp](../resources/intune-apps-webapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19f02-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="19f02-106">Prerequisites</span></span>
<span data-ttu-id="19f02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="19f02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="19f02-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19f02-109">Permission type</span></span>|<span data-ttu-id="19f02-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19f02-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19f02-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19f02-111">Delegated (work or school account)</span></span>|<span data-ttu-id="19f02-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="19f02-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="19f02-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19f02-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19f02-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19f02-114">Not supported.</span></span>|
|<span data-ttu-id="19f02-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19f02-115">Application</span></span>|<span data-ttu-id="19f02-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19f02-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19f02-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19f02-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="19f02-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19f02-118">Request headers</span></span>
|<span data-ttu-id="19f02-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19f02-119">Header</span></span>|<span data-ttu-id="19f02-120">Значение</span><span class="sxs-lookup"><span data-stu-id="19f02-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19f02-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19f02-121">Authorization</span></span>|<span data-ttu-id="19f02-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="19f02-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19f02-123">Accept</span><span class="sxs-lookup"><span data-stu-id="19f02-123">Accept</span></span>|<span data-ttu-id="19f02-124">application/json</span><span class="sxs-lookup"><span data-stu-id="19f02-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19f02-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19f02-125">Request body</span></span>
<span data-ttu-id="19f02-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19f02-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19f02-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="19f02-127">Response</span></span>
<span data-ttu-id="19f02-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [webApp](../resources/intune-apps-webapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19f02-128">If successful, this method returns a `200 OK` response code and a collection of [webApp](../resources/intune-apps-webapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19f02-129">Пример</span><span class="sxs-lookup"><span data-stu-id="19f02-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="19f02-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="19f02-130">Request</span></span>
<span data-ttu-id="19f02-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19f02-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="19f02-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="19f02-132">Response</span></span>
<span data-ttu-id="19f02-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19f02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 934

{
  "value": [
    {
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
      "publishingState": "processing",
      "appUrl": "https://example.com/appUrl/",
      "useManagedBrowser": true
    }
  ]
}
```



