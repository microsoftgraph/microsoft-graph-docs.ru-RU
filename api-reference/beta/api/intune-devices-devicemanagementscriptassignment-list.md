---
title: Список Девицеманажементскриптассигнментс
description: Список свойств и связей объектов Девицеманажементскриптассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5dd298e0f1724b3b0be15306229211bddc71ff5
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945011"
---
# <a name="list-devicemanagementscriptassignments"></a><span data-ttu-id="d94d6-103">Список Девицеманажементскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="d94d6-103">List deviceManagementScriptAssignments</span></span>

> <span data-ttu-id="d94d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d94d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d94d6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d94d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d94d6-106">Список свойств и связей объектов [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d94d6-106">List properties and relationships of the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d94d6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d94d6-107">Prerequisites</span></span>
<span data-ttu-id="d94d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d94d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d94d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d94d6-110">Permission type</span></span>|<span data-ttu-id="d94d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d94d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d94d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d94d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d94d6-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d94d6-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d94d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d94d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d94d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d94d6-115">Not supported.</span></span>|
|<span data-ttu-id="d94d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d94d6-116">Application</span></span>|<span data-ttu-id="d94d6-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d94d6-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d94d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d94d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d94d6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d94d6-119">Request headers</span></span>
|<span data-ttu-id="d94d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d94d6-120">Header</span></span>|<span data-ttu-id="d94d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d94d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d94d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d94d6-122">Authorization</span></span>|<span data-ttu-id="d94d6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d94d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d94d6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d94d6-124">Accept</span></span>|<span data-ttu-id="d94d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d94d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d94d6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d94d6-126">Request body</span></span>
<span data-ttu-id="d94d6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d94d6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d94d6-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d94d6-128">Response</span></span>
<span data-ttu-id="d94d6-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d94d6-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d94d6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d94d6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d94d6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d94d6-131">Request</span></span>
<span data-ttu-id="d94d6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d94d6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
```

### <a name="response"></a><span data-ttu-id="d94d6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d94d6-133">Response</span></span>
<span data-ttu-id="d94d6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d94d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





