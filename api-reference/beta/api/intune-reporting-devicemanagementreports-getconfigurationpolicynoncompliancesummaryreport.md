---
title: Действие getConfigurationPolicyNonComplianceSummaryReport
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 81c1ea400c58608654a6e8b118865bb7ae23944d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160676"
---
# <a name="getconfigurationpolicynoncompliancesummaryreport-action"></a><span data-ttu-id="e9d6c-103">Действие getConfigurationPolicyNonComplianceSummaryReport</span><span class="sxs-lookup"><span data-stu-id="e9d6c-103">getConfigurationPolicyNonComplianceSummaryReport action</span></span>

<span data-ttu-id="e9d6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9d6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9d6c-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9d6c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9d6c-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9d6c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e9d6c-108">Prerequisites</span></span>
<span data-ttu-id="e9d6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9d6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9d6c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9d6c-111">Permission type</span></span>|<span data-ttu-id="e9d6c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9d6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9d6c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9d6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9d6c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d6c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e9d6c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9d6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9d6c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-116">Not supported.</span></span>|
|<span data-ttu-id="e9d6c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9d6c-117">Application</span></span>|<span data-ttu-id="e9d6c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d6c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9d6c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9d6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getConfigurationPolicyNonComplianceSummaryReport
```

## <a name="request-headers"></a><span data-ttu-id="e9d6c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e9d6c-120">Request headers</span></span>
|<span data-ttu-id="e9d6c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9d6c-121">Header</span></span>|<span data-ttu-id="e9d6c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9d6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9d6c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9d6c-123">Authorization</span></span>|<span data-ttu-id="e9d6c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9d6c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9d6c-125">Accept</span></span>|<span data-ttu-id="e9d6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9d6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9d6c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9d6c-127">Request body</span></span>
<span data-ttu-id="e9d6c-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e9d6c-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e9d6c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9d6c-130">Property</span></span>|<span data-ttu-id="e9d6c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e9d6c-131">Type</span></span>|<span data-ttu-id="e9d6c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e9d6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9d6c-133">name</span><span class="sxs-lookup"><span data-stu-id="e9d6c-133">name</span></span>|<span data-ttu-id="e9d6c-134">String</span><span class="sxs-lookup"><span data-stu-id="e9d6c-134">String</span></span>|<span data-ttu-id="e9d6c-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-135">Not yet documented</span></span>|
|<span data-ttu-id="e9d6c-136">select</span><span class="sxs-lookup"><span data-stu-id="e9d6c-136">select</span></span>|<span data-ttu-id="e9d6c-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e9d6c-137">String collection</span></span>|<span data-ttu-id="e9d6c-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e9d6c-138">Not yet documented</span></span>|
|<span data-ttu-id="e9d6c-139">search</span><span class="sxs-lookup"><span data-stu-id="e9d6c-139">search</span></span>|<span data-ttu-id="e9d6c-140">String</span><span class="sxs-lookup"><span data-stu-id="e9d6c-140">String</span></span>|<span data-ttu-id="e9d6c-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-141">Not yet documented</span></span>|
|<span data-ttu-id="e9d6c-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="e9d6c-142">groupBy</span></span>|<span data-ttu-id="e9d6c-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e9d6c-143">String collection</span></span>|<span data-ttu-id="e9d6c-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e9d6c-144">Not yet documented</span></span>|
|<span data-ttu-id="e9d6c-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="e9d6c-145">orderBy</span></span>|<span data-ttu-id="e9d6c-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e9d6c-146">String collection</span></span>|<span data-ttu-id="e9d6c-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e9d6c-147">Not yet documented</span></span>|
|<span data-ttu-id="e9d6c-148">skip</span><span class="sxs-lookup"><span data-stu-id="e9d6c-148">skip</span></span>|<span data-ttu-id="e9d6c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e9d6c-149">Int32</span></span>|<span data-ttu-id="e9d6c-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-150">Not yet documented</span></span>|
|<span data-ttu-id="e9d6c-151">top</span><span class="sxs-lookup"><span data-stu-id="e9d6c-151">top</span></span>|<span data-ttu-id="e9d6c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e9d6c-152">Int32</span></span>|<span data-ttu-id="e9d6c-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-153">Not yet documented</span></span>|
|<span data-ttu-id="e9d6c-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="e9d6c-154">sessionId</span></span>|<span data-ttu-id="e9d6c-155">String</span><span class="sxs-lookup"><span data-stu-id="e9d6c-155">String</span></span>|<span data-ttu-id="e9d6c-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-156">Not yet documented</span></span>|
|<span data-ttu-id="e9d6c-157">filter</span><span class="sxs-lookup"><span data-stu-id="e9d6c-157">filter</span></span>|<span data-ttu-id="e9d6c-158">String</span><span class="sxs-lookup"><span data-stu-id="e9d6c-158">String</span></span>|<span data-ttu-id="e9d6c-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e9d6c-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9d6c-160">Response</span></span>
<span data-ttu-id="e9d6c-161">В случае успеха это действие возвращает код `200 OK` отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9d6c-162">Пример</span><span class="sxs-lookup"><span data-stu-id="e9d6c-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9d6c-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9d6c-163">Request</span></span>
<span data-ttu-id="e9d6c-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getConfigurationPolicyNonComplianceSummaryReport

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

### <a name="response"></a><span data-ttu-id="e9d6c-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9d6c-165">Response</span></span>
<span data-ttu-id="e9d6c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9d6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": "Z2V0Q29uZmlndXJhdGlvblBvbGljeU5vbkNvbXBsaWFuY2VTdW1tYXJ5UmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIC0xNjM2NzI4OTg4"
}
```




