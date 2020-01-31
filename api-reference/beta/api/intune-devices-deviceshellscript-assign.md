---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c1a888271cfdd03d13101b7adaeff9295b61b44e
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636471"
---
# <a name="assign-action"></a><span data-ttu-id="d1bbe-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="d1bbe-103">assign action</span></span>

> <span data-ttu-id="d1bbe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1bbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1bbe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1bbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1bbe-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1bbe-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1bbe-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d1bbe-107">Prerequisites</span></span>
<span data-ttu-id="d1bbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1bbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1bbe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1bbe-110">Permission type</span></span>|<span data-ttu-id="d1bbe-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1bbe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1bbe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1bbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1bbe-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1bbe-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d1bbe-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1bbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1bbe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1bbe-115">Not supported.</span></span>|
|<span data-ttu-id="d1bbe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1bbe-116">Application</span></span>|<span data-ttu-id="d1bbe-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1bbe-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1bbe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1bbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d1bbe-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d1bbe-119">Request headers</span></span>
|<span data-ttu-id="d1bbe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1bbe-120">Header</span></span>|<span data-ttu-id="d1bbe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d1bbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1bbe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1bbe-122">Authorization</span></span>|<span data-ttu-id="d1bbe-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1bbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1bbe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d1bbe-124">Accept</span></span>|<span data-ttu-id="d1bbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1bbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1bbe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1bbe-126">Request body</span></span>
<span data-ttu-id="d1bbe-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1bbe-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d1bbe-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d1bbe-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d1bbe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1bbe-129">Property</span></span>|<span data-ttu-id="d1bbe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d1bbe-130">Type</span></span>|<span data-ttu-id="d1bbe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d1bbe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1bbe-132">девицеманажементскриптграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="d1bbe-132">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="d1bbe-133">Коллекция [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d1bbe-133">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="d1bbe-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1bbe-134">Not yet documented</span></span>|
|<span data-ttu-id="d1bbe-135">девицеманажементскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="d1bbe-135">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="d1bbe-136">Коллекция [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d1bbe-136">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="d1bbe-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d1bbe-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d1bbe-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1bbe-138">Response</span></span>
<span data-ttu-id="d1bbe-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d1bbe-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d1bbe-140">Пример</span><span class="sxs-lookup"><span data-stu-id="d1bbe-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1bbe-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1bbe-141">Request</span></span>
<span data-ttu-id="d1bbe-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1bbe-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assign

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

### <a name="response"></a><span data-ttu-id="d1bbe-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1bbe-143">Response</span></span>
<span data-ttu-id="d1bbe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1bbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





