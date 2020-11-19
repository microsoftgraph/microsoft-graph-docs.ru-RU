---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 385c2230dd6911388f3e357cae508ec5521cd481
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223908"
---
# <a name="assign-action"></a><span data-ttu-id="abd8d-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="abd8d-103">assign action</span></span>

<span data-ttu-id="abd8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abd8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abd8d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abd8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abd8d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="abd8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abd8d-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="abd8d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abd8d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="abd8d-108">Prerequisites</span></span>
<span data-ttu-id="abd8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abd8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abd8d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abd8d-111">Permission type</span></span>|<span data-ttu-id="abd8d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="abd8d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abd8d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abd8d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="abd8d-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="abd8d-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="abd8d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abd8d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="abd8d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abd8d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abd8d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abd8d-117">Not supported.</span></span>|
|<span data-ttu-id="abd8d-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="abd8d-118">Application</span></span>||
| <span data-ttu-id="abd8d-119">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="abd8d-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="abd8d-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abd8d-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abd8d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abd8d-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="abd8d-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="abd8d-122">Request headers</span></span>
|<span data-ttu-id="abd8d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="abd8d-123">Header</span></span>|<span data-ttu-id="abd8d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="abd8d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abd8d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abd8d-125">Authorization</span></span>|<span data-ttu-id="abd8d-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abd8d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abd8d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="abd8d-127">Accept</span></span>|<span data-ttu-id="abd8d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="abd8d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abd8d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abd8d-129">Request body</span></span>
<span data-ttu-id="abd8d-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abd8d-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="abd8d-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="abd8d-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="abd8d-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="abd8d-132">Property</span></span>|<span data-ttu-id="abd8d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="abd8d-133">Type</span></span>|<span data-ttu-id="abd8d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="abd8d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abd8d-135">девицеманажементскриптграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="abd8d-135">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="abd8d-136">Коллекция [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="abd8d-136">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="abd8d-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="abd8d-137">Not yet documented</span></span>|
|<span data-ttu-id="abd8d-138">девицеманажементскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="abd8d-138">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="abd8d-139">Коллекция [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="abd8d-139">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="abd8d-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="abd8d-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="abd8d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="abd8d-141">Response</span></span>
<span data-ttu-id="abd8d-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="abd8d-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="abd8d-143">Пример</span><span class="sxs-lookup"><span data-stu-id="abd8d-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="abd8d-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="abd8d-144">Request</span></span>
<span data-ttu-id="abd8d-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abd8d-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="abd8d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="abd8d-146">Response</span></span>
<span data-ttu-id="abd8d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abd8d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







