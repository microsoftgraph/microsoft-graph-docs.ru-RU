---
title: действие getCachedReport
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b38f720f18966e7f628819ba57f348d4055acc3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156592"
---
# <a name="getcachedreport-action"></a><span data-ttu-id="13470-103">действие getCachedReport</span><span class="sxs-lookup"><span data-stu-id="13470-103">getCachedReport action</span></span>

<span data-ttu-id="13470-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13470-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13470-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13470-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13470-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13470-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13470-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="13470-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13470-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="13470-108">Prerequisites</span></span>
<span data-ttu-id="13470-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13470-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13470-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13470-111">Permission type</span></span>|<span data-ttu-id="13470-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13470-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13470-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13470-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13470-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13470-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="13470-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13470-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13470-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13470-116">Not supported.</span></span>|
|<span data-ttu-id="13470-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="13470-117">Application</span></span>|<span data-ttu-id="13470-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13470-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13470-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13470-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCachedReport
```

## <a name="request-headers"></a><span data-ttu-id="13470-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="13470-120">Request headers</span></span>
|<span data-ttu-id="13470-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13470-121">Header</span></span>|<span data-ttu-id="13470-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13470-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13470-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13470-123">Authorization</span></span>|<span data-ttu-id="13470-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13470-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13470-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13470-125">Accept</span></span>|<span data-ttu-id="13470-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13470-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13470-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13470-127">Request body</span></span>
<span data-ttu-id="13470-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13470-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="13470-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="13470-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="13470-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="13470-130">Property</span></span>|<span data-ttu-id="13470-131">Тип</span><span class="sxs-lookup"><span data-stu-id="13470-131">Type</span></span>|<span data-ttu-id="13470-132">Описание</span><span class="sxs-lookup"><span data-stu-id="13470-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13470-133">id</span><span class="sxs-lookup"><span data-stu-id="13470-133">id</span></span>|<span data-ttu-id="13470-134">Строка</span><span class="sxs-lookup"><span data-stu-id="13470-134">String</span></span>|<span data-ttu-id="13470-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="13470-135">Not yet documented</span></span>|
|<span data-ttu-id="13470-136">select</span><span class="sxs-lookup"><span data-stu-id="13470-136">select</span></span>|<span data-ttu-id="13470-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="13470-137">String collection</span></span>|<span data-ttu-id="13470-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="13470-138">Not yet documented</span></span>|
|<span data-ttu-id="13470-139">search</span><span class="sxs-lookup"><span data-stu-id="13470-139">search</span></span>|<span data-ttu-id="13470-140">String</span><span class="sxs-lookup"><span data-stu-id="13470-140">String</span></span>|<span data-ttu-id="13470-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="13470-141">Not yet documented</span></span>|
|<span data-ttu-id="13470-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="13470-142">groupBy</span></span>|<span data-ttu-id="13470-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="13470-143">String collection</span></span>|<span data-ttu-id="13470-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="13470-144">Not yet documented</span></span>|
|<span data-ttu-id="13470-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="13470-145">orderBy</span></span>|<span data-ttu-id="13470-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="13470-146">String collection</span></span>|<span data-ttu-id="13470-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="13470-147">Not yet documented</span></span>|
|<span data-ttu-id="13470-148">skip</span><span class="sxs-lookup"><span data-stu-id="13470-148">skip</span></span>|<span data-ttu-id="13470-149">Int32</span><span class="sxs-lookup"><span data-stu-id="13470-149">Int32</span></span>|<span data-ttu-id="13470-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="13470-150">Not yet documented</span></span>|
|<span data-ttu-id="13470-151">top</span><span class="sxs-lookup"><span data-stu-id="13470-151">top</span></span>|<span data-ttu-id="13470-152">Int32</span><span class="sxs-lookup"><span data-stu-id="13470-152">Int32</span></span>|<span data-ttu-id="13470-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="13470-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="13470-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="13470-154">Response</span></span>
<span data-ttu-id="13470-155">В случае успешного действия это действие возвращает код `200 OK` отклика и поток в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="13470-155">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13470-156">Пример</span><span class="sxs-lookup"><span data-stu-id="13470-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="13470-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="13470-157">Request</span></span>
<span data-ttu-id="13470-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13470-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getCachedReport

Content-type: application/json
Content-length: 209

{
  "id": "Id value",
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
  "top": 3
}
```

### <a name="response"></a><span data-ttu-id="13470-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="13470-159">Response</span></span>
<span data-ttu-id="13470-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13470-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": "Z2V0Q2FjaGVkUmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDc5MjIxODQ3OA=="
}
```




