---
title: Get mobileAppCategory
description: Чтение свойств и связей объекта mobileAppCategory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27522477a0a19d5fba412ae350360d3171f77aed
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355094"
---
# <a name="get-mobileappcategory"></a><span data-ttu-id="f84bd-103">Get mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="f84bd-103">Get mobileAppCategory</span></span>

> <span data-ttu-id="f84bd-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f84bd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f84bd-105">Чтение свойств и связей объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="f84bd-105">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f84bd-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f84bd-106">Prerequisites</span></span>
<span data-ttu-id="f84bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f84bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f84bd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f84bd-109">Permission type</span></span>|<span data-ttu-id="f84bd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f84bd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f84bd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f84bd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f84bd-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f84bd-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f84bd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f84bd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f84bd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f84bd-114">Not supported.</span></span>|
|<span data-ttu-id="f84bd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f84bd-115">Application</span></span>|<span data-ttu-id="f84bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f84bd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f84bd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f84bd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f84bd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f84bd-118">Optional query parameters</span></span>
<span data-ttu-id="f84bd-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f84bd-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f84bd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f84bd-120">Request headers</span></span>
|<span data-ttu-id="f84bd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f84bd-121">Header</span></span>|<span data-ttu-id="f84bd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f84bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f84bd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f84bd-123">Authorization</span></span>|<span data-ttu-id="f84bd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f84bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f84bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f84bd-125">Accept</span></span>|<span data-ttu-id="f84bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f84bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f84bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f84bd-127">Request body</span></span>
<span data-ttu-id="f84bd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f84bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f84bd-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f84bd-129">Response</span></span>
<span data-ttu-id="f84bd-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f84bd-130">If successful, this method returns a `200 OK` response code and [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f84bd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f84bd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f84bd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f84bd-132">Request</span></span>
<span data-ttu-id="f84bd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f84bd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="f84bd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f84bd-134">Response</span></span>
<span data-ttu-id="f84bd-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f84bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppCategory",
    "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




