---
title: List deviceLogCollectionResponses
description: Список свойств и связей объектов deviceLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f8f6979d38dd0c80edd8f4ecb616f62178596972
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154373"
---
# <a name="list-devicelogcollectionresponses"></a><span data-ttu-id="87ddb-103">List deviceLogCollectionResponses</span><span class="sxs-lookup"><span data-stu-id="87ddb-103">List deviceLogCollectionResponses</span></span>

<span data-ttu-id="87ddb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87ddb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87ddb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87ddb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87ddb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87ddb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87ddb-107">Список свойств и связей [объектов deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="87ddb-107">List properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87ddb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87ddb-108">Prerequisites</span></span>
<span data-ttu-id="87ddb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87ddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87ddb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87ddb-111">Permission type</span></span>|<span data-ttu-id="87ddb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87ddb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87ddb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87ddb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87ddb-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ddb-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="87ddb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87ddb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87ddb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87ddb-116">Not supported.</span></span>|
|<span data-ttu-id="87ddb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="87ddb-117">Application</span></span>|<span data-ttu-id="87ddb-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ddb-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87ddb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87ddb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="87ddb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87ddb-120">Request headers</span></span>
|<span data-ttu-id="87ddb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87ddb-121">Header</span></span>|<span data-ttu-id="87ddb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87ddb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87ddb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87ddb-123">Authorization</span></span>|<span data-ttu-id="87ddb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87ddb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87ddb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87ddb-125">Accept</span></span>|<span data-ttu-id="87ddb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87ddb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87ddb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87ddb-127">Request body</span></span>
<span data-ttu-id="87ddb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87ddb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87ddb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="87ddb-129">Response</span></span>
<span data-ttu-id="87ddb-130">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="87ddb-130">If successful, this method returns a `200 OK` response code and a collection of [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87ddb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="87ddb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87ddb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="87ddb-132">Request</span></span>
<span data-ttu-id="87ddb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87ddb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

### <a name="response"></a><span data-ttu-id="87ddb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="87ddb-134">Response</span></span>
<span data-ttu-id="87ddb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87ddb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
      "id": "05fb97dc-97dc-05fb-dc97-fb05dc97fb05",
      "status": "Status value",
      "managedDeviceId": "3b336f00-6f00-3b33-006f-333b006f333b",
      "errorCode": 9,
      "requestedDateTimeUTC": "2016-12-31T23:57:40.7845755-08:00",
      "receivedDateTimeUTC": "2016-12-31T23:59:48.6545758-08:00",
      "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
      "expirationDateTimeUTC": "2017-01-01T00:02:49.2157996-08:00",
      "size": 1.3333333333333333
    }
  ]
}
```




