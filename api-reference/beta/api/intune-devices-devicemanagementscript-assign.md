---
title: Действие assign
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a3a54693fcb2c689827e41d811cd616d428dc83f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934396"
---
# <a name="assign-action"></a><span data-ttu-id="e5dbf-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="e5dbf-103">assign action</span></span>

> <span data-ttu-id="e5dbf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5dbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5dbf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5dbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5dbf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e5dbf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5dbf-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e5dbf-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5dbf-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e5dbf-108">Prerequisites</span></span>
<span data-ttu-id="e5dbf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5dbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5dbf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5dbf-111">Permission type</span></span>|<span data-ttu-id="e5dbf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5dbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5dbf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5dbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5dbf-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5dbf-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e5dbf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5dbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5dbf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5dbf-116">Not supported.</span></span>|
|<span data-ttu-id="e5dbf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5dbf-117">Application</span></span>|<span data-ttu-id="e5dbf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5dbf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5dbf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5dbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e5dbf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5dbf-120">Request headers</span></span>
|<span data-ttu-id="e5dbf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5dbf-121">Header</span></span>|<span data-ttu-id="e5dbf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5dbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5dbf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5dbf-123">Authorization</span></span>|<span data-ttu-id="e5dbf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e5dbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5dbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5dbf-125">Accept</span></span>|<span data-ttu-id="e5dbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5dbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5dbf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5dbf-127">Request body</span></span>
<span data-ttu-id="e5dbf-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5dbf-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e5dbf-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e5dbf-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e5dbf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5dbf-130">Property</span></span>|<span data-ttu-id="e5dbf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e5dbf-131">Type</span></span>|<span data-ttu-id="e5dbf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e5dbf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5dbf-133">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="e5dbf-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="e5dbf-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e5dbf-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="e5dbf-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e5dbf-135">Not yet documented</span></span>|
|<span data-ttu-id="e5dbf-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="e5dbf-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="e5dbf-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e5dbf-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="e5dbf-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e5dbf-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e5dbf-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5dbf-139">Response</span></span>
<span data-ttu-id="e5dbf-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e5dbf-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e5dbf-141">Пример</span><span class="sxs-lookup"><span data-stu-id="e5dbf-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5dbf-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5dbf-142">Request</span></span>
<span data-ttu-id="e5dbf-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5dbf-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e5dbf-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5dbf-144">Response</span></span>
<span data-ttu-id="e5dbf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e5dbf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





