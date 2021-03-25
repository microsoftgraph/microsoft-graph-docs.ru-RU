---
title: действие getReportFilters
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 995eac190e8cc843e437361d8b445b05019ffe96
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156431"
---
# <a name="getreportfilters-action"></a><span data-ttu-id="af879-103">действие getReportFilters</span><span class="sxs-lookup"><span data-stu-id="af879-103">getReportFilters action</span></span>

<span data-ttu-id="af879-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af879-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af879-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af879-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af879-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af879-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af879-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="af879-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af879-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="af879-108">Prerequisites</span></span>
<span data-ttu-id="af879-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af879-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af879-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af879-111">Permission type</span></span>|<span data-ttu-id="af879-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af879-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af879-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af879-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af879-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af879-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="af879-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af879-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af879-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af879-116">Not supported.</span></span>|
|<span data-ttu-id="af879-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="af879-117">Application</span></span>|<span data-ttu-id="af879-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af879-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af879-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af879-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getReportFilters
```

## <a name="request-headers"></a><span data-ttu-id="af879-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="af879-120">Request headers</span></span>
|<span data-ttu-id="af879-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af879-121">Header</span></span>|<span data-ttu-id="af879-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af879-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af879-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af879-123">Authorization</span></span>|<span data-ttu-id="af879-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af879-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af879-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af879-125">Accept</span></span>|<span data-ttu-id="af879-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af879-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af879-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af879-127">Request body</span></span>
<span data-ttu-id="af879-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af879-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="af879-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="af879-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="af879-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="af879-130">Property</span></span>|<span data-ttu-id="af879-131">Тип</span><span class="sxs-lookup"><span data-stu-id="af879-131">Type</span></span>|<span data-ttu-id="af879-132">Описание</span><span class="sxs-lookup"><span data-stu-id="af879-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af879-133">name</span><span class="sxs-lookup"><span data-stu-id="af879-133">name</span></span>|<span data-ttu-id="af879-134">String</span><span class="sxs-lookup"><span data-stu-id="af879-134">String</span></span>|<span data-ttu-id="af879-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="af879-135">Not yet documented</span></span>|
|<span data-ttu-id="af879-136">select</span><span class="sxs-lookup"><span data-stu-id="af879-136">select</span></span>|<span data-ttu-id="af879-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="af879-137">String collection</span></span>|<span data-ttu-id="af879-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af879-138">Not yet documented</span></span>|
|<span data-ttu-id="af879-139">search</span><span class="sxs-lookup"><span data-stu-id="af879-139">search</span></span>|<span data-ttu-id="af879-140">String</span><span class="sxs-lookup"><span data-stu-id="af879-140">String</span></span>|<span data-ttu-id="af879-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="af879-141">Not yet documented</span></span>|
|<span data-ttu-id="af879-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="af879-142">groupBy</span></span>|<span data-ttu-id="af879-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="af879-143">String collection</span></span>|<span data-ttu-id="af879-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af879-144">Not yet documented</span></span>|
|<span data-ttu-id="af879-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="af879-145">orderBy</span></span>|<span data-ttu-id="af879-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="af879-146">String collection</span></span>|<span data-ttu-id="af879-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af879-147">Not yet documented</span></span>|
|<span data-ttu-id="af879-148">skip</span><span class="sxs-lookup"><span data-stu-id="af879-148">skip</span></span>|<span data-ttu-id="af879-149">Int32</span><span class="sxs-lookup"><span data-stu-id="af879-149">Int32</span></span>|<span data-ttu-id="af879-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="af879-150">Not yet documented</span></span>|
|<span data-ttu-id="af879-151">top</span><span class="sxs-lookup"><span data-stu-id="af879-151">top</span></span>|<span data-ttu-id="af879-152">Int32</span><span class="sxs-lookup"><span data-stu-id="af879-152">Int32</span></span>|<span data-ttu-id="af879-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="af879-153">Not yet documented</span></span>|
|<span data-ttu-id="af879-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="af879-154">sessionId</span></span>|<span data-ttu-id="af879-155">String</span><span class="sxs-lookup"><span data-stu-id="af879-155">String</span></span>|<span data-ttu-id="af879-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="af879-156">Not yet documented</span></span>|
|<span data-ttu-id="af879-157">filter</span><span class="sxs-lookup"><span data-stu-id="af879-157">filter</span></span>|<span data-ttu-id="af879-158">String</span><span class="sxs-lookup"><span data-stu-id="af879-158">String</span></span>|<span data-ttu-id="af879-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="af879-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="af879-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="af879-160">Response</span></span>
<span data-ttu-id="af879-161">В случае успешного действия это действие возвращает код `200 OK` отклика и поток в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="af879-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af879-162">Пример</span><span class="sxs-lookup"><span data-stu-id="af879-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="af879-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="af879-163">Request</span></span>
<span data-ttu-id="af879-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af879-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getReportFilters

Content-type: application/json
Content-length: 278

{
  "name": "Name value",
  "select": [
    "Select value"
  ],
  "search": "Search value",
  "groupBy": [
    "Group By value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "skip": 4,
  "top": 3,
  "sessionId": "Session Id value",
  "filter": "Filter value"
}
```

### <a name="response"></a><span data-ttu-id="af879-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="af879-165">Response</span></span>
<span data-ttu-id="af879-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af879-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": "Z2V0UmVwb3J0RmlsdGVycyBJbnR1bmUgRG9jIFNhbXBsZSAxMzYxOTI0Mjkx"
}
```




