---
title: Список Девицелогколлектионреспонсес
description: Список свойств и связей объектов Девицелогколлектионреспонсе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b8abd07487cbd491b6310022757a14d01e160db7
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124308"
---
# <a name="list-devicelogcollectionresponses"></a><span data-ttu-id="eebdc-103">Список Девицелогколлектионреспонсес</span><span class="sxs-lookup"><span data-stu-id="eebdc-103">List deviceLogCollectionResponses</span></span>

<span data-ttu-id="eebdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eebdc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eebdc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eebdc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eebdc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eebdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eebdc-107">Список свойств и связей объектов [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="eebdc-107">List properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eebdc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eebdc-108">Prerequisites</span></span>
<span data-ttu-id="eebdc-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="eebdc-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="eebdc-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eebdc-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eebdc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eebdc-111">Permission type</span></span>|<span data-ttu-id="eebdc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eebdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eebdc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eebdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eebdc-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="eebdc-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="eebdc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eebdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eebdc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eebdc-116">Not supported.</span></span>|
|<span data-ttu-id="eebdc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eebdc-117">Application</span></span>|<span data-ttu-id="eebdc-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="eebdc-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eebdc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eebdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="eebdc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eebdc-120">Request headers</span></span>
|<span data-ttu-id="eebdc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eebdc-121">Header</span></span>|<span data-ttu-id="eebdc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eebdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eebdc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eebdc-123">Authorization</span></span>|<span data-ttu-id="eebdc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eebdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eebdc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eebdc-125">Accept</span></span>|<span data-ttu-id="eebdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eebdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eebdc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eebdc-127">Request body</span></span>
<span data-ttu-id="eebdc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eebdc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eebdc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="eebdc-129">Response</span></span>
<span data-ttu-id="eebdc-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eebdc-130">If successful, this method returns a `200 OK` response code and a collection of [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eebdc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="eebdc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eebdc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="eebdc-132">Request</span></span>
<span data-ttu-id="eebdc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eebdc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

### <a name="response"></a><span data-ttu-id="eebdc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="eebdc-134">Response</span></span>
<span data-ttu-id="eebdc-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="eebdc-135">Here is an example of the response.</span></span> <span data-ttu-id="eebdc-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="eebdc-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="eebdc-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="eebdc-137">All of the properties will be returned from an actual call.</span></span>
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



