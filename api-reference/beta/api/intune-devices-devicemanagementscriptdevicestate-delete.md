---
title: Удаление Девицеманажементскриптдевицестате
description: Удаляет объект Девицеманажементскриптдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b38f36ac115ed1539c667183cb818da843af236
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469400"
---
# <a name="delete-devicemanagementscriptdevicestate"></a><span data-ttu-id="90c04-103">Удаление Девицеманажементскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="90c04-103">Delete deviceManagementScriptDeviceState</span></span>

<span data-ttu-id="90c04-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="90c04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90c04-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90c04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90c04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90c04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90c04-107">Удаляет объект [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="90c04-107">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90c04-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90c04-108">Prerequisites</span></span>
<span data-ttu-id="90c04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90c04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90c04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90c04-111">Permission type</span></span>|<span data-ttu-id="90c04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90c04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90c04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90c04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90c04-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90c04-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="90c04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90c04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90c04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90c04-116">Not supported.</span></span>|
|<span data-ttu-id="90c04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90c04-117">Application</span></span>|<span data-ttu-id="90c04-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90c04-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90c04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90c04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="90c04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90c04-120">Request headers</span></span>
|<span data-ttu-id="90c04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90c04-121">Header</span></span>|<span data-ttu-id="90c04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90c04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90c04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90c04-123">Authorization</span></span>|<span data-ttu-id="90c04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90c04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90c04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90c04-125">Accept</span></span>|<span data-ttu-id="90c04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90c04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90c04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90c04-127">Request body</span></span>
<span data-ttu-id="90c04-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90c04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90c04-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c04-129">Response</span></span>
<span data-ttu-id="90c04-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="90c04-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="90c04-131">Пример</span><span class="sxs-lookup"><span data-stu-id="90c04-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="90c04-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90c04-132">Request</span></span>
<span data-ttu-id="90c04-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90c04-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="90c04-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c04-134">Response</span></span>
<span data-ttu-id="90c04-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90c04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





