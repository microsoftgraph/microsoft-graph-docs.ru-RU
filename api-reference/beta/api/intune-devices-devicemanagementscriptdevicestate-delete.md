---
title: Удаление deviceManagementScriptDeviceState
description: Удаляет устройствоManagementScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 504a7955bcfd989a51a386b8b19b13c4deb97344
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155969"
---
# <a name="delete-devicemanagementscriptdevicestate"></a><span data-ttu-id="e4844-103">Удаление deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="e4844-103">Delete deviceManagementScriptDeviceState</span></span>

<span data-ttu-id="e4844-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4844-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4844-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4844-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4844-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4844-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4844-107">Удаляет [устройствоManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="e4844-107">Deletes a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4844-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4844-108">Prerequisites</span></span>
<span data-ttu-id="e4844-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4844-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4844-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4844-111">Permission type</span></span>|<span data-ttu-id="e4844-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4844-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4844-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4844-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4844-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4844-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e4844-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4844-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4844-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4844-116">Not supported.</span></span>|
|<span data-ttu-id="e4844-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e4844-117">Application</span></span>|<span data-ttu-id="e4844-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4844-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4844-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4844-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
DELETE /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="e4844-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e4844-120">Request headers</span></span>
|<span data-ttu-id="e4844-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4844-121">Header</span></span>|<span data-ttu-id="e4844-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e4844-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4844-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4844-123">Authorization</span></span>|<span data-ttu-id="e4844-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4844-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4844-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4844-125">Accept</span></span>|<span data-ttu-id="e4844-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4844-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4844-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4844-127">Request body</span></span>
<span data-ttu-id="e4844-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4844-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4844-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4844-129">Response</span></span>
<span data-ttu-id="e4844-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4844-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4844-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e4844-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4844-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4844-132">Request</span></span>
<span data-ttu-id="e4844-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4844-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="e4844-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4844-134">Response</span></span>
<span data-ttu-id="e4844-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4844-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




