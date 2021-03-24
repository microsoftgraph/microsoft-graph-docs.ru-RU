---
title: rotateBitLockerKeys action
description: Поворот BitLockerKeys
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b436b409d6288f22e4f6fb5c1b6ce49ad824345
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136330"
---
# <a name="rotatebitlockerkeys-action"></a><span data-ttu-id="0e145-103">rotateBitLockerKeys action</span><span class="sxs-lookup"><span data-stu-id="0e145-103">rotateBitLockerKeys action</span></span>

<span data-ttu-id="0e145-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e145-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e145-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e145-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e145-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e145-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e145-107">Поворот BitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="0e145-107">Rotate BitLockerKeys</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e145-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0e145-108">Prerequisites</span></span>
<span data-ttu-id="0e145-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e145-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e145-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e145-111">Permission type</span></span>|<span data-ttu-id="0e145-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e145-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e145-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e145-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e145-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e145-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0e145-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e145-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e145-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e145-116">Not supported.</span></span>|
|<span data-ttu-id="0e145-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0e145-117">Application</span></span>|<span data-ttu-id="0e145-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e145-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e145-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e145-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/rotateBitLockerKeys
POST /deviceManagement/comanagedDevices/{managedDeviceId}/rotateBitLockerKeys
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/rotateBitLockerKeys
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rotateBitLockerKeys
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/rotateBitLockerKeys
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/rotateBitLockerKeys
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rotateBitLockerKeys
```

## <a name="request-headers"></a><span data-ttu-id="0e145-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0e145-120">Request headers</span></span>
|<span data-ttu-id="0e145-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e145-121">Header</span></span>|<span data-ttu-id="0e145-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0e145-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e145-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e145-123">Authorization</span></span>|<span data-ttu-id="0e145-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e145-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e145-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e145-125">Accept</span></span>|<span data-ttu-id="0e145-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e145-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e145-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e145-127">Request body</span></span>
<span data-ttu-id="0e145-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e145-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e145-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e145-129">Response</span></span>
<span data-ttu-id="0e145-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0e145-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e145-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0e145-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e145-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e145-132">Request</span></span>
<span data-ttu-id="0e145-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e145-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/rotateBitLockerKeys
```

### <a name="response"></a><span data-ttu-id="0e145-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e145-134">Response</span></span>
<span data-ttu-id="0e145-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e145-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




