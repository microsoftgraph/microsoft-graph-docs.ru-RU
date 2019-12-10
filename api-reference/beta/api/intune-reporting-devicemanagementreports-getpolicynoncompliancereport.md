---
title: действие Жетполицинонкомплианцерепорт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0411d991fad42df1547c35f54c6d0f8dbc98dd35
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940280"
---
# <a name="getpolicynoncompliancereport-action"></a><span data-ttu-id="ea4ed-103">действие Жетполицинонкомплианцерепорт</span><span class="sxs-lookup"><span data-stu-id="ea4ed-103">getPolicyNonComplianceReport action</span></span>

> <span data-ttu-id="ea4ed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea4ed-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea4ed-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea4ed-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ea4ed-107">Prerequisites</span></span>
<span data-ttu-id="ea4ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea4ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea4ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea4ed-110">Permission type</span></span>|<span data-ttu-id="ea4ed-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea4ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea4ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea4ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea4ed-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ea4ed-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ea4ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea4ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea4ed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-115">Not supported.</span></span>|
|<span data-ttu-id="ea4ed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea4ed-116">Application</span></span>|<span data-ttu-id="ea4ed-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ea4ed-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea4ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea4ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="ea4ed-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ea4ed-119">Request headers</span></span>
|<span data-ttu-id="ea4ed-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea4ed-120">Header</span></span>|<span data-ttu-id="ea4ed-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ea4ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea4ed-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea4ed-122">Authorization</span></span>|<span data-ttu-id="ea4ed-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea4ed-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ea4ed-124">Accept</span></span>|<span data-ttu-id="ea4ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea4ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea4ed-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea4ed-126">Request body</span></span>
<span data-ttu-id="ea4ed-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ea4ed-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ea4ed-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea4ed-129">Property</span></span>|<span data-ttu-id="ea4ed-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ea4ed-130">Type</span></span>|<span data-ttu-id="ea4ed-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ea4ed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea4ed-132">name</span><span class="sxs-lookup"><span data-stu-id="ea4ed-132">name</span></span>|<span data-ttu-id="ea4ed-133">String</span><span class="sxs-lookup"><span data-stu-id="ea4ed-133">String</span></span>|<span data-ttu-id="ea4ed-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-134">Not yet documented</span></span>|
|<span data-ttu-id="ea4ed-135">select</span><span class="sxs-lookup"><span data-stu-id="ea4ed-135">select</span></span>|<span data-ttu-id="ea4ed-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ea4ed-136">String collection</span></span>|<span data-ttu-id="ea4ed-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ea4ed-137">Not yet documented</span></span>|
|<span data-ttu-id="ea4ed-138">search</span><span class="sxs-lookup"><span data-stu-id="ea4ed-138">search</span></span>|<span data-ttu-id="ea4ed-139">String</span><span class="sxs-lookup"><span data-stu-id="ea4ed-139">String</span></span>|<span data-ttu-id="ea4ed-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-140">Not yet documented</span></span>|
|<span data-ttu-id="ea4ed-141">Оператора</span><span class="sxs-lookup"><span data-stu-id="ea4ed-141">groupBy</span></span>|<span data-ttu-id="ea4ed-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ea4ed-142">String collection</span></span>|<span data-ttu-id="ea4ed-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ea4ed-143">Not yet documented</span></span>|
|<span data-ttu-id="ea4ed-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="ea4ed-144">orderBy</span></span>|<span data-ttu-id="ea4ed-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ea4ed-145">String collection</span></span>|<span data-ttu-id="ea4ed-146">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ea4ed-146">Not yet documented</span></span>|
|<span data-ttu-id="ea4ed-147">skip</span><span class="sxs-lookup"><span data-stu-id="ea4ed-147">skip</span></span>|<span data-ttu-id="ea4ed-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ea4ed-148">Int32</span></span>|<span data-ttu-id="ea4ed-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-149">Not yet documented</span></span>|
|<span data-ttu-id="ea4ed-150">top</span><span class="sxs-lookup"><span data-stu-id="ea4ed-150">top</span></span>|<span data-ttu-id="ea4ed-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ea4ed-151">Int32</span></span>|<span data-ttu-id="ea4ed-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-152">Not yet documented</span></span>|
|<span data-ttu-id="ea4ed-153">sessionId</span><span class="sxs-lookup"><span data-stu-id="ea4ed-153">sessionId</span></span>|<span data-ttu-id="ea4ed-154">String</span><span class="sxs-lookup"><span data-stu-id="ea4ed-154">String</span></span>|<span data-ttu-id="ea4ed-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-155">Not yet documented</span></span>|
|<span data-ttu-id="ea4ed-156">filter</span><span class="sxs-lookup"><span data-stu-id="ea4ed-156">filter</span></span>|<span data-ttu-id="ea4ed-157">String</span><span class="sxs-lookup"><span data-stu-id="ea4ed-157">String</span></span>|<span data-ttu-id="ea4ed-158">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ea4ed-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ea4ed-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea4ed-159">Response</span></span>
<span data-ttu-id="ea4ed-160">При успешном выполнении это действие возвращает `200 OK` код отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea4ed-161">Пример</span><span class="sxs-lookup"><span data-stu-id="ea4ed-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea4ed-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea4ed-162">Request</span></span>
<span data-ttu-id="ea4ed-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getPolicyNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="ea4ed-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea4ed-164">Response</span></span>
<span data-ttu-id="ea4ed-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```





