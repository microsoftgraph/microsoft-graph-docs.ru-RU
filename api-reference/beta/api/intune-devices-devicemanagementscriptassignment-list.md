---
title: Список Девицеманажементскриптассигнментс
description: Список свойств и связей объектов Девицеманажементскриптассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc3a8f0dadc9d092e9b404c9b9c0164f9dc36bb9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792354"
---
# <a name="list-devicemanagementscriptassignments"></a><span data-ttu-id="e90e5-103">Список Девицеманажементскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="e90e5-103">List deviceManagementScriptAssignments</span></span>

<span data-ttu-id="e90e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e90e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e90e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e90e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e90e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e90e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e90e5-107">Список свойств и связей объектов [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e90e5-107">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e90e5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e90e5-108">Prerequisites</span></span>
<span data-ttu-id="e90e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e90e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e90e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e90e5-111">Permission type</span></span>|<span data-ttu-id="e90e5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e90e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e90e5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e90e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e90e5-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e90e5-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e90e5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e90e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e90e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e90e5-116">Not supported.</span></span>|
|<span data-ttu-id="e90e5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e90e5-117">Application</span></span>|<span data-ttu-id="e90e5-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e90e5-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e90e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e90e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e90e5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e90e5-120">Request headers</span></span>
|<span data-ttu-id="e90e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e90e5-121">Header</span></span>|<span data-ttu-id="e90e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e90e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e90e5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e90e5-123">Authorization</span></span>|<span data-ttu-id="e90e5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e90e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e90e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e90e5-125">Accept</span></span>|<span data-ttu-id="e90e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e90e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e90e5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e90e5-127">Request body</span></span>
<span data-ttu-id="e90e5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e90e5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e90e5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e90e5-129">Response</span></span>
<span data-ttu-id="e90e5-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e90e5-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e90e5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e90e5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e90e5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e90e5-132">Request</span></span>
<span data-ttu-id="e90e5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e90e5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
```

### <a name="response"></a><span data-ttu-id="e90e5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e90e5-134">Response</span></span>
<span data-ttu-id="e90e5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e90e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 437

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



