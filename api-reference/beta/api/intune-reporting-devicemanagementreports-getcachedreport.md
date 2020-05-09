---
title: действие Жеткачедрепорт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86094a4434712c8d49669bcdc92554470318e2cc
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178292"
---
# <a name="getcachedreport-action"></a><span data-ttu-id="77577-103">действие Жеткачедрепорт</span><span class="sxs-lookup"><span data-stu-id="77577-103">getCachedReport action</span></span>

<span data-ttu-id="77577-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77577-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77577-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77577-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77577-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77577-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77577-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="77577-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77577-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="77577-108">Prerequisites</span></span>
<span data-ttu-id="77577-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77577-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77577-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77577-111">Permission type</span></span>|<span data-ttu-id="77577-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77577-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77577-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77577-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77577-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="77577-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="77577-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77577-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77577-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77577-116">Not supported.</span></span>|
|<span data-ttu-id="77577-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77577-117">Application</span></span>|<span data-ttu-id="77577-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="77577-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77577-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77577-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCachedReport
```

## <a name="request-headers"></a><span data-ttu-id="77577-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="77577-120">Request headers</span></span>
|<span data-ttu-id="77577-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77577-121">Header</span></span>|<span data-ttu-id="77577-122">Значение</span><span class="sxs-lookup"><span data-stu-id="77577-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77577-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77577-123">Authorization</span></span>|<span data-ttu-id="77577-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77577-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77577-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77577-125">Accept</span></span>|<span data-ttu-id="77577-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77577-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77577-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77577-127">Request body</span></span>
<span data-ttu-id="77577-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77577-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="77577-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="77577-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="77577-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="77577-130">Property</span></span>|<span data-ttu-id="77577-131">Тип</span><span class="sxs-lookup"><span data-stu-id="77577-131">Type</span></span>|<span data-ttu-id="77577-132">Описание</span><span class="sxs-lookup"><span data-stu-id="77577-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77577-133">id</span><span class="sxs-lookup"><span data-stu-id="77577-133">id</span></span>|<span data-ttu-id="77577-134">Строка</span><span class="sxs-lookup"><span data-stu-id="77577-134">String</span></span>|<span data-ttu-id="77577-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="77577-135">Not yet documented</span></span>|
|<span data-ttu-id="77577-136">select</span><span class="sxs-lookup"><span data-stu-id="77577-136">select</span></span>|<span data-ttu-id="77577-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="77577-137">String collection</span></span>|<span data-ttu-id="77577-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="77577-138">Not yet documented</span></span>|
|<span data-ttu-id="77577-139">search</span><span class="sxs-lookup"><span data-stu-id="77577-139">search</span></span>|<span data-ttu-id="77577-140">String</span><span class="sxs-lookup"><span data-stu-id="77577-140">String</span></span>|<span data-ttu-id="77577-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="77577-141">Not yet documented</span></span>|
|<span data-ttu-id="77577-142">Оператора</span><span class="sxs-lookup"><span data-stu-id="77577-142">groupBy</span></span>|<span data-ttu-id="77577-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="77577-143">String collection</span></span>|<span data-ttu-id="77577-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="77577-144">Not yet documented</span></span>|
|<span data-ttu-id="77577-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="77577-145">orderBy</span></span>|<span data-ttu-id="77577-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="77577-146">String collection</span></span>|<span data-ttu-id="77577-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="77577-147">Not yet documented</span></span>|
|<span data-ttu-id="77577-148">skip</span><span class="sxs-lookup"><span data-stu-id="77577-148">skip</span></span>|<span data-ttu-id="77577-149">Int32</span><span class="sxs-lookup"><span data-stu-id="77577-149">Int32</span></span>|<span data-ttu-id="77577-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="77577-150">Not yet documented</span></span>|
|<span data-ttu-id="77577-151">top</span><span class="sxs-lookup"><span data-stu-id="77577-151">top</span></span>|<span data-ttu-id="77577-152">Int32</span><span class="sxs-lookup"><span data-stu-id="77577-152">Int32</span></span>|<span data-ttu-id="77577-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="77577-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="77577-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="77577-154">Response</span></span>
<span data-ttu-id="77577-155">При успешном выполнении это действие возвращает `200 OK` код отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77577-155">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77577-156">Пример</span><span class="sxs-lookup"><span data-stu-id="77577-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="77577-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="77577-157">Request</span></span>
<span data-ttu-id="77577-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77577-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77577-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="77577-159">Response</span></span>
<span data-ttu-id="77577-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77577-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": "Z2V0Q2FjaGVkUmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDc5MjIxODQ3OA=="
}
```



