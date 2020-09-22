---
title: Список Девицелогколлектионреспонсес
description: Список свойств и связей объектов Девицелогколлектионреспонсе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f2235e23e083b0625158b09873366610f928348
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014590"
---
# <a name="list-devicelogcollectionresponses"></a><span data-ttu-id="294e2-103">Список Девицелогколлектионреспонсес</span><span class="sxs-lookup"><span data-stu-id="294e2-103">List deviceLogCollectionResponses</span></span>

<span data-ttu-id="294e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="294e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="294e2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="294e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="294e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="294e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="294e2-107">Список свойств и связей объектов [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="294e2-107">List properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="294e2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="294e2-108">Prerequisites</span></span>
<span data-ttu-id="294e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="294e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="294e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="294e2-111">Permission type</span></span>|<span data-ttu-id="294e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="294e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="294e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="294e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="294e2-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e2-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="294e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="294e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="294e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="294e2-116">Not supported.</span></span>|
|<span data-ttu-id="294e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="294e2-117">Application</span></span>|<span data-ttu-id="294e2-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="294e2-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="294e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="294e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="294e2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="294e2-120">Request headers</span></span>
|<span data-ttu-id="294e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="294e2-121">Header</span></span>|<span data-ttu-id="294e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="294e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="294e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="294e2-123">Authorization</span></span>|<span data-ttu-id="294e2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="294e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="294e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="294e2-125">Accept</span></span>|<span data-ttu-id="294e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="294e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="294e2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="294e2-127">Request body</span></span>
<span data-ttu-id="294e2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="294e2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="294e2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="294e2-129">Response</span></span>
<span data-ttu-id="294e2-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="294e2-130">If successful, this method returns a `200 OK` response code and a collection of [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="294e2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="294e2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="294e2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="294e2-132">Request</span></span>
<span data-ttu-id="294e2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="294e2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

### <a name="response"></a><span data-ttu-id="294e2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="294e2-134">Response</span></span>
<span data-ttu-id="294e2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="294e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






