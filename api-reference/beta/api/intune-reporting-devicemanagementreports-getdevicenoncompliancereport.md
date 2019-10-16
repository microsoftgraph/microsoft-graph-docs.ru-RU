---
title: действие Жетдевиценонкомплианцерепорт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c396d75edfa23583646a024f2eaba82335604186
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537242"
---
# <a name="getdevicenoncompliancereport-action"></a><span data-ttu-id="fcdbf-103">действие Жетдевиценонкомплианцерепорт</span><span class="sxs-lookup"><span data-stu-id="fcdbf-103">getDeviceNonComplianceReport action</span></span>

> <span data-ttu-id="fcdbf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcdbf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcdbf-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcdbf-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fcdbf-107">Prerequisites</span></span>
<span data-ttu-id="fcdbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcdbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcdbf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcdbf-110">Permission type</span></span>|<span data-ttu-id="fcdbf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcdbf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcdbf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcdbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fcdbf-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="fcdbf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fcdbf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcdbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcdbf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-115">Not supported.</span></span>|
|<span data-ttu-id="fcdbf-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fcdbf-116">Application</span></span>|<span data-ttu-id="fcdbf-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="fcdbf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcdbf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcdbf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getDeviceNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="fcdbf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcdbf-119">Request headers</span></span>
|<span data-ttu-id="fcdbf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcdbf-120">Header</span></span>|<span data-ttu-id="fcdbf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fcdbf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcdbf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcdbf-122">Authorization</span></span>|<span data-ttu-id="fcdbf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcdbf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fcdbf-124">Accept</span></span>|<span data-ttu-id="fcdbf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fcdbf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcdbf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcdbf-126">Request body</span></span>
<span data-ttu-id="fcdbf-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fcdbf-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fcdbf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcdbf-129">Property</span></span>|<span data-ttu-id="fcdbf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fcdbf-130">Type</span></span>|<span data-ttu-id="fcdbf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fcdbf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcdbf-132">name</span><span class="sxs-lookup"><span data-stu-id="fcdbf-132">name</span></span>|<span data-ttu-id="fcdbf-133">String</span><span class="sxs-lookup"><span data-stu-id="fcdbf-133">String</span></span>|<span data-ttu-id="fcdbf-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-134">Not yet documented</span></span>|
|<span data-ttu-id="fcdbf-135">select</span><span class="sxs-lookup"><span data-stu-id="fcdbf-135">select</span></span>|<span data-ttu-id="fcdbf-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fcdbf-136">String collection</span></span>|<span data-ttu-id="fcdbf-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fcdbf-137">Not yet documented</span></span>|
|<span data-ttu-id="fcdbf-138">search</span><span class="sxs-lookup"><span data-stu-id="fcdbf-138">search</span></span>|<span data-ttu-id="fcdbf-139">String</span><span class="sxs-lookup"><span data-stu-id="fcdbf-139">String</span></span>|<span data-ttu-id="fcdbf-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-140">Not yet documented</span></span>|
|<span data-ttu-id="fcdbf-141">Оператора</span><span class="sxs-lookup"><span data-stu-id="fcdbf-141">groupBy</span></span>|<span data-ttu-id="fcdbf-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fcdbf-142">String collection</span></span>|<span data-ttu-id="fcdbf-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fcdbf-143">Not yet documented</span></span>|
|<span data-ttu-id="fcdbf-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="fcdbf-144">orderBy</span></span>|<span data-ttu-id="fcdbf-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fcdbf-145">String collection</span></span>|<span data-ttu-id="fcdbf-146">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fcdbf-146">Not yet documented</span></span>|
|<span data-ttu-id="fcdbf-147">skip</span><span class="sxs-lookup"><span data-stu-id="fcdbf-147">skip</span></span>|<span data-ttu-id="fcdbf-148">Int32</span><span class="sxs-lookup"><span data-stu-id="fcdbf-148">Int32</span></span>|<span data-ttu-id="fcdbf-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-149">Not yet documented</span></span>|
|<span data-ttu-id="fcdbf-150">top</span><span class="sxs-lookup"><span data-stu-id="fcdbf-150">top</span></span>|<span data-ttu-id="fcdbf-151">Int32</span><span class="sxs-lookup"><span data-stu-id="fcdbf-151">Int32</span></span>|<span data-ttu-id="fcdbf-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-152">Not yet documented</span></span>|
|<span data-ttu-id="fcdbf-153">sessionId</span><span class="sxs-lookup"><span data-stu-id="fcdbf-153">sessionId</span></span>|<span data-ttu-id="fcdbf-154">String</span><span class="sxs-lookup"><span data-stu-id="fcdbf-154">String</span></span>|<span data-ttu-id="fcdbf-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-155">Not yet documented</span></span>|
|<span data-ttu-id="fcdbf-156">filter</span><span class="sxs-lookup"><span data-stu-id="fcdbf-156">filter</span></span>|<span data-ttu-id="fcdbf-157">String</span><span class="sxs-lookup"><span data-stu-id="fcdbf-157">String</span></span>|<span data-ttu-id="fcdbf-158">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fcdbf-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fcdbf-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcdbf-159">Response</span></span>
<span data-ttu-id="fcdbf-160">При успешном выполнении это действие возвращает `200 OK` код отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcdbf-161">Пример</span><span class="sxs-lookup"><span data-stu-id="fcdbf-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcdbf-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcdbf-162">Request</span></span>
<span data-ttu-id="fcdbf-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fcdbf-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcdbf-164">Response</span></span>
<span data-ttu-id="fcdbf-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcdbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```






