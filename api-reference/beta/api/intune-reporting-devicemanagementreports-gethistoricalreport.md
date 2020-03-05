---
title: действие Жесисторикалрепорт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20ef59592c55b23b04cce2211ca752e896c36e86
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459171"
---
# <a name="gethistoricalreport-action"></a><span data-ttu-id="4ef36-103">действие Жесисторикалрепорт</span><span class="sxs-lookup"><span data-stu-id="4ef36-103">getHistoricalReport action</span></span>

<span data-ttu-id="4ef36-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4ef36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ef36-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ef36-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ef36-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ef36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ef36-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4ef36-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ef36-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4ef36-108">Prerequisites</span></span>
<span data-ttu-id="4ef36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ef36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ef36-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ef36-111">Permission type</span></span>|<span data-ttu-id="4ef36-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ef36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ef36-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ef36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ef36-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4ef36-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4ef36-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ef36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ef36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ef36-116">Not supported.</span></span>|
|<span data-ttu-id="4ef36-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ef36-117">Application</span></span>|<span data-ttu-id="4ef36-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4ef36-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ef36-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ef36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getHistoricalReport
```

## <a name="request-headers"></a><span data-ttu-id="4ef36-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4ef36-120">Request headers</span></span>
|<span data-ttu-id="4ef36-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ef36-121">Header</span></span>|<span data-ttu-id="4ef36-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4ef36-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ef36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ef36-123">Authorization</span></span>|<span data-ttu-id="4ef36-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ef36-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ef36-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ef36-125">Accept</span></span>|<span data-ttu-id="4ef36-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ef36-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ef36-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ef36-127">Request body</span></span>
<span data-ttu-id="4ef36-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ef36-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4ef36-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4ef36-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4ef36-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ef36-130">Property</span></span>|<span data-ttu-id="4ef36-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4ef36-131">Type</span></span>|<span data-ttu-id="4ef36-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4ef36-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ef36-133">name</span><span class="sxs-lookup"><span data-stu-id="4ef36-133">name</span></span>|<span data-ttu-id="4ef36-134">String</span><span class="sxs-lookup"><span data-stu-id="4ef36-134">String</span></span>|<span data-ttu-id="4ef36-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4ef36-135">Not yet documented</span></span>|
|<span data-ttu-id="4ef36-136">select</span><span class="sxs-lookup"><span data-stu-id="4ef36-136">select</span></span>|<span data-ttu-id="4ef36-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4ef36-137">String collection</span></span>|<span data-ttu-id="4ef36-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4ef36-138">Not yet documented</span></span>|
|<span data-ttu-id="4ef36-139">search</span><span class="sxs-lookup"><span data-stu-id="4ef36-139">search</span></span>|<span data-ttu-id="4ef36-140">String</span><span class="sxs-lookup"><span data-stu-id="4ef36-140">String</span></span>|<span data-ttu-id="4ef36-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4ef36-141">Not yet documented</span></span>|
|<span data-ttu-id="4ef36-142">Оператора</span><span class="sxs-lookup"><span data-stu-id="4ef36-142">groupBy</span></span>|<span data-ttu-id="4ef36-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4ef36-143">String collection</span></span>|<span data-ttu-id="4ef36-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4ef36-144">Not yet documented</span></span>|
|<span data-ttu-id="4ef36-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="4ef36-145">orderBy</span></span>|<span data-ttu-id="4ef36-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4ef36-146">String collection</span></span>|<span data-ttu-id="4ef36-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4ef36-147">Not yet documented</span></span>|
|<span data-ttu-id="4ef36-148">skip</span><span class="sxs-lookup"><span data-stu-id="4ef36-148">skip</span></span>|<span data-ttu-id="4ef36-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4ef36-149">Int32</span></span>|<span data-ttu-id="4ef36-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4ef36-150">Not yet documented</span></span>|
|<span data-ttu-id="4ef36-151">top</span><span class="sxs-lookup"><span data-stu-id="4ef36-151">top</span></span>|<span data-ttu-id="4ef36-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4ef36-152">Int32</span></span>|<span data-ttu-id="4ef36-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4ef36-153">Not yet documented</span></span>|
|<span data-ttu-id="4ef36-154">filter</span><span class="sxs-lookup"><span data-stu-id="4ef36-154">filter</span></span>|<span data-ttu-id="4ef36-155">String</span><span class="sxs-lookup"><span data-stu-id="4ef36-155">String</span></span>|<span data-ttu-id="4ef36-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4ef36-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4ef36-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ef36-157">Response</span></span>
<span data-ttu-id="4ef36-158">При успешном выполнении это действие возвращает `200 OK` код отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ef36-158">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ef36-159">Пример</span><span class="sxs-lookup"><span data-stu-id="4ef36-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ef36-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ef36-160">Request</span></span>
<span data-ttu-id="4ef36-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ef36-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getHistoricalReport

Content-type: application/json
Content-length: 242

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
  "filter": "Filter value"
}
```

### <a name="response"></a><span data-ttu-id="4ef36-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ef36-162">Response</span></span>
<span data-ttu-id="4ef36-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ef36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```





