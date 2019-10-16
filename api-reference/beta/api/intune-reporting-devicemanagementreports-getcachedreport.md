---
title: действие Жеткачедрепорт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d64fba30bf2eed48fe14a203c85e0ceab977c4a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537249"
---
# <a name="getcachedreport-action"></a><span data-ttu-id="ab4e1-103">действие Жеткачедрепорт</span><span class="sxs-lookup"><span data-stu-id="ab4e1-103">getCachedReport action</span></span>

> <span data-ttu-id="ab4e1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab4e1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab4e1-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab4e1-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ab4e1-107">Prerequisites</span></span>
<span data-ttu-id="ab4e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab4e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab4e1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab4e1-110">Permission type</span></span>|<span data-ttu-id="ab4e1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab4e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab4e1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab4e1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab4e1-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ab4e1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ab4e1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab4e1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab4e1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-115">Not supported.</span></span>|
|<span data-ttu-id="ab4e1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ab4e1-116">Application</span></span>|<span data-ttu-id="ab4e1-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ab4e1-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab4e1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab4e1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCachedReport
```

## <a name="request-headers"></a><span data-ttu-id="ab4e1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab4e1-119">Request headers</span></span>
|<span data-ttu-id="ab4e1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab4e1-120">Header</span></span>|<span data-ttu-id="ab4e1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ab4e1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab4e1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab4e1-122">Authorization</span></span>|<span data-ttu-id="ab4e1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab4e1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ab4e1-124">Accept</span></span>|<span data-ttu-id="ab4e1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ab4e1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab4e1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab4e1-126">Request body</span></span>
<span data-ttu-id="ab4e1-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ab4e1-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ab4e1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab4e1-129">Property</span></span>|<span data-ttu-id="ab4e1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ab4e1-130">Type</span></span>|<span data-ttu-id="ab4e1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ab4e1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab4e1-132">id</span><span class="sxs-lookup"><span data-stu-id="ab4e1-132">id</span></span>|<span data-ttu-id="ab4e1-133">String</span><span class="sxs-lookup"><span data-stu-id="ab4e1-133">String</span></span>|<span data-ttu-id="ab4e1-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-134">Not yet documented</span></span>|
|<span data-ttu-id="ab4e1-135">select</span><span class="sxs-lookup"><span data-stu-id="ab4e1-135">select</span></span>|<span data-ttu-id="ab4e1-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ab4e1-136">String collection</span></span>|<span data-ttu-id="ab4e1-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ab4e1-137">Not yet documented</span></span>|
|<span data-ttu-id="ab4e1-138">search</span><span class="sxs-lookup"><span data-stu-id="ab4e1-138">search</span></span>|<span data-ttu-id="ab4e1-139">String</span><span class="sxs-lookup"><span data-stu-id="ab4e1-139">String</span></span>|<span data-ttu-id="ab4e1-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-140">Not yet documented</span></span>|
|<span data-ttu-id="ab4e1-141">Оператора</span><span class="sxs-lookup"><span data-stu-id="ab4e1-141">groupBy</span></span>|<span data-ttu-id="ab4e1-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ab4e1-142">String collection</span></span>|<span data-ttu-id="ab4e1-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ab4e1-143">Not yet documented</span></span>|
|<span data-ttu-id="ab4e1-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="ab4e1-144">orderBy</span></span>|<span data-ttu-id="ab4e1-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ab4e1-145">String collection</span></span>|<span data-ttu-id="ab4e1-146">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ab4e1-146">Not yet documented</span></span>|
|<span data-ttu-id="ab4e1-147">skip</span><span class="sxs-lookup"><span data-stu-id="ab4e1-147">skip</span></span>|<span data-ttu-id="ab4e1-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ab4e1-148">Int32</span></span>|<span data-ttu-id="ab4e1-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-149">Not yet documented</span></span>|
|<span data-ttu-id="ab4e1-150">top</span><span class="sxs-lookup"><span data-stu-id="ab4e1-150">top</span></span>|<span data-ttu-id="ab4e1-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ab4e1-151">Int32</span></span>|<span data-ttu-id="ab4e1-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ab4e1-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab4e1-153">Response</span></span>
<span data-ttu-id="ab4e1-154">При успешном выполнении это действие возвращает `200 OK` код отклика и поток в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-154">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab4e1-155">Пример</span><span class="sxs-lookup"><span data-stu-id="ab4e1-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab4e1-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab4e1-156">Request</span></span>
<span data-ttu-id="ab4e1-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getCachedReport

Content-type: application/json
Content-length: 209

{
  "id": "Id value",
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
  "top": 3
}
```

### <a name="response"></a><span data-ttu-id="ab4e1-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab4e1-158">Response</span></span>
<span data-ttu-id="ab4e1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab4e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```






