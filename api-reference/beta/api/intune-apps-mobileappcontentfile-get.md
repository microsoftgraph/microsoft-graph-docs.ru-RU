---
title: Get mobileAppContentFile
description: Чтение свойств и связей объекта mobileAppContentFile.
author: tfitzmac
ms.openlocfilehash: 3f72f132b8c6e1c1b08a487abd95391f639683a7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350598"
---
# <a name="get-mobileappcontentfile"></a><span data-ttu-id="2e5fb-103">Get mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="2e5fb-103">Get mobileAppContentFile</span></span>

> <span data-ttu-id="2e5fb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2e5fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e5fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e5fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e5fb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2e5fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e5fb-107">Чтение свойств и связей объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="2e5fb-107">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e5fb-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2e5fb-108">Prerequisites</span></span>
<span data-ttu-id="2e5fb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e5fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e5fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e5fb-111">Permission type</span></span>|<span data-ttu-id="2e5fb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e5fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e5fb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e5fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e5fb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5fb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2e5fb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e5fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e5fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e5fb-116">Not supported.</span></span>|
|<span data-ttu-id="2e5fb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e5fb-117">Application</span></span>|<span data-ttu-id="2e5fb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e5fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e5fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e5fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e5fb-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e5fb-120">Optional query parameters</span></span>
<span data-ttu-id="2e5fb-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2e5fb-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2e5fb-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e5fb-122">Request headers</span></span>
|<span data-ttu-id="2e5fb-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e5fb-123">Header</span></span>|<span data-ttu-id="2e5fb-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2e5fb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e5fb-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e5fb-125">Authorization</span></span>|<span data-ttu-id="2e5fb-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2e5fb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e5fb-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2e5fb-127">Accept</span></span>|<span data-ttu-id="2e5fb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2e5fb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e5fb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e5fb-129">Request body</span></span>
<span data-ttu-id="2e5fb-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e5fb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e5fb-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e5fb-131">Response</span></span>
<span data-ttu-id="2e5fb-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2e5fb-132">If successful, this method returns a `200 OK` response code and [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e5fb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2e5fb-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e5fb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e5fb-134">Request</span></span>
<span data-ttu-id="2e5fb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e5fb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a><span data-ttu-id="2e5fb-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e5fb-136">Response</span></span>
<span data-ttu-id="2e5fb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2e5fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 548

{
  "value": {
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
}
```





