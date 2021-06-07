---
title: getConfigurationPolicyNonComplianceReport action
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11206867779cadf14d4f19d7c14e84a0242be085
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52749041"
---
# <a name="getconfigurationpolicynoncompliancereport-action"></a><span data-ttu-id="302fe-103">getConfigurationPolicyNonComplianceReport action</span><span class="sxs-lookup"><span data-stu-id="302fe-103">getConfigurationPolicyNonComplianceReport action</span></span>

<span data-ttu-id="302fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="302fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="302fe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="302fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="302fe-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="302fe-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="302fe-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="302fe-107">Prerequisites</span></span>
<span data-ttu-id="302fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="302fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="302fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="302fe-110">Permission type</span></span>|<span data-ttu-id="302fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="302fe-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="302fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="302fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="302fe-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="302fe-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="302fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="302fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="302fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="302fe-115">Not supported.</span></span>|
|<span data-ttu-id="302fe-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="302fe-116">Application</span></span>|<span data-ttu-id="302fe-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="302fe-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="302fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="302fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getConfigurationPolicyNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="302fe-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="302fe-119">Request headers</span></span>
|<span data-ttu-id="302fe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="302fe-120">Header</span></span>|<span data-ttu-id="302fe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="302fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="302fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="302fe-122">Authorization</span></span>|<span data-ttu-id="302fe-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="302fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="302fe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="302fe-124">Accept</span></span>|<span data-ttu-id="302fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="302fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="302fe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="302fe-126">Request body</span></span>
<span data-ttu-id="302fe-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="302fe-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="302fe-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="302fe-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="302fe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="302fe-129">Property</span></span>|<span data-ttu-id="302fe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="302fe-130">Type</span></span>|<span data-ttu-id="302fe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="302fe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="302fe-132">name</span><span class="sxs-lookup"><span data-stu-id="302fe-132">name</span></span>|<span data-ttu-id="302fe-133">String</span><span class="sxs-lookup"><span data-stu-id="302fe-133">String</span></span>|<span data-ttu-id="302fe-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="302fe-134">Not yet documented</span></span>|
|<span data-ttu-id="302fe-135">select</span><span class="sxs-lookup"><span data-stu-id="302fe-135">select</span></span>|<span data-ttu-id="302fe-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="302fe-136">String collection</span></span>|<span data-ttu-id="302fe-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="302fe-137">Not yet documented</span></span>|
|<span data-ttu-id="302fe-138">search</span><span class="sxs-lookup"><span data-stu-id="302fe-138">search</span></span>|<span data-ttu-id="302fe-139">String</span><span class="sxs-lookup"><span data-stu-id="302fe-139">String</span></span>|<span data-ttu-id="302fe-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="302fe-140">Not yet documented</span></span>|
|<span data-ttu-id="302fe-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="302fe-141">groupBy</span></span>|<span data-ttu-id="302fe-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="302fe-142">String collection</span></span>|<span data-ttu-id="302fe-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="302fe-143">Not yet documented</span></span>|
|<span data-ttu-id="302fe-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="302fe-144">orderBy</span></span>|<span data-ttu-id="302fe-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="302fe-145">String collection</span></span>|<span data-ttu-id="302fe-146">Н/Д</span><span class="sxs-lookup"><span data-stu-id="302fe-146">Not yet documented</span></span>|
|<span data-ttu-id="302fe-147">skip</span><span class="sxs-lookup"><span data-stu-id="302fe-147">skip</span></span>|<span data-ttu-id="302fe-148">Int32</span><span class="sxs-lookup"><span data-stu-id="302fe-148">Int32</span></span>|<span data-ttu-id="302fe-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="302fe-149">Not yet documented</span></span>|
|<span data-ttu-id="302fe-150">top</span><span class="sxs-lookup"><span data-stu-id="302fe-150">top</span></span>|<span data-ttu-id="302fe-151">Int32</span><span class="sxs-lookup"><span data-stu-id="302fe-151">Int32</span></span>|<span data-ttu-id="302fe-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="302fe-152">Not yet documented</span></span>|
|<span data-ttu-id="302fe-153">sessionId</span><span class="sxs-lookup"><span data-stu-id="302fe-153">sessionId</span></span>|<span data-ttu-id="302fe-154">String</span><span class="sxs-lookup"><span data-stu-id="302fe-154">String</span></span>|<span data-ttu-id="302fe-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="302fe-155">Not yet documented</span></span>|
|<span data-ttu-id="302fe-156">filter</span><span class="sxs-lookup"><span data-stu-id="302fe-156">filter</span></span>|<span data-ttu-id="302fe-157">String</span><span class="sxs-lookup"><span data-stu-id="302fe-157">String</span></span>|<span data-ttu-id="302fe-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="302fe-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="302fe-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="302fe-159">Response</span></span>
<span data-ttu-id="302fe-160">В случае успешного действия это действие возвращает код `200 OK` отклика и поток в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="302fe-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="302fe-161">Пример</span><span class="sxs-lookup"><span data-stu-id="302fe-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="302fe-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="302fe-162">Request</span></span>
<span data-ttu-id="302fe-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="302fe-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/reports/getConfigurationPolicyNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="302fe-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="302fe-164">Response</span></span>
<span data-ttu-id="302fe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="302fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 115

{
  "value": "Z2V0Q29uZmlndXJhdGlvblBvbGljeU5vbkNvbXBsaWFuY2VSZXBvcnQgSW50dW5lIERvYyBTYW1wbGUgLTE2MTk2MDUzMTI="
}
```




