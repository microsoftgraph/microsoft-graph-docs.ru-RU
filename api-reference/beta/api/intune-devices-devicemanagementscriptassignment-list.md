---
title: Список Девицеманажементскриптассигнментс
description: Список свойств и связей объектов Девицеманажементскриптассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6320b953f2d1924656431e747b6fc85476a72b1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469421"
---
# <a name="list-devicemanagementscriptassignments"></a><span data-ttu-id="cf504-103">Список Девицеманажементскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="cf504-103">List deviceManagementScriptAssignments</span></span>

<span data-ttu-id="cf504-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cf504-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf504-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf504-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf504-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf504-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf504-107">Список свойств и связей объектов [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="cf504-107">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf504-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf504-108">Prerequisites</span></span>
<span data-ttu-id="cf504-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf504-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf504-111">Permission type</span></span>|<span data-ttu-id="cf504-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf504-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf504-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf504-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf504-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf504-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cf504-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf504-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf504-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf504-116">Not supported.</span></span>|
|<span data-ttu-id="cf504-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf504-117">Application</span></span>|<span data-ttu-id="cf504-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf504-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf504-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf504-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="cf504-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf504-120">Request headers</span></span>
|<span data-ttu-id="cf504-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf504-121">Header</span></span>|<span data-ttu-id="cf504-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf504-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf504-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf504-123">Authorization</span></span>|<span data-ttu-id="cf504-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf504-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf504-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf504-125">Accept</span></span>|<span data-ttu-id="cf504-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf504-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf504-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf504-127">Request body</span></span>
<span data-ttu-id="cf504-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf504-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf504-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf504-129">Response</span></span>
<span data-ttu-id="cf504-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf504-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf504-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cf504-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf504-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf504-132">Request</span></span>
<span data-ttu-id="cf504-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf504-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
```

### <a name="response"></a><span data-ttu-id="cf504-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf504-134">Response</span></span>
<span data-ttu-id="cf504-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf504-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
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





