---
title: getSettingNonComplianceReport action
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 708165851cfd3021ad62b0a5c560245adc4c0284
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758633"
---
# <a name="getsettingnoncompliancereport-action"></a><span data-ttu-id="98422-103">getSettingNonComplianceReport action</span><span class="sxs-lookup"><span data-stu-id="98422-103">getSettingNonComplianceReport action</span></span>

<span data-ttu-id="98422-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98422-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98422-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98422-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98422-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="98422-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98422-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="98422-107">Prerequisites</span></span>
<span data-ttu-id="98422-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98422-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98422-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98422-110">Permission type</span></span>|<span data-ttu-id="98422-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98422-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98422-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98422-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98422-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98422-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="98422-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98422-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98422-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98422-115">Not supported.</span></span>|
|<span data-ttu-id="98422-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="98422-116">Application</span></span>|<span data-ttu-id="98422-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98422-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98422-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98422-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getSettingNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="98422-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="98422-119">Request headers</span></span>
|<span data-ttu-id="98422-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98422-120">Header</span></span>|<span data-ttu-id="98422-121">Значение</span><span class="sxs-lookup"><span data-stu-id="98422-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98422-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="98422-122">Authorization</span></span>|<span data-ttu-id="98422-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98422-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98422-124">Accept</span><span class="sxs-lookup"><span data-stu-id="98422-124">Accept</span></span>|<span data-ttu-id="98422-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98422-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98422-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98422-126">Request body</span></span>
<span data-ttu-id="98422-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98422-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="98422-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="98422-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="98422-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="98422-129">Property</span></span>|<span data-ttu-id="98422-130">Тип</span><span class="sxs-lookup"><span data-stu-id="98422-130">Type</span></span>|<span data-ttu-id="98422-131">Описание</span><span class="sxs-lookup"><span data-stu-id="98422-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98422-132">name</span><span class="sxs-lookup"><span data-stu-id="98422-132">name</span></span>|<span data-ttu-id="98422-133">String</span><span class="sxs-lookup"><span data-stu-id="98422-133">String</span></span>|<span data-ttu-id="98422-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="98422-134">Not yet documented</span></span>|
|<span data-ttu-id="98422-135">select</span><span class="sxs-lookup"><span data-stu-id="98422-135">select</span></span>|<span data-ttu-id="98422-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="98422-136">String collection</span></span>|<span data-ttu-id="98422-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="98422-137">Not yet documented</span></span>|
|<span data-ttu-id="98422-138">search</span><span class="sxs-lookup"><span data-stu-id="98422-138">search</span></span>|<span data-ttu-id="98422-139">String</span><span class="sxs-lookup"><span data-stu-id="98422-139">String</span></span>|<span data-ttu-id="98422-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="98422-140">Not yet documented</span></span>|
|<span data-ttu-id="98422-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="98422-141">groupBy</span></span>|<span data-ttu-id="98422-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="98422-142">String collection</span></span>|<span data-ttu-id="98422-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="98422-143">Not yet documented</span></span>|
|<span data-ttu-id="98422-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="98422-144">orderBy</span></span>|<span data-ttu-id="98422-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="98422-145">String collection</span></span>|<span data-ttu-id="98422-146">Н/Д</span><span class="sxs-lookup"><span data-stu-id="98422-146">Not yet documented</span></span>|
|<span data-ttu-id="98422-147">skip</span><span class="sxs-lookup"><span data-stu-id="98422-147">skip</span></span>|<span data-ttu-id="98422-148">Int32</span><span class="sxs-lookup"><span data-stu-id="98422-148">Int32</span></span>|<span data-ttu-id="98422-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="98422-149">Not yet documented</span></span>|
|<span data-ttu-id="98422-150">top</span><span class="sxs-lookup"><span data-stu-id="98422-150">top</span></span>|<span data-ttu-id="98422-151">Int32</span><span class="sxs-lookup"><span data-stu-id="98422-151">Int32</span></span>|<span data-ttu-id="98422-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="98422-152">Not yet documented</span></span>|
|<span data-ttu-id="98422-153">sessionId</span><span class="sxs-lookup"><span data-stu-id="98422-153">sessionId</span></span>|<span data-ttu-id="98422-154">String</span><span class="sxs-lookup"><span data-stu-id="98422-154">String</span></span>|<span data-ttu-id="98422-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="98422-155">Not yet documented</span></span>|
|<span data-ttu-id="98422-156">filter</span><span class="sxs-lookup"><span data-stu-id="98422-156">filter</span></span>|<span data-ttu-id="98422-157">String</span><span class="sxs-lookup"><span data-stu-id="98422-157">String</span></span>|<span data-ttu-id="98422-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="98422-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="98422-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="98422-159">Response</span></span>
<span data-ttu-id="98422-160">В случае успешного действия это действие возвращает код `200 OK` отклика и поток в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="98422-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98422-161">Пример</span><span class="sxs-lookup"><span data-stu-id="98422-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="98422-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="98422-162">Request</span></span>
<span data-ttu-id="98422-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98422-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/reports/getSettingNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="98422-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="98422-164">Response</span></span>
<span data-ttu-id="98422-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98422-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 99

{
  "value": "Z2V0U2V0dGluZ05vbkNvbXBsaWFuY2VSZXBvcnQgSW50dW5lIERvYyBTYW1wbGUgMTEwMDk1MTE2MA=="
}
```




