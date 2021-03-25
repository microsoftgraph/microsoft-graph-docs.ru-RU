---
title: setScheduledRetireState action
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8e84d14c0161acc19966dba828b55828550e91b7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155542"
---
# <a name="setscheduledretirestate-action"></a><span data-ttu-id="fccbf-103">setScheduledRetireState action</span><span class="sxs-lookup"><span data-stu-id="fccbf-103">setScheduledRetireState action</span></span>

<span data-ttu-id="fccbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fccbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fccbf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fccbf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fccbf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fccbf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fccbf-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fccbf-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fccbf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fccbf-108">Prerequisites</span></span>
<span data-ttu-id="fccbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fccbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fccbf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fccbf-111">Permission type</span></span>|<span data-ttu-id="fccbf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fccbf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fccbf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fccbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fccbf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fccbf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fccbf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fccbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fccbf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fccbf-116">Not supported.</span></span>|
|<span data-ttu-id="fccbf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fccbf-117">Application</span></span>|<span data-ttu-id="fccbf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fccbf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fccbf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fccbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/setScheduledRetireState
```

## <a name="request-headers"></a><span data-ttu-id="fccbf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fccbf-120">Request headers</span></span>
|<span data-ttu-id="fccbf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fccbf-121">Header</span></span>|<span data-ttu-id="fccbf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fccbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fccbf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fccbf-123">Authorization</span></span>|<span data-ttu-id="fccbf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fccbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fccbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fccbf-125">Accept</span></span>|<span data-ttu-id="fccbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fccbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fccbf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fccbf-127">Request body</span></span>
<span data-ttu-id="fccbf-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fccbf-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fccbf-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="fccbf-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fccbf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fccbf-130">Property</span></span>|<span data-ttu-id="fccbf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fccbf-131">Type</span></span>|<span data-ttu-id="fccbf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fccbf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fccbf-133">state</span><span class="sxs-lookup"><span data-stu-id="fccbf-133">state</span></span>|[<span data-ttu-id="fccbf-134">scheduledRetireState</span><span class="sxs-lookup"><span data-stu-id="fccbf-134">scheduledRetireState</span></span>](../resources/intune-deviceconfig-scheduledretirestate.md)|<span data-ttu-id="fccbf-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fccbf-135">Not yet documented</span></span>|
|<span data-ttu-id="fccbf-136">managedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="fccbf-136">managedDeviceIds</span></span>|<span data-ttu-id="fccbf-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fccbf-137">String collection</span></span>|<span data-ttu-id="fccbf-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fccbf-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fccbf-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="fccbf-139">Response</span></span>
<span data-ttu-id="fccbf-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fccbf-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fccbf-141">Пример</span><span class="sxs-lookup"><span data-stu-id="fccbf-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="fccbf-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="fccbf-142">Request</span></span>
<span data-ttu-id="fccbf-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fccbf-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/setScheduledRetireState

Content-type: application/json
Content-length: 95

{
  "state": "comfirmRetire",
  "managedDeviceIds": [
    "Managed Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="fccbf-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fccbf-144">Response</span></span>
<span data-ttu-id="fccbf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fccbf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




