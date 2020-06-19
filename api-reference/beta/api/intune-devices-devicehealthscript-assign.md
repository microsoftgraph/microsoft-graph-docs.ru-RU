---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd35d0edabdd0f20e5a3c567858159fdf5dd8de6
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792424"
---
# <a name="assign-action"></a><span data-ttu-id="f7d4e-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="f7d4e-103">assign action</span></span>

<span data-ttu-id="f7d4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7d4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7d4e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7d4e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7d4e-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7d4e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f7d4e-108">Prerequisites</span></span>
<span data-ttu-id="f7d4e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f7d4e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7d4e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7d4e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7d4e-111">Permission type</span></span>|<span data-ttu-id="f7d4e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7d4e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7d4e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7d4e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7d4e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7d4e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f7d4e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7d4e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7d4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-116">Not supported.</span></span>|
|<span data-ttu-id="f7d4e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7d4e-117">Application</span></span>|<span data-ttu-id="f7d4e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7d4e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7d4e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7d4e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="f7d4e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f7d4e-120">Request headers</span></span>
|<span data-ttu-id="f7d4e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7d4e-121">Header</span></span>|<span data-ttu-id="f7d4e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7d4e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7d4e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7d4e-123">Authorization</span></span>|<span data-ttu-id="f7d4e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7d4e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7d4e-125">Accept</span></span>|<span data-ttu-id="f7d4e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7d4e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7d4e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7d4e-127">Request body</span></span>
<span data-ttu-id="f7d4e-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f7d4e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f7d4e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7d4e-130">Property</span></span>|<span data-ttu-id="f7d4e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f7d4e-131">Type</span></span>|<span data-ttu-id="f7d4e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f7d4e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7d4e-133">девицехеалсскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="f7d4e-133">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="f7d4e-134">Коллекция [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f7d4e-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="f7d4e-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f7d4e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f7d4e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7d4e-136">Response</span></span>
<span data-ttu-id="f7d4e-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f7d4e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f7d4e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7d4e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7d4e-139">Request</span></span>
<span data-ttu-id="f7d4e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assign

Content-type: application/json
Content-length: 688

{
  "deviceHealthScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "runRemediationScript": true,
      "runSchedule": {
        "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
        "interval": 8,
        "useUtc": true,
        "time": "11:58:36.2550000"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f7d4e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7d4e-141">Response</span></span>
<span data-ttu-id="f7d4e-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-142">Here is an example of the response.</span></span> <span data-ttu-id="f7d4e-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f7d4e-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f7d4e-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



