---
title: Действие assign
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 084f1533cb2e4e2305b13341abc2f213b3940d7c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800993"
---
# <a name="assign-action"></a><span data-ttu-id="c05fd-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="c05fd-103">assign action</span></span>

> <span data-ttu-id="c05fd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c05fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c05fd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c05fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c05fd-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c05fd-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c05fd-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c05fd-107">Prerequisites</span></span>
<span data-ttu-id="c05fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c05fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c05fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c05fd-110">Permission type</span></span>|<span data-ttu-id="c05fd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c05fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c05fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c05fd-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c05fd-113">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c05fd-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c05fd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c05fd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c05fd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c05fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c05fd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c05fd-116">Not supported.</span></span>|
|<span data-ttu-id="c05fd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c05fd-117">Application</span></span>||
| <span data-ttu-id="c05fd-118">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c05fd-118">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c05fd-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c05fd-119">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c05fd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c05fd-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c05fd-121">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c05fd-121">Request headers</span></span>
|<span data-ttu-id="c05fd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c05fd-122">Header</span></span>|<span data-ttu-id="c05fd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c05fd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c05fd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c05fd-124">Authorization</span></span>|<span data-ttu-id="c05fd-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c05fd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c05fd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c05fd-126">Accept</span></span>|<span data-ttu-id="c05fd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c05fd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c05fd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c05fd-128">Request body</span></span>
<span data-ttu-id="c05fd-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c05fd-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c05fd-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c05fd-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c05fd-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="c05fd-131">Property</span></span>|<span data-ttu-id="c05fd-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c05fd-132">Type</span></span>|<span data-ttu-id="c05fd-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c05fd-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c05fd-134">девицеманажементскриптграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="c05fd-134">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="c05fd-135">Коллекция [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c05fd-135">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="c05fd-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c05fd-136">Not yet documented</span></span>|
|<span data-ttu-id="c05fd-137">девицеманажементскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="c05fd-137">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="c05fd-138">Коллекция [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c05fd-138">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="c05fd-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c05fd-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c05fd-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="c05fd-140">Response</span></span>
<span data-ttu-id="c05fd-141">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c05fd-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c05fd-142">Пример</span><span class="sxs-lookup"><span data-stu-id="c05fd-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="c05fd-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="c05fd-143">Request</span></span>
<span data-ttu-id="c05fd-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c05fd-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c05fd-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c05fd-145">Response</span></span>
<span data-ttu-id="c05fd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c05fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







