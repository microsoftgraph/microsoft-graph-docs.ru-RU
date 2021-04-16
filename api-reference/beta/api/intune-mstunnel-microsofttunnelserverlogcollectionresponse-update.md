---
title: Обновление microsoftTunnelServerLogCollectionResponse
description: Обновление свойств объекта microsoftTunnelServerLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 37ab8e10ea1b33c6f600fd88d7670cc7c6a63ece
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865189"
---
# <a name="update-microsofttunnelserverlogcollectionresponse"></a><span data-ttu-id="e32e3-103">Обновление microsoftTunnelServerLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="e32e3-103">Update microsoftTunnelServerLogCollectionResponse</span></span>

<span data-ttu-id="e32e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e32e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e32e3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e32e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e32e3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e32e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e32e3-107">Обновление свойств объекта [microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="e32e3-107">Update the properties of a [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e32e3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e32e3-108">Prerequisites</span></span>
<span data-ttu-id="e32e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e32e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e32e3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e32e3-111">Permission type</span></span>|<span data-ttu-id="e32e3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e32e3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e32e3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e32e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e32e3-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e32e3-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="e32e3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e32e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e32e3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e32e3-116">Not supported.</span></span>|
|<span data-ttu-id="e32e3-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e32e3-117">Application</span></span>|<span data-ttu-id="e32e3-118">MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e32e3-118">MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e32e3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e32e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelServerLogCollectionResponses/{microsoftTunnelServerLogCollectionResponseId}
```

## <a name="request-headers"></a><span data-ttu-id="e32e3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e32e3-120">Request headers</span></span>
|<span data-ttu-id="e32e3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e32e3-121">Header</span></span>|<span data-ttu-id="e32e3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e32e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e32e3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e32e3-123">Authorization</span></span>|<span data-ttu-id="e32e3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e32e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e32e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e32e3-125">Accept</span></span>|<span data-ttu-id="e32e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e32e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e32e3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e32e3-127">Request body</span></span>
<span data-ttu-id="e32e3-128">В теле запроса поставляем представление JSON для [объекта microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="e32e3-128">In the request body, supply a JSON representation for the [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object.</span></span>

<span data-ttu-id="e32e3-129">В следующей таблице показаны свойства, необходимые при создании [microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="e32e3-129">The following table shows the properties that are required when you create the [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md).</span></span>

|<span data-ttu-id="e32e3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e32e3-130">Property</span></span>|<span data-ttu-id="e32e3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e32e3-131">Type</span></span>|<span data-ttu-id="e32e3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e32e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e32e3-133">id</span><span class="sxs-lookup"><span data-stu-id="e32e3-133">id</span></span>|<span data-ttu-id="e32e3-134">String</span><span class="sxs-lookup"><span data-stu-id="e32e3-134">String</span></span>|<span data-ttu-id="e32e3-135">Уникальный ID объекта</span><span class="sxs-lookup"><span data-stu-id="e32e3-135">The unique ID of the entity</span></span>|
|<span data-ttu-id="e32e3-136">status</span><span class="sxs-lookup"><span data-stu-id="e32e3-136">status</span></span>|[<span data-ttu-id="e32e3-137">microsoftTunnelLogCollectionStatus</span><span class="sxs-lookup"><span data-stu-id="e32e3-137">microsoftTunnelLogCollectionStatus</span></span>](../resources/intune-mstunnel-microsofttunnellogcollectionstatus.md)|<span data-ttu-id="e32e3-138">Состояние коллекции журналов.</span><span class="sxs-lookup"><span data-stu-id="e32e3-138">The status of log collection.</span></span> <span data-ttu-id="e32e3-139">Возможные значения: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e32e3-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="e32e3-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e32e3-140">startDateTime</span></span>|<span data-ttu-id="e32e3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e32e3-141">DateTimeOffset</span></span>|<span data-ttu-id="e32e3-142">Время начала собранных журналов</span><span class="sxs-lookup"><span data-stu-id="e32e3-142">The start time of the logs collected</span></span> |
|<span data-ttu-id="e32e3-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e32e3-143">endDateTime</span></span>|<span data-ttu-id="e32e3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e32e3-144">DateTimeOffset</span></span>|<span data-ttu-id="e32e3-145">Время окончания собранных журналов</span><span class="sxs-lookup"><span data-stu-id="e32e3-145">The end time of the logs collected</span></span>|
|<span data-ttu-id="e32e3-146">sizeInBytes</span><span class="sxs-lookup"><span data-stu-id="e32e3-146">sizeInBytes</span></span>|<span data-ttu-id="e32e3-147">Int64</span><span class="sxs-lookup"><span data-stu-id="e32e3-147">Int64</span></span>|<span data-ttu-id="e32e3-148">Размер журналов в bytes</span><span class="sxs-lookup"><span data-stu-id="e32e3-148">The size of the logs in bytes</span></span>|



## <a name="response"></a><span data-ttu-id="e32e3-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="e32e3-149">Response</span></span>
<span data-ttu-id="e32e3-150">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e32e3-150">If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e32e3-151">Пример</span><span class="sxs-lookup"><span data-stu-id="e32e3-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e32e3-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e32e3-152">Request</span></span>
<span data-ttu-id="e32e3-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e32e3-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelServerLogCollectionResponses/{microsoftTunnelServerLogCollectionResponseId}
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

### <a name="response"></a><span data-ttu-id="e32e3-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="e32e3-154">Response</span></span>
<span data-ttu-id="e32e3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e32e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




