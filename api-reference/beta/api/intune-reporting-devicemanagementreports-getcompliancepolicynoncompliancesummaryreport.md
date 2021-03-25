---
title: getCompliancePolicyNonComplianceSummaryReport action
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e55bb442f88f22271b5a9b814d912cddf97be77
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156543"
---
# <a name="getcompliancepolicynoncompliancesummaryreport-action"></a><span data-ttu-id="cd503-103">getCompliancePolicyNonComplianceSummaryReport action</span><span class="sxs-lookup"><span data-stu-id="cd503-103">getCompliancePolicyNonComplianceSummaryReport action</span></span>

<span data-ttu-id="cd503-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd503-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd503-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd503-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd503-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd503-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd503-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd503-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd503-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cd503-108">Prerequisites</span></span>
<span data-ttu-id="cd503-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd503-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd503-111">Permission type</span></span>|<span data-ttu-id="cd503-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd503-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd503-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd503-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd503-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd503-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cd503-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd503-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd503-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd503-116">Not supported.</span></span>|
|<span data-ttu-id="cd503-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cd503-117">Application</span></span>|<span data-ttu-id="cd503-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd503-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd503-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd503-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCompliancePolicyNonComplianceSummaryReport
```

## <a name="request-headers"></a><span data-ttu-id="cd503-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cd503-120">Request headers</span></span>
|<span data-ttu-id="cd503-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd503-121">Header</span></span>|<span data-ttu-id="cd503-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cd503-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd503-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd503-123">Authorization</span></span>|<span data-ttu-id="cd503-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd503-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd503-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cd503-125">Accept</span></span>|<span data-ttu-id="cd503-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd503-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd503-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd503-127">Request body</span></span>
<span data-ttu-id="cd503-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd503-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cd503-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="cd503-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cd503-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd503-130">Property</span></span>|<span data-ttu-id="cd503-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cd503-131">Type</span></span>|<span data-ttu-id="cd503-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cd503-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd503-133">name</span><span class="sxs-lookup"><span data-stu-id="cd503-133">name</span></span>|<span data-ttu-id="cd503-134">String</span><span class="sxs-lookup"><span data-stu-id="cd503-134">String</span></span>|<span data-ttu-id="cd503-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd503-135">Not yet documented</span></span>|
|<span data-ttu-id="cd503-136">select</span><span class="sxs-lookup"><span data-stu-id="cd503-136">select</span></span>|<span data-ttu-id="cd503-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cd503-137">String collection</span></span>|<span data-ttu-id="cd503-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cd503-138">Not yet documented</span></span>|
|<span data-ttu-id="cd503-139">search</span><span class="sxs-lookup"><span data-stu-id="cd503-139">search</span></span>|<span data-ttu-id="cd503-140">String</span><span class="sxs-lookup"><span data-stu-id="cd503-140">String</span></span>|<span data-ttu-id="cd503-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd503-141">Not yet documented</span></span>|
|<span data-ttu-id="cd503-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="cd503-142">groupBy</span></span>|<span data-ttu-id="cd503-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cd503-143">String collection</span></span>|<span data-ttu-id="cd503-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cd503-144">Not yet documented</span></span>|
|<span data-ttu-id="cd503-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="cd503-145">orderBy</span></span>|<span data-ttu-id="cd503-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cd503-146">String collection</span></span>|<span data-ttu-id="cd503-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cd503-147">Not yet documented</span></span>|
|<span data-ttu-id="cd503-148">skip</span><span class="sxs-lookup"><span data-stu-id="cd503-148">skip</span></span>|<span data-ttu-id="cd503-149">Int32</span><span class="sxs-lookup"><span data-stu-id="cd503-149">Int32</span></span>|<span data-ttu-id="cd503-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd503-150">Not yet documented</span></span>|
|<span data-ttu-id="cd503-151">top</span><span class="sxs-lookup"><span data-stu-id="cd503-151">top</span></span>|<span data-ttu-id="cd503-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cd503-152">Int32</span></span>|<span data-ttu-id="cd503-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd503-153">Not yet documented</span></span>|
|<span data-ttu-id="cd503-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="cd503-154">sessionId</span></span>|<span data-ttu-id="cd503-155">String</span><span class="sxs-lookup"><span data-stu-id="cd503-155">String</span></span>|<span data-ttu-id="cd503-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd503-156">Not yet documented</span></span>|
|<span data-ttu-id="cd503-157">filter</span><span class="sxs-lookup"><span data-stu-id="cd503-157">filter</span></span>|<span data-ttu-id="cd503-158">String</span><span class="sxs-lookup"><span data-stu-id="cd503-158">String</span></span>|<span data-ttu-id="cd503-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd503-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cd503-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd503-160">Response</span></span>
<span data-ttu-id="cd503-161">В случае успешного действия это действие возвращает код `200 OK` отклика и поток в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cd503-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd503-162">Пример</span><span class="sxs-lookup"><span data-stu-id="cd503-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd503-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd503-163">Request</span></span>
<span data-ttu-id="cd503-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd503-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getCompliancePolicyNonComplianceSummaryReport

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

### <a name="response"></a><span data-ttu-id="cd503-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd503-165">Response</span></span>
<span data-ttu-id="cd503-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd503-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 119

{
  "value": "Z2V0Q29tcGxpYW5jZVBvbGljeU5vbkNvbXBsaWFuY2VTdW1tYXJ5UmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDg4MTYwMDMxNQ=="
}
```




