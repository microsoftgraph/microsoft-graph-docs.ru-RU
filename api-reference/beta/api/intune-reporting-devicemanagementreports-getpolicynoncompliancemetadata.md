---
title: действие Жетполицинонкомплианцеметадата
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de8bddbcc6abe40e6fb60bcaf3644a7ea3c953f6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472328"
---
# <a name="getpolicynoncompliancemetadata-action"></a><span data-ttu-id="3b9fa-103">действие Жетполицинонкомплианцеметадата</span><span class="sxs-lookup"><span data-stu-id="3b9fa-103">getPolicyNonComplianceMetadata action</span></span>

<span data-ttu-id="3b9fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b9fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b9fa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b9fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b9fa-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b9fa-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3b9fa-108">Prerequisites</span></span>
<span data-ttu-id="3b9fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b9fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b9fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b9fa-111">Permission type</span></span>|<span data-ttu-id="3b9fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b9fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b9fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b9fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b9fa-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3b9fa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3b9fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b9fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b9fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-116">Not supported.</span></span>|
|<span data-ttu-id="3b9fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b9fa-117">Application</span></span>|<span data-ttu-id="3b9fa-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3b9fa-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b9fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b9fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNonComplianceMetadata
```

## <a name="request-headers"></a><span data-ttu-id="3b9fa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3b9fa-120">Request headers</span></span>
|<span data-ttu-id="3b9fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b9fa-121">Header</span></span>|<span data-ttu-id="3b9fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3b9fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b9fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b9fa-123">Authorization</span></span>|<span data-ttu-id="3b9fa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b9fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b9fa-125">Accept</span></span>|<span data-ttu-id="3b9fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b9fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b9fa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b9fa-127">Request body</span></span>
<span data-ttu-id="3b9fa-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3b9fa-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3b9fa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b9fa-130">Property</span></span>|<span data-ttu-id="3b9fa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b9fa-131">Type</span></span>|<span data-ttu-id="3b9fa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b9fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b9fa-133">name</span><span class="sxs-lookup"><span data-stu-id="3b9fa-133">name</span></span>|<span data-ttu-id="3b9fa-134">String</span><span class="sxs-lookup"><span data-stu-id="3b9fa-134">String</span></span>|<span data-ttu-id="3b9fa-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-135">Not yet documented</span></span>|
|<span data-ttu-id="3b9fa-136">select</span><span class="sxs-lookup"><span data-stu-id="3b9fa-136">select</span></span>|<span data-ttu-id="3b9fa-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3b9fa-137">String collection</span></span>|<span data-ttu-id="3b9fa-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3b9fa-138">Not yet documented</span></span>|
|<span data-ttu-id="3b9fa-139">search</span><span class="sxs-lookup"><span data-stu-id="3b9fa-139">search</span></span>|<span data-ttu-id="3b9fa-140">String</span><span class="sxs-lookup"><span data-stu-id="3b9fa-140">String</span></span>|<span data-ttu-id="3b9fa-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-141">Not yet documented</span></span>|
|<span data-ttu-id="3b9fa-142">Оператора</span><span class="sxs-lookup"><span data-stu-id="3b9fa-142">groupBy</span></span>|<span data-ttu-id="3b9fa-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3b9fa-143">String collection</span></span>|<span data-ttu-id="3b9fa-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3b9fa-144">Not yet documented</span></span>|
|<span data-ttu-id="3b9fa-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="3b9fa-145">orderBy</span></span>|<span data-ttu-id="3b9fa-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3b9fa-146">String collection</span></span>|<span data-ttu-id="3b9fa-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3b9fa-147">Not yet documented</span></span>|
|<span data-ttu-id="3b9fa-148">skip</span><span class="sxs-lookup"><span data-stu-id="3b9fa-148">skip</span></span>|<span data-ttu-id="3b9fa-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3b9fa-149">Int32</span></span>|<span data-ttu-id="3b9fa-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-150">Not yet documented</span></span>|
|<span data-ttu-id="3b9fa-151">top</span><span class="sxs-lookup"><span data-stu-id="3b9fa-151">top</span></span>|<span data-ttu-id="3b9fa-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3b9fa-152">Int32</span></span>|<span data-ttu-id="3b9fa-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-153">Not yet documented</span></span>|
|<span data-ttu-id="3b9fa-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="3b9fa-154">sessionId</span></span>|<span data-ttu-id="3b9fa-155">String</span><span class="sxs-lookup"><span data-stu-id="3b9fa-155">String</span></span>|<span data-ttu-id="3b9fa-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-156">Not yet documented</span></span>|
|<span data-ttu-id="3b9fa-157">filter</span><span class="sxs-lookup"><span data-stu-id="3b9fa-157">filter</span></span>|<span data-ttu-id="3b9fa-158">String</span><span class="sxs-lookup"><span data-stu-id="3b9fa-158">String</span></span>|<span data-ttu-id="3b9fa-159">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3b9fa-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3b9fa-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b9fa-160">Response</span></span>
<span data-ttu-id="3b9fa-161">При успешном выполнении это действие возвращает `200 OK` код отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b9fa-162">Пример</span><span class="sxs-lookup"><span data-stu-id="3b9fa-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b9fa-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b9fa-163">Request</span></span>
<span data-ttu-id="3b9fa-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getPolicyNonComplianceMetadata

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

### <a name="response"></a><span data-ttu-id="3b9fa-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b9fa-165">Response</span></span>
<span data-ttu-id="3b9fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b9fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```



