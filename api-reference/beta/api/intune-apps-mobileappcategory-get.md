---
title: Get mobileAppCategory
description: Чтение свойств и связей объекта mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 602f97d337d70c5ddef1d649c92956b4f8d489e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977497"
---
# <a name="get-mobileappcategory"></a><span data-ttu-id="79486-103">Get mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="79486-103">Get mobileAppCategory</span></span>

<span data-ttu-id="79486-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79486-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79486-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79486-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79486-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79486-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79486-107">Чтение свойств и связей объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="79486-107">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79486-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="79486-108">Prerequisites</span></span>
<span data-ttu-id="79486-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79486-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79486-111">Permission type</span></span>|<span data-ttu-id="79486-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79486-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79486-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79486-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79486-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="79486-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="79486-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79486-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79486-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79486-116">Not supported.</span></span>|
|<span data-ttu-id="79486-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79486-117">Application</span></span>|<span data-ttu-id="79486-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="79486-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79486-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79486-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79486-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="79486-120">Optional query parameters</span></span>
<span data-ttu-id="79486-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="79486-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79486-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79486-122">Request headers</span></span>
|<span data-ttu-id="79486-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79486-123">Header</span></span>|<span data-ttu-id="79486-124">Значение</span><span class="sxs-lookup"><span data-stu-id="79486-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79486-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="79486-125">Authorization</span></span>|<span data-ttu-id="79486-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79486-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79486-127">Accept</span><span class="sxs-lookup"><span data-stu-id="79486-127">Accept</span></span>|<span data-ttu-id="79486-128">application/json</span><span class="sxs-lookup"><span data-stu-id="79486-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79486-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79486-129">Request body</span></span>
<span data-ttu-id="79486-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79486-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79486-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="79486-131">Response</span></span>
<span data-ttu-id="79486-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="79486-132">If successful, this method returns a `200 OK` response code and [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79486-133">Пример</span><span class="sxs-lookup"><span data-stu-id="79486-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="79486-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="79486-134">Request</span></span>
<span data-ttu-id="79486-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79486-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="79486-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="79486-136">Response</span></span>
<span data-ttu-id="79486-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79486-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






