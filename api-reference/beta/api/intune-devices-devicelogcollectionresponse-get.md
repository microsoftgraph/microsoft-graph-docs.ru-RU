---
title: Get deviceLogCollectionResponse
description: Чтение свойств и связей объекта deviceLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e96b5bc980052fb890ecf87636d3341d82ef7f01
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154380"
---
# <a name="get-devicelogcollectionresponse"></a><span data-ttu-id="d1736-103">Get deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="d1736-103">Get deviceLogCollectionResponse</span></span>

<span data-ttu-id="d1736-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1736-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1736-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1736-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1736-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1736-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1736-107">Чтение свойств и связей [объекта deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="d1736-107">Read properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1736-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d1736-108">Prerequisites</span></span>
<span data-ttu-id="d1736-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1736-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1736-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1736-111">Permission type</span></span>|<span data-ttu-id="d1736-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1736-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1736-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1736-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1736-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1736-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d1736-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1736-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1736-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1736-116">Not supported.</span></span>|
|<span data-ttu-id="d1736-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d1736-117">Application</span></span>|<span data-ttu-id="d1736-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1736-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1736-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1736-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1736-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1736-120">Optional query parameters</span></span>
<span data-ttu-id="d1736-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d1736-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1736-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1736-122">Request headers</span></span>
|<span data-ttu-id="d1736-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1736-123">Header</span></span>|<span data-ttu-id="d1736-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d1736-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1736-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1736-125">Authorization</span></span>|<span data-ttu-id="d1736-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1736-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1736-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d1736-127">Accept</span></span>|<span data-ttu-id="d1736-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d1736-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1736-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1736-129">Request body</span></span>
<span data-ttu-id="d1736-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1736-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1736-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1736-131">Response</span></span>
<span data-ttu-id="d1736-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d1736-132">If successful, this method returns a `200 OK` response code and [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1736-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d1736-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1736-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1736-134">Request</span></span>
<span data-ttu-id="d1736-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1736-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

### <a name="response"></a><span data-ttu-id="d1736-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1736-136">Response</span></span>
<span data-ttu-id="d1736-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1736-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "value": {
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
}
```




