---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e4403754bd44f0e7ed0a590f81849eb7f09a873b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49229186"
---
# <a name="assign-action"></a><span data-ttu-id="728da-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="728da-103">assign action</span></span>

<span data-ttu-id="728da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="728da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="728da-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="728da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="728da-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="728da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="728da-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="728da-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="728da-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="728da-108">Prerequisites</span></span>
<span data-ttu-id="728da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="728da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="728da-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="728da-111">Permission type</span></span>|<span data-ttu-id="728da-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="728da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="728da-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="728da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="728da-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="728da-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="728da-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="728da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="728da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="728da-116">Not supported.</span></span>|
|<span data-ttu-id="728da-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="728da-117">Application</span></span>|<span data-ttu-id="728da-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="728da-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="728da-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="728da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="728da-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="728da-120">Request headers</span></span>
|<span data-ttu-id="728da-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="728da-121">Header</span></span>|<span data-ttu-id="728da-122">Значение</span><span class="sxs-lookup"><span data-stu-id="728da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="728da-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="728da-123">Authorization</span></span>|<span data-ttu-id="728da-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="728da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="728da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="728da-125">Accept</span></span>|<span data-ttu-id="728da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="728da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="728da-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="728da-127">Request body</span></span>
<span data-ttu-id="728da-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="728da-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="728da-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="728da-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="728da-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="728da-130">Property</span></span>|<span data-ttu-id="728da-131">Тип</span><span class="sxs-lookup"><span data-stu-id="728da-131">Type</span></span>|<span data-ttu-id="728da-132">Описание</span><span class="sxs-lookup"><span data-stu-id="728da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="728da-133">девицехеалсскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="728da-133">deviceHealthScriptAssignments</span></span>|<span data-ttu-id="728da-134">Коллекция [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="728da-134">[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) collection</span></span>|<span data-ttu-id="728da-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="728da-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="728da-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="728da-136">Response</span></span>
<span data-ttu-id="728da-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="728da-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="728da-138">Пример</span><span class="sxs-lookup"><span data-stu-id="728da-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="728da-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="728da-139">Request</span></span>
<span data-ttu-id="728da-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="728da-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assign

Content-type: application/json
Content-length: 688

{
  "deviceHealthScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
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

### <a name="response"></a><span data-ttu-id="728da-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="728da-141">Response</span></span>
<span data-ttu-id="728da-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="728da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




