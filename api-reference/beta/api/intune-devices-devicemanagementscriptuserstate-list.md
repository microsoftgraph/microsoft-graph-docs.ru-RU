---
title: Список Девицеманажементскриптусерстатес
description: Список свойств и связей объектов Девицеманажементскриптусерстате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42b294c50d823c33d4f6f88fddba3e41f4581f87
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768326"
---
# <a name="list-devicemanagementscriptuserstates"></a><span data-ttu-id="bd42c-103">Список Девицеманажементскриптусерстатес</span><span class="sxs-lookup"><span data-stu-id="bd42c-103">List deviceManagementScriptUserStates</span></span>

> <span data-ttu-id="bd42c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd42c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd42c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd42c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd42c-106">Список свойств и связей объектов [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="bd42c-106">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd42c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bd42c-107">Prerequisites</span></span>
<span data-ttu-id="bd42c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd42c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd42c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd42c-110">Permission type</span></span>|<span data-ttu-id="bd42c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd42c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd42c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd42c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd42c-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd42c-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bd42c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd42c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd42c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd42c-115">Not supported.</span></span>|
|<span data-ttu-id="bd42c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bd42c-116">Application</span></span>|<span data-ttu-id="bd42c-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd42c-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd42c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd42c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="bd42c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bd42c-119">Request headers</span></span>
|<span data-ttu-id="bd42c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd42c-120">Header</span></span>|<span data-ttu-id="bd42c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bd42c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd42c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd42c-122">Authorization</span></span>|<span data-ttu-id="bd42c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd42c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd42c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bd42c-124">Accept</span></span>|<span data-ttu-id="bd42c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd42c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd42c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd42c-126">Request body</span></span>
<span data-ttu-id="bd42c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd42c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd42c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd42c-128">Response</span></span>
<span data-ttu-id="bd42c-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd42c-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd42c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bd42c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd42c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd42c-131">Request</span></span>
<span data-ttu-id="bd42c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd42c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
```

### <a name="response"></a><span data-ttu-id="bd42c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd42c-133">Response</span></span>
<span data-ttu-id="bd42c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd42c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 282

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
      "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
      "successDeviceCount": 2,
      "errorDeviceCount": 0,
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




