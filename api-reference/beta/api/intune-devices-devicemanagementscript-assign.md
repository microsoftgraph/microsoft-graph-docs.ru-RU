---
title: Действие assign
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 189e7c73220ed88735ada7052367db589ad2905e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171332"
---
# <a name="assign-action"></a><span data-ttu-id="7c50f-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="7c50f-103">assign action</span></span>

> <span data-ttu-id="7c50f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c50f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c50f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c50f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c50f-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c50f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c50f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7c50f-107">Prerequisites</span></span>
<span data-ttu-id="7c50f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c50f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7c50f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c50f-110">Permission type</span></span>|<span data-ttu-id="7c50f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c50f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c50f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c50f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c50f-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c50f-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7c50f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c50f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c50f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c50f-115">Not supported.</span></span>|
|<span data-ttu-id="7c50f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c50f-116">Application</span></span>|<span data-ttu-id="7c50f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c50f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c50f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c50f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7c50f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c50f-119">Request headers</span></span>
|<span data-ttu-id="7c50f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c50f-120">Header</span></span>|<span data-ttu-id="7c50f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7c50f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c50f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c50f-122">Authorization</span></span>|<span data-ttu-id="7c50f-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7c50f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c50f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7c50f-124">Accept</span></span>|<span data-ttu-id="7c50f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c50f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c50f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c50f-126">Request body</span></span>
<span data-ttu-id="7c50f-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c50f-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7c50f-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7c50f-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7c50f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c50f-129">Property</span></span>|<span data-ttu-id="7c50f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7c50f-130">Type</span></span>|<span data-ttu-id="7c50f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7c50f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c50f-132">Девицеманажементскриптграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="7c50f-132">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="7c50f-133">Коллекция [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7c50f-133">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="7c50f-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7c50f-134">Not yet documented</span></span>|
|<span data-ttu-id="7c50f-135">Девицеманажементскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="7c50f-135">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="7c50f-136">Коллекция [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7c50f-136">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="7c50f-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7c50f-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7c50f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c50f-138">Response</span></span>
<span data-ttu-id="7c50f-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7c50f-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7c50f-140">Пример</span><span class="sxs-lookup"><span data-stu-id="7c50f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c50f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c50f-141">Request</span></span>
<span data-ttu-id="7c50f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c50f-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c50f-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c50f-143">Response</span></span>
<span data-ttu-id="7c50f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7c50f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




