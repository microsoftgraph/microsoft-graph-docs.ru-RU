---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe1a1dee7be8b33f95479b544009dd6faed514e2
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085992"
---
# <a name="assign-action"></a><span data-ttu-id="9d8bb-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="9d8bb-103">assign action</span></span>

> <span data-ttu-id="9d8bb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d8bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d8bb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d8bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d8bb-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9d8bb-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d8bb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9d8bb-107">Prerequisites</span></span>
<span data-ttu-id="9d8bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d8bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d8bb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d8bb-110">Permission type</span></span>|<span data-ttu-id="9d8bb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d8bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d8bb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d8bb-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9d8bb-113">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="9d8bb-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9d8bb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8bb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9d8bb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d8bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d8bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d8bb-116">Not supported.</span></span>|
|<span data-ttu-id="9d8bb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d8bb-117">Application</span></span>||
| <span data-ttu-id="9d8bb-118">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="9d8bb-118">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9d8bb-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8bb-119">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d8bb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d8bb-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="9d8bb-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9d8bb-121">Request headers</span></span>
|<span data-ttu-id="9d8bb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d8bb-122">Header</span></span>|<span data-ttu-id="9d8bb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9d8bb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d8bb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d8bb-124">Authorization</span></span>|<span data-ttu-id="9d8bb-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d8bb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d8bb-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9d8bb-126">Accept</span></span>|<span data-ttu-id="9d8bb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9d8bb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d8bb-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d8bb-128">Request body</span></span>
<span data-ttu-id="9d8bb-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d8bb-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9d8bb-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9d8bb-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9d8bb-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d8bb-131">Property</span></span>|<span data-ttu-id="9d8bb-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9d8bb-132">Type</span></span>|<span data-ttu-id="9d8bb-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9d8bb-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d8bb-134">девицеманажементскриптграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="9d8bb-134">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="9d8bb-135">Коллекция [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9d8bb-135">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="9d8bb-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9d8bb-136">Not yet documented</span></span>|
|<span data-ttu-id="9d8bb-137">девицеманажементскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="9d8bb-137">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="9d8bb-138">Коллекция [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9d8bb-138">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="9d8bb-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9d8bb-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9d8bb-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d8bb-140">Response</span></span>
<span data-ttu-id="9d8bb-141">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9d8bb-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9d8bb-142">Пример</span><span class="sxs-lookup"><span data-stu-id="9d8bb-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d8bb-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d8bb-143">Request</span></span>
<span data-ttu-id="9d8bb-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d8bb-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign

Content-type: application/json
Content-length: 550

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
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9d8bb-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d8bb-145">Response</span></span>
<span data-ttu-id="9d8bb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d8bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









