---
title: Сценарий настраиваемой оболочки атрибутов устройства назначает действие
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9a42bdcdef7e15e1b32215243221af2e3fdbc90f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666319"
---
# <a name="device-custom-attribute-shell-script--assign-action"></a><span data-ttu-id="2fefd-103">Сценарий настраиваемой оболочки атрибутов устройства назначает действие</span><span class="sxs-lookup"><span data-stu-id="2fefd-103">Device custom attribute shell script  assign action</span></span>

<span data-ttu-id="2fefd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fefd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fefd-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fefd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fefd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2fefd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fefd-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2fefd-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fefd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2fefd-108">Prerequisites</span></span>
<span data-ttu-id="2fefd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fefd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fefd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fefd-111">Permission type</span></span>|<span data-ttu-id="2fefd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fefd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fefd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fefd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2fefd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fefd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2fefd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fefd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fefd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fefd-116">Not supported.</span></span>|
|<span data-ttu-id="2fefd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2fefd-117">Application</span></span>|<span data-ttu-id="2fefd-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fefd-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fefd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fefd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="2fefd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2fefd-120">Request headers</span></span>
|<span data-ttu-id="2fefd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2fefd-121">Header</span></span>|<span data-ttu-id="2fefd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2fefd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fefd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fefd-123">Authorization</span></span>|<span data-ttu-id="2fefd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2fefd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fefd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2fefd-125">Accept</span></span>|<span data-ttu-id="2fefd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fefd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fefd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2fefd-127">Request body</span></span>
<span data-ttu-id="2fefd-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fefd-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2fefd-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2fefd-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2fefd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fefd-130">Property</span></span>|<span data-ttu-id="2fefd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2fefd-131">Type</span></span>|<span data-ttu-id="2fefd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2fefd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fefd-133">DeviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="2fefd-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="2fefd-134">[коллекция deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2fefd-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="2fefd-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2fefd-135">Not yet documented</span></span>|
|<span data-ttu-id="2fefd-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="2fefd-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="2fefd-137">[коллекция deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2fefd-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="2fefd-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2fefd-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2fefd-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="2fefd-139">Response</span></span>
<span data-ttu-id="2fefd-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2fefd-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2fefd-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2fefd-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fefd-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fefd-142">Request</span></span>
<span data-ttu-id="2fefd-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fefd-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assign

Content-type: application/json
Content-length: 781

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
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="2fefd-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fefd-144">Response</span></span>
<span data-ttu-id="2fefd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2fefd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




