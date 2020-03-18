---
title: действие Жетполицинонкомплианцерепорт
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bce5c547d447aeb3d28d536d7e8dfb50bab912aa
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801371"
---
# <a name="getpolicynoncompliancereport-action"></a><span data-ttu-id="d6cde-103">действие Жетполицинонкомплианцерепорт</span><span class="sxs-lookup"><span data-stu-id="d6cde-103">getPolicyNonComplianceReport action</span></span>

> <span data-ttu-id="d6cde-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6cde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6cde-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6cde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6cde-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6cde-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6cde-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d6cde-107">Prerequisites</span></span>
<span data-ttu-id="d6cde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6cde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6cde-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6cde-110">Permission type</span></span>|<span data-ttu-id="d6cde-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6cde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6cde-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6cde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6cde-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="d6cde-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d6cde-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6cde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6cde-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6cde-115">Not supported.</span></span>|
|<span data-ttu-id="d6cde-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d6cde-116">Application</span></span>|<span data-ttu-id="d6cde-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="d6cde-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6cde-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6cde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="d6cde-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6cde-119">Request headers</span></span>
|<span data-ttu-id="d6cde-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6cde-120">Header</span></span>|<span data-ttu-id="d6cde-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d6cde-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6cde-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6cde-122">Authorization</span></span>|<span data-ttu-id="d6cde-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6cde-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6cde-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d6cde-124">Accept</span></span>|<span data-ttu-id="d6cde-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6cde-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6cde-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6cde-126">Request body</span></span>
<span data-ttu-id="d6cde-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6cde-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d6cde-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d6cde-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d6cde-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6cde-129">Property</span></span>|<span data-ttu-id="d6cde-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d6cde-130">Type</span></span>|<span data-ttu-id="d6cde-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d6cde-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6cde-132">name</span><span class="sxs-lookup"><span data-stu-id="d6cde-132">name</span></span>|<span data-ttu-id="d6cde-133">String</span><span class="sxs-lookup"><span data-stu-id="d6cde-133">String</span></span>|<span data-ttu-id="d6cde-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6cde-134">Not yet documented</span></span>|
|<span data-ttu-id="d6cde-135">select</span><span class="sxs-lookup"><span data-stu-id="d6cde-135">select</span></span>|<span data-ttu-id="d6cde-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6cde-136">String collection</span></span>|<span data-ttu-id="d6cde-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d6cde-137">Not yet documented</span></span>|
|<span data-ttu-id="d6cde-138">search</span><span class="sxs-lookup"><span data-stu-id="d6cde-138">search</span></span>|<span data-ttu-id="d6cde-139">String</span><span class="sxs-lookup"><span data-stu-id="d6cde-139">String</span></span>|<span data-ttu-id="d6cde-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6cde-140">Not yet documented</span></span>|
|<span data-ttu-id="d6cde-141">Оператора</span><span class="sxs-lookup"><span data-stu-id="d6cde-141">groupBy</span></span>|<span data-ttu-id="d6cde-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6cde-142">String collection</span></span>|<span data-ttu-id="d6cde-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d6cde-143">Not yet documented</span></span>|
|<span data-ttu-id="d6cde-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="d6cde-144">orderBy</span></span>|<span data-ttu-id="d6cde-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6cde-145">String collection</span></span>|<span data-ttu-id="d6cde-146">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d6cde-146">Not yet documented</span></span>|
|<span data-ttu-id="d6cde-147">skip</span><span class="sxs-lookup"><span data-stu-id="d6cde-147">skip</span></span>|<span data-ttu-id="d6cde-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d6cde-148">Int32</span></span>|<span data-ttu-id="d6cde-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6cde-149">Not yet documented</span></span>|
|<span data-ttu-id="d6cde-150">top</span><span class="sxs-lookup"><span data-stu-id="d6cde-150">top</span></span>|<span data-ttu-id="d6cde-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d6cde-151">Int32</span></span>|<span data-ttu-id="d6cde-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6cde-152">Not yet documented</span></span>|
|<span data-ttu-id="d6cde-153">sessionId</span><span class="sxs-lookup"><span data-stu-id="d6cde-153">sessionId</span></span>|<span data-ttu-id="d6cde-154">String</span><span class="sxs-lookup"><span data-stu-id="d6cde-154">String</span></span>|<span data-ttu-id="d6cde-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6cde-155">Not yet documented</span></span>|
|<span data-ttu-id="d6cde-156">filter</span><span class="sxs-lookup"><span data-stu-id="d6cde-156">filter</span></span>|<span data-ttu-id="d6cde-157">String</span><span class="sxs-lookup"><span data-stu-id="d6cde-157">String</span></span>|<span data-ttu-id="d6cde-158">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d6cde-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d6cde-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6cde-159">Response</span></span>
<span data-ttu-id="d6cde-160">При успешном выполнении это действие возвращает `200 OK` код отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6cde-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6cde-161">Пример</span><span class="sxs-lookup"><span data-stu-id="d6cde-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6cde-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6cde-162">Request</span></span>
<span data-ttu-id="d6cde-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6cde-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d6cde-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6cde-164">Response</span></span>
<span data-ttu-id="d6cde-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6cde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```




