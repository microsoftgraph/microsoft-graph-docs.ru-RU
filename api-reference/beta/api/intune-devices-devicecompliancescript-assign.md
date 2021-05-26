---
title: Сценарий соответствия требованиям устройств назначает действие
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 115becc83d2cccc9fba80b734181bdbfcd1bec71
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664953"
---
# <a name="device-compliance-script-assign-action"></a><span data-ttu-id="55ee5-103">Сценарий соответствия требованиям устройств назначает действие</span><span class="sxs-lookup"><span data-stu-id="55ee5-103">Device compliance script assign action</span></span>

<span data-ttu-id="55ee5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55ee5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55ee5-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55ee5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55ee5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55ee5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55ee5-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="55ee5-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55ee5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="55ee5-108">Prerequisites</span></span>
<span data-ttu-id="55ee5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55ee5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55ee5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55ee5-111">Permission type</span></span>|<span data-ttu-id="55ee5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55ee5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55ee5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55ee5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55ee5-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55ee5-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="55ee5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55ee5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55ee5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55ee5-116">Not supported.</span></span>|
|<span data-ttu-id="55ee5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="55ee5-117">Application</span></span>|<span data-ttu-id="55ee5-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55ee5-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55ee5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55ee5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="55ee5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="55ee5-120">Request headers</span></span>
|<span data-ttu-id="55ee5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55ee5-121">Header</span></span>|<span data-ttu-id="55ee5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="55ee5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55ee5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55ee5-123">Authorization</span></span>|<span data-ttu-id="55ee5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55ee5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55ee5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55ee5-125">Accept</span></span>|<span data-ttu-id="55ee5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55ee5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55ee5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55ee5-127">Request body</span></span>
<span data-ttu-id="55ee5-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55ee5-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="55ee5-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="55ee5-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="55ee5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="55ee5-130">Property</span></span>|<span data-ttu-id="55ee5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="55ee5-131">Type</span></span>|<span data-ttu-id="55ee5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="55ee5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55ee5-133">DeviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="55ee5-133">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="55ee5-134">[коллекция deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="55ee5-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="55ee5-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="55ee5-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="55ee5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="55ee5-136">Response</span></span>
<span data-ttu-id="55ee5-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="55ee5-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="55ee5-138">Пример</span><span class="sxs-lookup"><span data-stu-id="55ee5-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="55ee5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="55ee5-139">Request</span></span>
<span data-ttu-id="55ee5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55ee5-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assign

Content-type: application/json
Content-length: 756

{
  "deviceHealthScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
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

### <a name="response"></a><span data-ttu-id="55ee5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="55ee5-141">Response</span></span>
<span data-ttu-id="55ee5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55ee5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




