---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac1a767008da94d59f9f53a29a1ca7cee7e93f94
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792340"
---
# <a name="assign-action"></a><span data-ttu-id="14e46-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="14e46-103">assign action</span></span>

<span data-ttu-id="14e46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14e46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14e46-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14e46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14e46-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14e46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14e46-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="14e46-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14e46-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="14e46-108">Prerequisites</span></span>
<span data-ttu-id="14e46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14e46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14e46-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14e46-111">Permission type</span></span>|<span data-ttu-id="14e46-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14e46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14e46-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14e46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14e46-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e46-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="14e46-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14e46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14e46-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14e46-116">Not supported.</span></span>|
|<span data-ttu-id="14e46-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14e46-117">Application</span></span>|<span data-ttu-id="14e46-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e46-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14e46-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14e46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="14e46-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="14e46-120">Request headers</span></span>
|<span data-ttu-id="14e46-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14e46-121">Header</span></span>|<span data-ttu-id="14e46-122">Значение</span><span class="sxs-lookup"><span data-stu-id="14e46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14e46-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14e46-123">Authorization</span></span>|<span data-ttu-id="14e46-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14e46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14e46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14e46-125">Accept</span></span>|<span data-ttu-id="14e46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14e46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14e46-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14e46-127">Request body</span></span>
<span data-ttu-id="14e46-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14e46-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="14e46-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="14e46-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="14e46-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="14e46-130">Property</span></span>|<span data-ttu-id="14e46-131">Тип</span><span class="sxs-lookup"><span data-stu-id="14e46-131">Type</span></span>|<span data-ttu-id="14e46-132">Описание</span><span class="sxs-lookup"><span data-stu-id="14e46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14e46-133">девицеманажементскриптграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="14e46-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="14e46-134">Коллекция [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="14e46-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="14e46-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="14e46-135">Not yet documented</span></span>|
|<span data-ttu-id="14e46-136">девицеманажементскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="14e46-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="14e46-137">Коллекция [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="14e46-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="14e46-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="14e46-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="14e46-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="14e46-139">Response</span></span>
<span data-ttu-id="14e46-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="14e46-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="14e46-141">Пример</span><span class="sxs-lookup"><span data-stu-id="14e46-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="14e46-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="14e46-142">Request</span></span>
<span data-ttu-id="14e46-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14e46-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assign

Content-type: application/json
Content-length: 713

{
  "deviceManagementScriptGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
      "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
      "targetGroupId": "Target Group Id value"
    }
  ],
  "deviceManagementScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="14e46-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="14e46-144">Response</span></span>
<span data-ttu-id="14e46-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14e46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



