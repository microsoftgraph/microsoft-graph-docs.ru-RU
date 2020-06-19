---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 142fb4168d37184c30c0c3d5c7eeaa01cd9fa23f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791274"
---
# <a name="assign-action"></a><span data-ttu-id="cdcc4-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="cdcc4-103">assign action</span></span>

<span data-ttu-id="cdcc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdcc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdcc4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdcc4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdcc4-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdcc4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cdcc4-108">Prerequisites</span></span>
<span data-ttu-id="cdcc4-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cdcc4-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdcc4-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdcc4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdcc4-111">Permission type</span></span>|<span data-ttu-id="cdcc4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdcc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdcc4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdcc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdcc4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdcc4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cdcc4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdcc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdcc4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-116">Not supported.</span></span>|
|<span data-ttu-id="cdcc4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdcc4-117">Application</span></span>|<span data-ttu-id="cdcc4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdcc4-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdcc4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdcc4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assign
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy/assign
```

## <a name="request-headers"></a><span data-ttu-id="cdcc4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cdcc4-120">Request headers</span></span>
|<span data-ttu-id="cdcc4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdcc4-121">Header</span></span>|<span data-ttu-id="cdcc4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cdcc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdcc4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdcc4-123">Authorization</span></span>|<span data-ttu-id="cdcc4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdcc4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cdcc4-125">Accept</span></span>|<span data-ttu-id="cdcc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdcc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdcc4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cdcc4-127">Request body</span></span>
<span data-ttu-id="cdcc4-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cdcc4-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cdcc4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdcc4-130">Property</span></span>|<span data-ttu-id="cdcc4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cdcc4-131">Type</span></span>|<span data-ttu-id="cdcc4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cdcc4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdcc4-133">вдакполициассигнментс</span><span class="sxs-lookup"><span data-stu-id="cdcc4-133">wdacPolicyAssignments</span></span>|<span data-ttu-id="cdcc4-134">Коллекция [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cdcc4-134">[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) collection</span></span>|<span data-ttu-id="cdcc4-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cdcc4-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cdcc4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdcc4-136">Response</span></span>
<span data-ttu-id="cdcc4-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cdcc4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="cdcc4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdcc4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdcc4-139">Request</span></span>
<span data-ttu-id="cdcc4-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assign

Content-type: application/json
Content-length: 494

{
  "wdacPolicyAssignments": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
      "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="cdcc4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdcc4-141">Response</span></span>
<span data-ttu-id="cdcc4-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-142">Here is an example of the response.</span></span> <span data-ttu-id="cdcc4-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cdcc4-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



