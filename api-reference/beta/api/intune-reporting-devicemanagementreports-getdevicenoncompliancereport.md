---
title: действие Жетдевиценонкомплианцерепорт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7712c8944dcce5672c793c8d97c2f90f2a595e7d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698192"
---
# <a name="getdevicenoncompliancereport-action"></a><span data-ttu-id="677f6-103">действие Жетдевиценонкомплианцерепорт</span><span class="sxs-lookup"><span data-stu-id="677f6-103">getDeviceNonComplianceReport action</span></span>

<span data-ttu-id="677f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="677f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="677f6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="677f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="677f6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="677f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="677f6-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="677f6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="677f6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="677f6-108">Prerequisites</span></span>
<span data-ttu-id="677f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="677f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="677f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="677f6-111">Permission type</span></span>|<span data-ttu-id="677f6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="677f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="677f6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="677f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="677f6-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="677f6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="677f6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="677f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="677f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="677f6-116">Not supported.</span></span>|
|<span data-ttu-id="677f6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="677f6-117">Application</span></span>|<span data-ttu-id="677f6-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="677f6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="677f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="677f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getDeviceNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="677f6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="677f6-120">Request headers</span></span>
|<span data-ttu-id="677f6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="677f6-121">Header</span></span>|<span data-ttu-id="677f6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="677f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="677f6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="677f6-123">Authorization</span></span>|<span data-ttu-id="677f6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="677f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="677f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="677f6-125">Accept</span></span>|<span data-ttu-id="677f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="677f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="677f6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="677f6-127">Request body</span></span>
<span data-ttu-id="677f6-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="677f6-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="677f6-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="677f6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="677f6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="677f6-130">Property</span></span>|<span data-ttu-id="677f6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="677f6-131">Type</span></span>|<span data-ttu-id="677f6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="677f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="677f6-133">name</span><span class="sxs-lookup"><span data-stu-id="677f6-133">name</span></span>|<span data-ttu-id="677f6-134">String</span><span class="sxs-lookup"><span data-stu-id="677f6-134">String</span></span>|<span data-ttu-id="677f6-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="677f6-135">Not yet documented</span></span>|
|<span data-ttu-id="677f6-136">select</span><span class="sxs-lookup"><span data-stu-id="677f6-136">select</span></span>|<span data-ttu-id="677f6-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="677f6-137">String collection</span></span>|<span data-ttu-id="677f6-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="677f6-138">Not yet documented</span></span>|
|<span data-ttu-id="677f6-139">search</span><span class="sxs-lookup"><span data-stu-id="677f6-139">search</span></span>|<span data-ttu-id="677f6-140">String</span><span class="sxs-lookup"><span data-stu-id="677f6-140">String</span></span>|<span data-ttu-id="677f6-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="677f6-141">Not yet documented</span></span>|
|<span data-ttu-id="677f6-142">Оператора</span><span class="sxs-lookup"><span data-stu-id="677f6-142">groupBy</span></span>|<span data-ttu-id="677f6-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="677f6-143">String collection</span></span>|<span data-ttu-id="677f6-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="677f6-144">Not yet documented</span></span>|
|<span data-ttu-id="677f6-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="677f6-145">orderBy</span></span>|<span data-ttu-id="677f6-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="677f6-146">String collection</span></span>|<span data-ttu-id="677f6-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="677f6-147">Not yet documented</span></span>|
|<span data-ttu-id="677f6-148">skip</span><span class="sxs-lookup"><span data-stu-id="677f6-148">skip</span></span>|<span data-ttu-id="677f6-149">Int32</span><span class="sxs-lookup"><span data-stu-id="677f6-149">Int32</span></span>|<span data-ttu-id="677f6-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="677f6-150">Not yet documented</span></span>|
|<span data-ttu-id="677f6-151">top</span><span class="sxs-lookup"><span data-stu-id="677f6-151">top</span></span>|<span data-ttu-id="677f6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="677f6-152">Int32</span></span>|<span data-ttu-id="677f6-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="677f6-153">Not yet documented</span></span>|
|<span data-ttu-id="677f6-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="677f6-154">sessionId</span></span>|<span data-ttu-id="677f6-155">String</span><span class="sxs-lookup"><span data-stu-id="677f6-155">String</span></span>|<span data-ttu-id="677f6-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="677f6-156">Not yet documented</span></span>|
|<span data-ttu-id="677f6-157">filter</span><span class="sxs-lookup"><span data-stu-id="677f6-157">filter</span></span>|<span data-ttu-id="677f6-158">String</span><span class="sxs-lookup"><span data-stu-id="677f6-158">String</span></span>|<span data-ttu-id="677f6-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="677f6-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="677f6-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="677f6-160">Response</span></span>
<span data-ttu-id="677f6-161">При успешном выполнении это действие возвращает `200 OK` код отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="677f6-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="677f6-162">Пример</span><span class="sxs-lookup"><span data-stu-id="677f6-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="677f6-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="677f6-163">Request</span></span>
<span data-ttu-id="677f6-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="677f6-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getDeviceNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="677f6-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="677f6-165">Response</span></span>
<span data-ttu-id="677f6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="677f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 99

{
  "value": "Z2V0RGV2aWNlTm9uQ29tcGxpYW5jZVJlcG9ydCBJbnR1bmUgRG9jIFNhbXBsZSAtMTY1MDA3NDI3OA=="
}
```





