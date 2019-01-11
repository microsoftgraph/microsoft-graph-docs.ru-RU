---
title: Перечисление объектов mobileAppContentFile
description: Список свойств и связей объектов mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e1354f47d668a15f7dc2877b87558f14c4c2a86f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891639"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="0094b-103">Перечисление объектов mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0094b-103">List mobileAppContentFiles</span></span>

> <span data-ttu-id="0094b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0094b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0094b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0094b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0094b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0094b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0094b-107">Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="0094b-107">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0094b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0094b-108">Prerequisites</span></span>
<span data-ttu-id="0094b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0094b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0094b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0094b-111">Permission type</span></span>|<span data-ttu-id="0094b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0094b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0094b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0094b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0094b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0094b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0094b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0094b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0094b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0094b-116">Not supported.</span></span>|
|<span data-ttu-id="0094b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0094b-117">Application</span></span>|<span data-ttu-id="0094b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0094b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0094b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0094b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="0094b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0094b-120">Request headers</span></span>
|<span data-ttu-id="0094b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0094b-121">Header</span></span>|<span data-ttu-id="0094b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0094b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0094b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0094b-123">Authorization</span></span>|<span data-ttu-id="0094b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0094b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0094b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0094b-125">Accept</span></span>|<span data-ttu-id="0094b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0094b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0094b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0094b-127">Request body</span></span>
<span data-ttu-id="0094b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0094b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0094b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0094b-129">Response</span></span>
<span data-ttu-id="0094b-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0094b-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0094b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0094b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0094b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0094b-132">Request</span></span>
<span data-ttu-id="0094b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0094b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="0094b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0094b-134">Response</span></span>
<span data-ttu-id="0094b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0094b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 588

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContentFile",
      "azureStorageUri": "Azure Storage Uri value",
      "isCommitted": true,
      "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "name": "Name value",
      "size": 4,
      "sizeEncrypted": 13,
      "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
      "manifest": "bWFuaWZlc3Q=",
      "uploadState": "transientError",
      "isFrameworkFile": true,
      "isDependency": true
    }
  ]
}
```





