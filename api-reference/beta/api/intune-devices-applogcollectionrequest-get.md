---
title: Get appLogCollectionRequest
description: Чтение свойств и связей объекта appLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88a6f732fb30b1840f6ccc5b0c18816e4aaa9b42
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150663"
---
# <a name="get-applogcollectionrequest"></a><span data-ttu-id="91f11-103">Get appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="91f11-103">Get appLogCollectionRequest</span></span>

<span data-ttu-id="91f11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91f11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91f11-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91f11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91f11-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91f11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91f11-107">Чтение свойств и связей объекта [appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="91f11-107">Read properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91f11-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="91f11-108">Prerequisites</span></span>
<span data-ttu-id="91f11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91f11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91f11-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91f11-111">Permission type</span></span>|<span data-ttu-id="91f11-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91f11-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91f11-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91f11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91f11-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f11-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="91f11-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91f11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91f11-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91f11-116">Not supported.</span></span>|
|<span data-ttu-id="91f11-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="91f11-117">Application</span></span>|<span data-ttu-id="91f11-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f11-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91f11-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91f11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91f11-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91f11-120">Optional query parameters</span></span>
<span data-ttu-id="91f11-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="91f11-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91f11-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91f11-122">Request headers</span></span>
|<span data-ttu-id="91f11-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91f11-123">Header</span></span>|<span data-ttu-id="91f11-124">Значение</span><span class="sxs-lookup"><span data-stu-id="91f11-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91f11-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="91f11-125">Authorization</span></span>|<span data-ttu-id="91f11-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91f11-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91f11-127">Accept</span><span class="sxs-lookup"><span data-stu-id="91f11-127">Accept</span></span>|<span data-ttu-id="91f11-128">application/json</span><span class="sxs-lookup"><span data-stu-id="91f11-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91f11-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91f11-129">Request body</span></span>
<span data-ttu-id="91f11-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91f11-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91f11-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="91f11-131">Response</span></span>
<span data-ttu-id="91f11-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="91f11-132">If successful, this method returns a `200 OK` response code and [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91f11-133">Пример</span><span class="sxs-lookup"><span data-stu-id="91f11-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="91f11-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="91f11-134">Request</span></span>
<span data-ttu-id="91f11-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91f11-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

### <a name="response"></a><span data-ttu-id="91f11-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="91f11-136">Response</span></span>
<span data-ttu-id="91f11-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91f11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": {
    "@odata.type": "#microsoft.graph.appLogCollectionRequest",
    "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
    "status": "completed",
    "errorMessage": "Error Message value",
    "customLogFolders": [
      "Custom Log Folders value"
    ],
    "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
  }
}
```




