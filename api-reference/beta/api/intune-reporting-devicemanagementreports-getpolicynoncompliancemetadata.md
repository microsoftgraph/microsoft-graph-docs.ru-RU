---
title: действие getPolicyNonComplianceMetadata
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a4b97e410f7c0a303f290b5c970ce05dd32b2b5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156473"
---
# <a name="getpolicynoncompliancemetadata-action"></a><span data-ttu-id="d3a48-103">действие getPolicyNonComplianceMetadata</span><span class="sxs-lookup"><span data-stu-id="d3a48-103">getPolicyNonComplianceMetadata action</span></span>

<span data-ttu-id="d3a48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3a48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3a48-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3a48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3a48-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3a48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3a48-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d3a48-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3a48-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d3a48-108">Prerequisites</span></span>
<span data-ttu-id="d3a48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3a48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3a48-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3a48-111">Permission type</span></span>|<span data-ttu-id="d3a48-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3a48-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3a48-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3a48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3a48-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3a48-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d3a48-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3a48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3a48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3a48-116">Not supported.</span></span>|
|<span data-ttu-id="d3a48-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d3a48-117">Application</span></span>|<span data-ttu-id="d3a48-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3a48-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3a48-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3a48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNonComplianceMetadata
```

## <a name="request-headers"></a><span data-ttu-id="d3a48-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d3a48-120">Request headers</span></span>
|<span data-ttu-id="d3a48-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3a48-121">Header</span></span>|<span data-ttu-id="d3a48-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d3a48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3a48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3a48-123">Authorization</span></span>|<span data-ttu-id="d3a48-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3a48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3a48-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3a48-125">Accept</span></span>|<span data-ttu-id="d3a48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3a48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3a48-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3a48-127">Request body</span></span>
<span data-ttu-id="d3a48-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3a48-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d3a48-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d3a48-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d3a48-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3a48-130">Property</span></span>|<span data-ttu-id="d3a48-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d3a48-131">Type</span></span>|<span data-ttu-id="d3a48-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d3a48-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3a48-133">name</span><span class="sxs-lookup"><span data-stu-id="d3a48-133">name</span></span>|<span data-ttu-id="d3a48-134">String</span><span class="sxs-lookup"><span data-stu-id="d3a48-134">String</span></span>|<span data-ttu-id="d3a48-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d3a48-135">Not yet documented</span></span>|
|<span data-ttu-id="d3a48-136">select</span><span class="sxs-lookup"><span data-stu-id="d3a48-136">select</span></span>|<span data-ttu-id="d3a48-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d3a48-137">String collection</span></span>|<span data-ttu-id="d3a48-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3a48-138">Not yet documented</span></span>|
|<span data-ttu-id="d3a48-139">search</span><span class="sxs-lookup"><span data-stu-id="d3a48-139">search</span></span>|<span data-ttu-id="d3a48-140">String</span><span class="sxs-lookup"><span data-stu-id="d3a48-140">String</span></span>|<span data-ttu-id="d3a48-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d3a48-141">Not yet documented</span></span>|
|<span data-ttu-id="d3a48-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="d3a48-142">groupBy</span></span>|<span data-ttu-id="d3a48-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d3a48-143">String collection</span></span>|<span data-ttu-id="d3a48-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3a48-144">Not yet documented</span></span>|
|<span data-ttu-id="d3a48-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="d3a48-145">orderBy</span></span>|<span data-ttu-id="d3a48-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d3a48-146">String collection</span></span>|<span data-ttu-id="d3a48-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3a48-147">Not yet documented</span></span>|
|<span data-ttu-id="d3a48-148">skip</span><span class="sxs-lookup"><span data-stu-id="d3a48-148">skip</span></span>|<span data-ttu-id="d3a48-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d3a48-149">Int32</span></span>|<span data-ttu-id="d3a48-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d3a48-150">Not yet documented</span></span>|
|<span data-ttu-id="d3a48-151">top</span><span class="sxs-lookup"><span data-stu-id="d3a48-151">top</span></span>|<span data-ttu-id="d3a48-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d3a48-152">Int32</span></span>|<span data-ttu-id="d3a48-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d3a48-153">Not yet documented</span></span>|
|<span data-ttu-id="d3a48-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="d3a48-154">sessionId</span></span>|<span data-ttu-id="d3a48-155">String</span><span class="sxs-lookup"><span data-stu-id="d3a48-155">String</span></span>|<span data-ttu-id="d3a48-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d3a48-156">Not yet documented</span></span>|
|<span data-ttu-id="d3a48-157">filter</span><span class="sxs-lookup"><span data-stu-id="d3a48-157">filter</span></span>|<span data-ttu-id="d3a48-158">String</span><span class="sxs-lookup"><span data-stu-id="d3a48-158">String</span></span>|<span data-ttu-id="d3a48-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d3a48-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d3a48-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3a48-160">Response</span></span>
<span data-ttu-id="d3a48-161">В случае успешного действия это действие возвращает код `200 OK` отклика и поток в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d3a48-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3a48-162">Пример</span><span class="sxs-lookup"><span data-stu-id="d3a48-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3a48-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3a48-163">Request</span></span>
<span data-ttu-id="d3a48-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3a48-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3a48-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3a48-165">Response</span></span>
<span data-ttu-id="d3a48-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3a48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 99

{
  "value": "Z2V0UG9saWN5Tm9uQ29tcGxpYW5jZU1ldGFkYXRhIEludHVuZSBEb2MgU2FtcGxlIC0xNzM5NTg5Nzc5"
}
```




