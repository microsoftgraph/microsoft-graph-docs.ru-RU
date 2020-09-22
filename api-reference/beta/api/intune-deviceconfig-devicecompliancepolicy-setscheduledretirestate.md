---
title: действие Сетсчедуледретирестате
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9601931d99e1ab5963971b24304e953c0f0798c3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072678"
---
# <a name="setscheduledretirestate-action"></a><span data-ttu-id="eac6b-103">действие Сетсчедуледретирестате</span><span class="sxs-lookup"><span data-stu-id="eac6b-103">setScheduledRetireState action</span></span>

<span data-ttu-id="eac6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eac6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eac6b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eac6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eac6b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eac6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eac6b-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eac6b-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eac6b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eac6b-108">Prerequisites</span></span>
<span data-ttu-id="eac6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eac6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eac6b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eac6b-111">Permission type</span></span>|<span data-ttu-id="eac6b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eac6b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eac6b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eac6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eac6b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eac6b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eac6b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eac6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eac6b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eac6b-116">Not supported.</span></span>|
|<span data-ttu-id="eac6b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eac6b-117">Application</span></span>|<span data-ttu-id="eac6b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eac6b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eac6b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eac6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/setScheduledRetireState
```

## <a name="request-headers"></a><span data-ttu-id="eac6b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eac6b-120">Request headers</span></span>
|<span data-ttu-id="eac6b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eac6b-121">Header</span></span>|<span data-ttu-id="eac6b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eac6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eac6b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eac6b-123">Authorization</span></span>|<span data-ttu-id="eac6b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eac6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eac6b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eac6b-125">Accept</span></span>|<span data-ttu-id="eac6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eac6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eac6b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eac6b-127">Request body</span></span>
<span data-ttu-id="eac6b-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eac6b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="eac6b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="eac6b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="eac6b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eac6b-130">Property</span></span>|<span data-ttu-id="eac6b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eac6b-131">Type</span></span>|<span data-ttu-id="eac6b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eac6b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eac6b-133">state</span><span class="sxs-lookup"><span data-stu-id="eac6b-133">state</span></span>|[<span data-ttu-id="eac6b-134">scheduledRetireState</span><span class="sxs-lookup"><span data-stu-id="eac6b-134">scheduledRetireState</span></span>](../resources/intune-deviceconfig-scheduledretirestate.md)|<span data-ttu-id="eac6b-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eac6b-135">Not yet documented</span></span>|
|<span data-ttu-id="eac6b-136">манажеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="eac6b-136">managedDeviceIds</span></span>|<span data-ttu-id="eac6b-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="eac6b-137">String collection</span></span>|<span data-ttu-id="eac6b-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="eac6b-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="eac6b-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="eac6b-139">Response</span></span>
<span data-ttu-id="eac6b-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eac6b-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eac6b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="eac6b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="eac6b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="eac6b-142">Request</span></span>
<span data-ttu-id="eac6b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eac6b-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eac6b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="eac6b-144">Response</span></span>
<span data-ttu-id="eac6b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eac6b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






