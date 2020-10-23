---
title: Список Девицеманажементскриптграупассигнментс
description: Список свойств и связей объектов Девицеманажементскриптграупассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38e284888c245f113045c02d18dc1835747dcedf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48689610"
---
# <a name="list-devicemanagementscriptgroupassignments"></a><span data-ttu-id="9834a-103">Список Девицеманажементскриптграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="9834a-103">List deviceManagementScriptGroupAssignments</span></span>

<span data-ttu-id="9834a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9834a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9834a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9834a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9834a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9834a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9834a-107">Список свойств и связей объектов [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9834a-107">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9834a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9834a-108">Prerequisites</span></span>
<span data-ttu-id="9834a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9834a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9834a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9834a-111">Permission type</span></span>|<span data-ttu-id="9834a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9834a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9834a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9834a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9834a-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9834a-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9834a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9834a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9834a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9834a-116">Not supported.</span></span>|
|<span data-ttu-id="9834a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9834a-117">Application</span></span>|<span data-ttu-id="9834a-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9834a-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9834a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9834a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
GET /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="9834a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9834a-120">Request headers</span></span>
|<span data-ttu-id="9834a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9834a-121">Header</span></span>|<span data-ttu-id="9834a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9834a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9834a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9834a-123">Authorization</span></span>|<span data-ttu-id="9834a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9834a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9834a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9834a-125">Accept</span></span>|<span data-ttu-id="9834a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9834a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9834a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9834a-127">Request body</span></span>
<span data-ttu-id="9834a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9834a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9834a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9834a-129">Response</span></span>
<span data-ttu-id="9834a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9834a-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9834a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9834a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9834a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9834a-132">Request</span></span>
<span data-ttu-id="9834a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9834a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="9834a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9834a-134">Response</span></span>
<span data-ttu-id="9834a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9834a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
      "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
      "targetGroupId": "Target Group Id value"
    }
  ]
}
```





