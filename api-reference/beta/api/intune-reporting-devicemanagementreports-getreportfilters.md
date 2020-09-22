---
title: действие Жетрепортфилтерс
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0694f6b852d64e8d2b0bda9876ef3dbce5e199d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040478"
---
# <a name="getreportfilters-action"></a><span data-ttu-id="f7f5e-103">действие Жетрепортфилтерс</span><span class="sxs-lookup"><span data-stu-id="f7f5e-103">getReportFilters action</span></span>

<span data-ttu-id="f7f5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7f5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7f5e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7f5e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7f5e-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7f5e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7f5e-108">Prerequisites</span></span>
<span data-ttu-id="f7f5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7f5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7f5e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7f5e-111">Permission type</span></span>|<span data-ttu-id="f7f5e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7f5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7f5e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7f5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7f5e-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f7f5e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f7f5e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7f5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7f5e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-116">Not supported.</span></span>|
|<span data-ttu-id="f7f5e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7f5e-117">Application</span></span>|<span data-ttu-id="f7f5e-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f7f5e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7f5e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7f5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getReportFilters
```

## <a name="request-headers"></a><span data-ttu-id="f7f5e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f7f5e-120">Request headers</span></span>
|<span data-ttu-id="f7f5e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7f5e-121">Header</span></span>|<span data-ttu-id="f7f5e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7f5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7f5e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7f5e-123">Authorization</span></span>|<span data-ttu-id="f7f5e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7f5e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7f5e-125">Accept</span></span>|<span data-ttu-id="f7f5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7f5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7f5e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7f5e-127">Request body</span></span>
<span data-ttu-id="f7f5e-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f7f5e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f7f5e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7f5e-130">Property</span></span>|<span data-ttu-id="f7f5e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7f5e-131">Type</span></span>|<span data-ttu-id="f7f5e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7f5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7f5e-133">name</span><span class="sxs-lookup"><span data-stu-id="f7f5e-133">name</span></span>|<span data-ttu-id="f7f5e-134">String</span><span class="sxs-lookup"><span data-stu-id="f7f5e-134">String</span></span>|<span data-ttu-id="f7f5e-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-135">Not yet documented</span></span>|
|<span data-ttu-id="f7f5e-136">select</span><span class="sxs-lookup"><span data-stu-id="f7f5e-136">select</span></span>|<span data-ttu-id="f7f5e-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f7f5e-137">String collection</span></span>|<span data-ttu-id="f7f5e-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f7f5e-138">Not yet documented</span></span>|
|<span data-ttu-id="f7f5e-139">search</span><span class="sxs-lookup"><span data-stu-id="f7f5e-139">search</span></span>|<span data-ttu-id="f7f5e-140">String</span><span class="sxs-lookup"><span data-stu-id="f7f5e-140">String</span></span>|<span data-ttu-id="f7f5e-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-141">Not yet documented</span></span>|
|<span data-ttu-id="f7f5e-142">Оператора</span><span class="sxs-lookup"><span data-stu-id="f7f5e-142">groupBy</span></span>|<span data-ttu-id="f7f5e-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f7f5e-143">String collection</span></span>|<span data-ttu-id="f7f5e-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f7f5e-144">Not yet documented</span></span>|
|<span data-ttu-id="f7f5e-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="f7f5e-145">orderBy</span></span>|<span data-ttu-id="f7f5e-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f7f5e-146">String collection</span></span>|<span data-ttu-id="f7f5e-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f7f5e-147">Not yet documented</span></span>|
|<span data-ttu-id="f7f5e-148">skip</span><span class="sxs-lookup"><span data-stu-id="f7f5e-148">skip</span></span>|<span data-ttu-id="f7f5e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f7f5e-149">Int32</span></span>|<span data-ttu-id="f7f5e-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-150">Not yet documented</span></span>|
|<span data-ttu-id="f7f5e-151">top</span><span class="sxs-lookup"><span data-stu-id="f7f5e-151">top</span></span>|<span data-ttu-id="f7f5e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f7f5e-152">Int32</span></span>|<span data-ttu-id="f7f5e-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-153">Not yet documented</span></span>|
|<span data-ttu-id="f7f5e-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="f7f5e-154">sessionId</span></span>|<span data-ttu-id="f7f5e-155">String</span><span class="sxs-lookup"><span data-stu-id="f7f5e-155">String</span></span>|<span data-ttu-id="f7f5e-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-156">Not yet documented</span></span>|
|<span data-ttu-id="f7f5e-157">filter</span><span class="sxs-lookup"><span data-stu-id="f7f5e-157">filter</span></span>|<span data-ttu-id="f7f5e-158">String</span><span class="sxs-lookup"><span data-stu-id="f7f5e-158">String</span></span>|<span data-ttu-id="f7f5e-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f7f5e-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7f5e-160">Response</span></span>
<span data-ttu-id="f7f5e-161">При успешном выполнении это действие возвращает `200 OK` код отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7f5e-162">Пример</span><span class="sxs-lookup"><span data-stu-id="f7f5e-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7f5e-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7f5e-163">Request</span></span>
<span data-ttu-id="f7f5e-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f7f5e-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7f5e-165">Response</span></span>
<span data-ttu-id="f7f5e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7f5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": "Z2V0UmVwb3J0RmlsdGVycyBJbnR1bmUgRG9jIFNhbXBsZSAxMzYxOTI0Mjkx"
}
```






