---
title: Get mobileAppContent
description: Чтение свойств и связей объекта mobileAppContent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29b21c116db938d400b2a9c0fa57371fd04c0cd5
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177145"
---
# <a name="get-mobileappcontent"></a><span data-ttu-id="22d95-103">Get mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="22d95-103">Get mobileAppContent</span></span>

> <span data-ttu-id="22d95-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22d95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22d95-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22d95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22d95-106">Чтение свойств и связей объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="22d95-106">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22d95-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="22d95-107">Prerequisites</span></span>
<span data-ttu-id="22d95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22d95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d95-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22d95-110">Permission type</span></span>|<span data-ttu-id="22d95-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22d95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22d95-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22d95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22d95-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="22d95-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="22d95-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22d95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22d95-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22d95-115">Not supported.</span></span>|
|<span data-ttu-id="22d95-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22d95-116">Application</span></span>|<span data-ttu-id="22d95-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="22d95-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22d95-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22d95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22d95-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22d95-119">Optional query parameters</span></span>
<span data-ttu-id="22d95-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="22d95-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22d95-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22d95-121">Request headers</span></span>
|<span data-ttu-id="22d95-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22d95-122">Header</span></span>|<span data-ttu-id="22d95-123">Значение</span><span class="sxs-lookup"><span data-stu-id="22d95-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22d95-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22d95-124">Authorization</span></span>|<span data-ttu-id="22d95-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22d95-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22d95-126">Accept</span><span class="sxs-lookup"><span data-stu-id="22d95-126">Accept</span></span>|<span data-ttu-id="22d95-127">application/json</span><span class="sxs-lookup"><span data-stu-id="22d95-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22d95-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="22d95-128">Request body</span></span>
<span data-ttu-id="22d95-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22d95-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22d95-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="22d95-130">Response</span></span>
<span data-ttu-id="22d95-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="22d95-131">If successful, this method returns a `200 OK` response code and [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22d95-132">Пример</span><span class="sxs-lookup"><span data-stu-id="22d95-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="22d95-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="22d95-133">Request</span></span>
<span data-ttu-id="22d95-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22d95-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="22d95-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d95-135">Response</span></span>
<span data-ttu-id="22d95-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22d95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContent",
    "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
  }
}
```




