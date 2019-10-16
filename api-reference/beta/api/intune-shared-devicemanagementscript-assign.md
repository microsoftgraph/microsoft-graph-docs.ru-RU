---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f66c96934a174a99e4d1c35b7c548c3dc4181ada
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538170"
---
# <a name="assign-action"></a><span data-ttu-id="d0687-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="d0687-103">assign action</span></span>

> <span data-ttu-id="d0687-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0687-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0687-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0687-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0687-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d0687-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0687-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d0687-107">Prerequisites</span></span>
<span data-ttu-id="d0687-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0687-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0687-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0687-110">Permission type</span></span>|<span data-ttu-id="d0687-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0687-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0687-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0687-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d0687-113">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d0687-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d0687-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0687-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d0687-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0687-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0687-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0687-116">Not supported.</span></span>|
|<span data-ttu-id="d0687-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d0687-117">Application</span></span>||
| <span data-ttu-id="d0687-118">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d0687-118">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d0687-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0687-119">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0687-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0687-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d0687-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0687-121">Request headers</span></span>
|<span data-ttu-id="d0687-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0687-122">Header</span></span>|<span data-ttu-id="d0687-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d0687-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0687-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0687-124">Authorization</span></span>|<span data-ttu-id="d0687-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0687-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0687-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d0687-126">Accept</span></span>|<span data-ttu-id="d0687-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d0687-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0687-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0687-128">Request body</span></span>
<span data-ttu-id="d0687-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0687-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d0687-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d0687-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d0687-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0687-131">Property</span></span>|<span data-ttu-id="d0687-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d0687-132">Type</span></span>|<span data-ttu-id="d0687-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d0687-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0687-134">девицеманажементскриптграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="d0687-134">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="d0687-135">Коллекция [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d0687-135">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="d0687-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d0687-136">Not yet documented</span></span>|
|<span data-ttu-id="d0687-137">девицеманажементскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="d0687-137">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="d0687-138">Коллекция [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d0687-138">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="d0687-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d0687-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d0687-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0687-140">Response</span></span>
<span data-ttu-id="d0687-141">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d0687-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d0687-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d0687-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0687-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0687-143">Request</span></span>
<span data-ttu-id="d0687-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0687-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d0687-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0687-145">Response</span></span>
<span data-ttu-id="d0687-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0687-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






