---
title: действие Жесисторикалрепорт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a378b673fdedbaa695ce64f1250be87b675f95d
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178278"
---
# <a name="gethistoricalreport-action"></a><span data-ttu-id="6569f-103">действие Жесисторикалрепорт</span><span class="sxs-lookup"><span data-stu-id="6569f-103">getHistoricalReport action</span></span>

<span data-ttu-id="6569f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6569f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6569f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6569f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6569f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6569f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6569f-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6569f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6569f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6569f-108">Prerequisites</span></span>
<span data-ttu-id="6569f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6569f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6569f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6569f-111">Permission type</span></span>|<span data-ttu-id="6569f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6569f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6569f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6569f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6569f-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="6569f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6569f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6569f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6569f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6569f-116">Not supported.</span></span>|
|<span data-ttu-id="6569f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6569f-117">Application</span></span>|<span data-ttu-id="6569f-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="6569f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6569f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6569f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getHistoricalReport
```

## <a name="request-headers"></a><span data-ttu-id="6569f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6569f-120">Request headers</span></span>
|<span data-ttu-id="6569f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6569f-121">Header</span></span>|<span data-ttu-id="6569f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6569f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6569f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6569f-123">Authorization</span></span>|<span data-ttu-id="6569f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6569f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6569f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6569f-125">Accept</span></span>|<span data-ttu-id="6569f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6569f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6569f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6569f-127">Request body</span></span>
<span data-ttu-id="6569f-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6569f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6569f-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="6569f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6569f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6569f-130">Property</span></span>|<span data-ttu-id="6569f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6569f-131">Type</span></span>|<span data-ttu-id="6569f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6569f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6569f-133">name</span><span class="sxs-lookup"><span data-stu-id="6569f-133">name</span></span>|<span data-ttu-id="6569f-134">String</span><span class="sxs-lookup"><span data-stu-id="6569f-134">String</span></span>|<span data-ttu-id="6569f-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6569f-135">Not yet documented</span></span>|
|<span data-ttu-id="6569f-136">select</span><span class="sxs-lookup"><span data-stu-id="6569f-136">select</span></span>|<span data-ttu-id="6569f-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6569f-137">String collection</span></span>|<span data-ttu-id="6569f-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6569f-138">Not yet documented</span></span>|
|<span data-ttu-id="6569f-139">search</span><span class="sxs-lookup"><span data-stu-id="6569f-139">search</span></span>|<span data-ttu-id="6569f-140">String</span><span class="sxs-lookup"><span data-stu-id="6569f-140">String</span></span>|<span data-ttu-id="6569f-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6569f-141">Not yet documented</span></span>|
|<span data-ttu-id="6569f-142">Оператора</span><span class="sxs-lookup"><span data-stu-id="6569f-142">groupBy</span></span>|<span data-ttu-id="6569f-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6569f-143">String collection</span></span>|<span data-ttu-id="6569f-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6569f-144">Not yet documented</span></span>|
|<span data-ttu-id="6569f-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="6569f-145">orderBy</span></span>|<span data-ttu-id="6569f-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6569f-146">String collection</span></span>|<span data-ttu-id="6569f-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6569f-147">Not yet documented</span></span>|
|<span data-ttu-id="6569f-148">skip</span><span class="sxs-lookup"><span data-stu-id="6569f-148">skip</span></span>|<span data-ttu-id="6569f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6569f-149">Int32</span></span>|<span data-ttu-id="6569f-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6569f-150">Not yet documented</span></span>|
|<span data-ttu-id="6569f-151">top</span><span class="sxs-lookup"><span data-stu-id="6569f-151">top</span></span>|<span data-ttu-id="6569f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6569f-152">Int32</span></span>|<span data-ttu-id="6569f-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6569f-153">Not yet documented</span></span>|
|<span data-ttu-id="6569f-154">filter</span><span class="sxs-lookup"><span data-stu-id="6569f-154">filter</span></span>|<span data-ttu-id="6569f-155">String</span><span class="sxs-lookup"><span data-stu-id="6569f-155">String</span></span>|<span data-ttu-id="6569f-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6569f-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6569f-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="6569f-157">Response</span></span>
<span data-ttu-id="6569f-158">При успешном выполнении это действие возвращает `200 OK` код отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6569f-158">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6569f-159">Пример</span><span class="sxs-lookup"><span data-stu-id="6569f-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="6569f-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="6569f-160">Request</span></span>
<span data-ttu-id="6569f-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6569f-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6569f-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="6569f-162">Response</span></span>
<span data-ttu-id="6569f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6569f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 83

{
  "value": "Z2V0SGlzdG9yaWNhbFJlcG9ydCBJbnR1bmUgRG9jIFNhbXBsZSAxNjE5NjA4MTY0"
}
```



