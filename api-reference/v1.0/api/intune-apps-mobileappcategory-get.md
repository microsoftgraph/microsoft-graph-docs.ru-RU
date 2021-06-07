---
title: Get mobileAppCategory
description: Чтение свойств и связей объекта mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 12e7206707a070be2f5e7463d85a2a09d94c5ad0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754098"
---
# <a name="get-mobileappcategory"></a><span data-ttu-id="e8519-103">Get mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="e8519-103">Get mobileAppCategory</span></span>

<span data-ttu-id="e8519-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8519-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8519-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8519-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8519-106">Чтение свойств и связей объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="e8519-106">Read properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8519-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e8519-107">Prerequisites</span></span>
<span data-ttu-id="e8519-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8519-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8519-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8519-110">Permission type</span></span>|<span data-ttu-id="e8519-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8519-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8519-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8519-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8519-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8519-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e8519-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8519-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8519-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8519-115">Not supported.</span></span>|
|<span data-ttu-id="e8519-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e8519-116">Application</span></span>|<span data-ttu-id="e8519-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8519-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8519-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8519-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8519-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e8519-119">Optional query parameters</span></span>
<span data-ttu-id="e8519-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e8519-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8519-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8519-121">Request headers</span></span>
|<span data-ttu-id="e8519-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8519-122">Header</span></span>|<span data-ttu-id="e8519-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e8519-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8519-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8519-124">Authorization</span></span>|<span data-ttu-id="e8519-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8519-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8519-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e8519-126">Accept</span></span>|<span data-ttu-id="e8519-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e8519-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8519-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8519-128">Request body</span></span>
<span data-ttu-id="e8519-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8519-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8519-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8519-130">Response</span></span>
<span data-ttu-id="e8519-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e8519-131">If successful, this method returns a `200 OK` response code and [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8519-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e8519-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8519-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8519-133">Request</span></span>
<span data-ttu-id="e8519-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8519-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a><span data-ttu-id="e8519-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8519-135">Response</span></span>
<span data-ttu-id="e8519-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8519-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




