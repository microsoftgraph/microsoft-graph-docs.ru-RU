---
title: Создание microsoftTunnelServerLogCollectionResponse
description: Создайте новый объект microsoftTunnelServerLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f9e8c139be2aec7edcf698322218fae44b5a5c2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153071"
---
# <a name="create-microsofttunnelserverlogcollectionresponse"></a><span data-ttu-id="a7d4d-103">Создание microsoftTunnelServerLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="a7d4d-103">Create microsoftTunnelServerLogCollectionResponse</span></span>

<span data-ttu-id="a7d4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7d4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7d4d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7d4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7d4d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7d4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7d4d-107">Создайте [новый объект microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="a7d4d-107">Create a new [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7d4d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a7d4d-108">Prerequisites</span></span>
<span data-ttu-id="a7d4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7d4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7d4d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7d4d-111">Permission type</span></span>|<span data-ttu-id="a7d4d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7d4d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7d4d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7d4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7d4d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7d4d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7d4d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7d4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7d4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7d4d-116">Not supported.</span></span>|
|<span data-ttu-id="a7d4d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a7d4d-117">Application</span></span>|<span data-ttu-id="a7d4d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7d4d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7d4d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7d4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelServerLogCollectionResponses
```

## <a name="request-headers"></a><span data-ttu-id="a7d4d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a7d4d-120">Request headers</span></span>
|<span data-ttu-id="a7d4d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7d4d-121">Header</span></span>|<span data-ttu-id="a7d4d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a7d4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7d4d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7d4d-123">Authorization</span></span>|<span data-ttu-id="a7d4d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7d4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7d4d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7d4d-125">Accept</span></span>|<span data-ttu-id="a7d4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7d4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7d4d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7d4d-127">Request body</span></span>
<span data-ttu-id="a7d4d-128">В теле запроса поставляем представление JSON для объекта microsoftTunnelServerLogCollectionResponse.</span><span class="sxs-lookup"><span data-stu-id="a7d4d-128">In the request body, supply a JSON representation for the microsoftTunnelServerLogCollectionResponse object.</span></span>

<span data-ttu-id="a7d4d-129">В следующей таблице показаны свойства, необходимые при создании microsoftTunnelServerLogCollectionResponse.</span><span class="sxs-lookup"><span data-stu-id="a7d4d-129">The following table shows the properties that are required when you create the microsoftTunnelServerLogCollectionResponse.</span></span>

|<span data-ttu-id="a7d4d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7d4d-130">Property</span></span>|<span data-ttu-id="a7d4d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a7d4d-131">Type</span></span>|<span data-ttu-id="a7d4d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a7d4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7d4d-133">id</span><span class="sxs-lookup"><span data-stu-id="a7d4d-133">id</span></span>|<span data-ttu-id="a7d4d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a7d4d-134">String</span></span>|<span data-ttu-id="a7d4d-135">Уникальный ID объекта</span><span class="sxs-lookup"><span data-stu-id="a7d4d-135">The unique ID of the entity</span></span>|
|<span data-ttu-id="a7d4d-136">status</span><span class="sxs-lookup"><span data-stu-id="a7d4d-136">status</span></span>|[<span data-ttu-id="a7d4d-137">microsoftTunnelLogCollectionStatus</span><span class="sxs-lookup"><span data-stu-id="a7d4d-137">microsoftTunnelLogCollectionStatus</span></span>](../resources/intune-mstunnel-microsofttunnellogcollectionstatus.md)|<span data-ttu-id="a7d4d-138">Состояние коллекции журналов.</span><span class="sxs-lookup"><span data-stu-id="a7d4d-138">The status of log collection.</span></span> <span data-ttu-id="a7d4d-139">Возможные значения: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a7d4d-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="a7d4d-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a7d4d-140">startDateTime</span></span>|<span data-ttu-id="a7d4d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7d4d-141">DateTimeOffset</span></span>|<span data-ttu-id="a7d4d-142">Время начала собранных журналов</span><span class="sxs-lookup"><span data-stu-id="a7d4d-142">The start time of the logs collected</span></span> |
|<span data-ttu-id="a7d4d-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a7d4d-143">endDateTime</span></span>|<span data-ttu-id="a7d4d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7d4d-144">DateTimeOffset</span></span>|<span data-ttu-id="a7d4d-145">Время окончания собранных журналов</span><span class="sxs-lookup"><span data-stu-id="a7d4d-145">The end time of the logs collected</span></span>|
|<span data-ttu-id="a7d4d-146">sizeInBytes</span><span class="sxs-lookup"><span data-stu-id="a7d4d-146">sizeInBytes</span></span>|<span data-ttu-id="a7d4d-147">Int64</span><span class="sxs-lookup"><span data-stu-id="a7d4d-147">Int64</span></span>|<span data-ttu-id="a7d4d-148">Размер журналов в bytes</span><span class="sxs-lookup"><span data-stu-id="a7d4d-148">The size of the logs in bytes</span></span>|



## <a name="response"></a><span data-ttu-id="a7d4d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7d4d-149">Response</span></span>
<span data-ttu-id="a7d4d-150">В случае успеха этот метод возвращает код отклика и `201 Created` [объект microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a7d4d-150">If successful, this method returns a `201 Created` response code and a [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7d4d-151">Пример</span><span class="sxs-lookup"><span data-stu-id="a7d4d-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7d4d-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7d4d-152">Request</span></span>
<span data-ttu-id="a7d4d-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7d4d-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelServerLogCollectionResponses
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "status": "completed",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "sizeInBytes": 11
}
```

### <a name="response"></a><span data-ttu-id="a7d4d-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7d4d-154">Response</span></span>
<span data-ttu-id="a7d4d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7d4d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "id": "05dcc2e9-c2e9-05dc-e9c2-dc05e9c2dc05",
  "status": "completed",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "sizeInBytes": 11
}
```




