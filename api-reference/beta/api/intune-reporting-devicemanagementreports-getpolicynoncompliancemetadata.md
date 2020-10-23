---
title: действие Жетполицинонкомплианцеметадата
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08ae61b37932672fde5ea682281899e1ddb393d9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698171"
---
# <a name="getpolicynoncompliancemetadata-action"></a><span data-ttu-id="50358-103">действие Жетполицинонкомплианцеметадата</span><span class="sxs-lookup"><span data-stu-id="50358-103">getPolicyNonComplianceMetadata action</span></span>

<span data-ttu-id="50358-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50358-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50358-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50358-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50358-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50358-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50358-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="50358-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50358-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="50358-108">Prerequisites</span></span>
<span data-ttu-id="50358-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50358-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50358-111">Permission type</span></span>|<span data-ttu-id="50358-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50358-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50358-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50358-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50358-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="50358-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="50358-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50358-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50358-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50358-116">Not supported.</span></span>|
|<span data-ttu-id="50358-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50358-117">Application</span></span>|<span data-ttu-id="50358-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="50358-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50358-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50358-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNonComplianceMetadata
```

## <a name="request-headers"></a><span data-ttu-id="50358-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50358-120">Request headers</span></span>
|<span data-ttu-id="50358-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50358-121">Header</span></span>|<span data-ttu-id="50358-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50358-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50358-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50358-123">Authorization</span></span>|<span data-ttu-id="50358-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50358-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50358-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50358-125">Accept</span></span>|<span data-ttu-id="50358-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50358-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50358-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50358-127">Request body</span></span>
<span data-ttu-id="50358-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50358-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="50358-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="50358-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="50358-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="50358-130">Property</span></span>|<span data-ttu-id="50358-131">Тип</span><span class="sxs-lookup"><span data-stu-id="50358-131">Type</span></span>|<span data-ttu-id="50358-132">Описание</span><span class="sxs-lookup"><span data-stu-id="50358-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50358-133">name</span><span class="sxs-lookup"><span data-stu-id="50358-133">name</span></span>|<span data-ttu-id="50358-134">String</span><span class="sxs-lookup"><span data-stu-id="50358-134">String</span></span>|<span data-ttu-id="50358-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="50358-135">Not yet documented</span></span>|
|<span data-ttu-id="50358-136">select</span><span class="sxs-lookup"><span data-stu-id="50358-136">select</span></span>|<span data-ttu-id="50358-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="50358-137">String collection</span></span>|<span data-ttu-id="50358-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="50358-138">Not yet documented</span></span>|
|<span data-ttu-id="50358-139">search</span><span class="sxs-lookup"><span data-stu-id="50358-139">search</span></span>|<span data-ttu-id="50358-140">String</span><span class="sxs-lookup"><span data-stu-id="50358-140">String</span></span>|<span data-ttu-id="50358-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="50358-141">Not yet documented</span></span>|
|<span data-ttu-id="50358-142">Оператора</span><span class="sxs-lookup"><span data-stu-id="50358-142">groupBy</span></span>|<span data-ttu-id="50358-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="50358-143">String collection</span></span>|<span data-ttu-id="50358-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="50358-144">Not yet documented</span></span>|
|<span data-ttu-id="50358-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="50358-145">orderBy</span></span>|<span data-ttu-id="50358-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="50358-146">String collection</span></span>|<span data-ttu-id="50358-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="50358-147">Not yet documented</span></span>|
|<span data-ttu-id="50358-148">skip</span><span class="sxs-lookup"><span data-stu-id="50358-148">skip</span></span>|<span data-ttu-id="50358-149">Int32</span><span class="sxs-lookup"><span data-stu-id="50358-149">Int32</span></span>|<span data-ttu-id="50358-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="50358-150">Not yet documented</span></span>|
|<span data-ttu-id="50358-151">top</span><span class="sxs-lookup"><span data-stu-id="50358-151">top</span></span>|<span data-ttu-id="50358-152">Int32</span><span class="sxs-lookup"><span data-stu-id="50358-152">Int32</span></span>|<span data-ttu-id="50358-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="50358-153">Not yet documented</span></span>|
|<span data-ttu-id="50358-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="50358-154">sessionId</span></span>|<span data-ttu-id="50358-155">String</span><span class="sxs-lookup"><span data-stu-id="50358-155">String</span></span>|<span data-ttu-id="50358-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="50358-156">Not yet documented</span></span>|
|<span data-ttu-id="50358-157">filter</span><span class="sxs-lookup"><span data-stu-id="50358-157">filter</span></span>|<span data-ttu-id="50358-158">String</span><span class="sxs-lookup"><span data-stu-id="50358-158">String</span></span>|<span data-ttu-id="50358-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="50358-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="50358-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="50358-160">Response</span></span>
<span data-ttu-id="50358-161">При успешном выполнении это действие возвращает `200 OK` код отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50358-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50358-162">Пример</span><span class="sxs-lookup"><span data-stu-id="50358-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="50358-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="50358-163">Request</span></span>
<span data-ttu-id="50358-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50358-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="50358-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="50358-165">Response</span></span>
<span data-ttu-id="50358-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50358-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 99

{
  "value": "Z2V0UG9saWN5Tm9uQ29tcGxpYW5jZU1ldGFkYXRhIEludHVuZSBEb2MgU2FtcGxlIC0xNzM5NTg5Nzc5"
}
```





