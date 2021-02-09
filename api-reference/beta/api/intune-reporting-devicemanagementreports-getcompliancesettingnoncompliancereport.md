---
title: Действие getComplianceSettingNonComplianceReport
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f0412c297209e004a99cb43af02955a0f43848fd
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160940"
---
# <a name="getcompliancesettingnoncompliancereport-action"></a><span data-ttu-id="e234f-103">Действие getComplianceSettingNonComplianceReport</span><span class="sxs-lookup"><span data-stu-id="e234f-103">getComplianceSettingNonComplianceReport action</span></span>

<span data-ttu-id="e234f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e234f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e234f-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e234f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e234f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e234f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e234f-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e234f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e234f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e234f-108">Prerequisites</span></span>
<span data-ttu-id="e234f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e234f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e234f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e234f-111">Permission type</span></span>|<span data-ttu-id="e234f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e234f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e234f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e234f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e234f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e234f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e234f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e234f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e234f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e234f-116">Not supported.</span></span>|
|<span data-ttu-id="e234f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e234f-117">Application</span></span>|<span data-ttu-id="e234f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e234f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e234f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e234f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getComplianceSettingNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="e234f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e234f-120">Request headers</span></span>
|<span data-ttu-id="e234f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e234f-121">Header</span></span>|<span data-ttu-id="e234f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e234f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e234f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e234f-123">Authorization</span></span>|<span data-ttu-id="e234f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e234f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e234f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e234f-125">Accept</span></span>|<span data-ttu-id="e234f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e234f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e234f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e234f-127">Request body</span></span>
<span data-ttu-id="e234f-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e234f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e234f-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e234f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e234f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e234f-130">Property</span></span>|<span data-ttu-id="e234f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e234f-131">Type</span></span>|<span data-ttu-id="e234f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e234f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e234f-133">name</span><span class="sxs-lookup"><span data-stu-id="e234f-133">name</span></span>|<span data-ttu-id="e234f-134">String</span><span class="sxs-lookup"><span data-stu-id="e234f-134">String</span></span>|<span data-ttu-id="e234f-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e234f-135">Not yet documented</span></span>|
|<span data-ttu-id="e234f-136">select</span><span class="sxs-lookup"><span data-stu-id="e234f-136">select</span></span>|<span data-ttu-id="e234f-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e234f-137">String collection</span></span>|<span data-ttu-id="e234f-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e234f-138">Not yet documented</span></span>|
|<span data-ttu-id="e234f-139">search</span><span class="sxs-lookup"><span data-stu-id="e234f-139">search</span></span>|<span data-ttu-id="e234f-140">String</span><span class="sxs-lookup"><span data-stu-id="e234f-140">String</span></span>|<span data-ttu-id="e234f-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e234f-141">Not yet documented</span></span>|
|<span data-ttu-id="e234f-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="e234f-142">groupBy</span></span>|<span data-ttu-id="e234f-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e234f-143">String collection</span></span>|<span data-ttu-id="e234f-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e234f-144">Not yet documented</span></span>|
|<span data-ttu-id="e234f-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="e234f-145">orderBy</span></span>|<span data-ttu-id="e234f-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e234f-146">String collection</span></span>|<span data-ttu-id="e234f-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e234f-147">Not yet documented</span></span>|
|<span data-ttu-id="e234f-148">skip</span><span class="sxs-lookup"><span data-stu-id="e234f-148">skip</span></span>|<span data-ttu-id="e234f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e234f-149">Int32</span></span>|<span data-ttu-id="e234f-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e234f-150">Not yet documented</span></span>|
|<span data-ttu-id="e234f-151">top</span><span class="sxs-lookup"><span data-stu-id="e234f-151">top</span></span>|<span data-ttu-id="e234f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e234f-152">Int32</span></span>|<span data-ttu-id="e234f-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e234f-153">Not yet documented</span></span>|
|<span data-ttu-id="e234f-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="e234f-154">sessionId</span></span>|<span data-ttu-id="e234f-155">String</span><span class="sxs-lookup"><span data-stu-id="e234f-155">String</span></span>|<span data-ttu-id="e234f-156">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e234f-156">Not yet documented</span></span>|
|<span data-ttu-id="e234f-157">filter</span><span class="sxs-lookup"><span data-stu-id="e234f-157">filter</span></span>|<span data-ttu-id="e234f-158">String</span><span class="sxs-lookup"><span data-stu-id="e234f-158">String</span></span>|<span data-ttu-id="e234f-159">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e234f-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e234f-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="e234f-160">Response</span></span>
<span data-ttu-id="e234f-161">В случае успеха это действие возвращает код `200 OK` отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e234f-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e234f-162">Пример</span><span class="sxs-lookup"><span data-stu-id="e234f-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="e234f-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="e234f-163">Request</span></span>
<span data-ttu-id="e234f-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e234f-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getComplianceSettingNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="e234f-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="e234f-165">Response</span></span>
<span data-ttu-id="e234f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e234f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 111

{
  "value": "Z2V0Q29tcGxpYW5jZVNldHRpbmdOb25Db21wbGlhbmNlUmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDU0NDgzMTA0NQ=="
}
```




