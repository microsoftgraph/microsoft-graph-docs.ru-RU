---
title: действие triggerConfigurationManagerAction
description: Действие триггера для клиента ConfigurationManager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d818b92eb7fd20a2e91351a761ae6c052a8b786
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136246"
---
# <a name="triggerconfigurationmanageraction-action"></a><span data-ttu-id="0904e-103">действие triggerConfigurationManagerAction</span><span class="sxs-lookup"><span data-stu-id="0904e-103">triggerConfigurationManagerAction action</span></span>

<span data-ttu-id="0904e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0904e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0904e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0904e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0904e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0904e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0904e-107">Действие триггера для клиента ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="0904e-107">Trigger action on ConfigurationManager client</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0904e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0904e-108">Prerequisites</span></span>
<span data-ttu-id="0904e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0904e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0904e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0904e-111">Permission type</span></span>|<span data-ttu-id="0904e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0904e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0904e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0904e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0904e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="0904e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="0904e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0904e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0904e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0904e-116">Not supported.</span></span>|
|<span data-ttu-id="0904e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0904e-117">Application</span></span>|<span data-ttu-id="0904e-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="0904e-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0904e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0904e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/comanagedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/triggerConfigurationManagerAction
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
```

## <a name="request-headers"></a><span data-ttu-id="0904e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0904e-120">Request headers</span></span>
|<span data-ttu-id="0904e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0904e-121">Header</span></span>|<span data-ttu-id="0904e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0904e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0904e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0904e-123">Authorization</span></span>|<span data-ttu-id="0904e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0904e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0904e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0904e-125">Accept</span></span>|<span data-ttu-id="0904e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0904e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0904e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0904e-127">Request body</span></span>
<span data-ttu-id="0904e-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0904e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0904e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0904e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0904e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0904e-130">Property</span></span>|<span data-ttu-id="0904e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0904e-131">Type</span></span>|<span data-ttu-id="0904e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0904e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0904e-133">configurationManagerAction</span><span class="sxs-lookup"><span data-stu-id="0904e-133">configurationManagerAction</span></span>|[<span data-ttu-id="0904e-134">configurationManagerAction</span><span class="sxs-lookup"><span data-stu-id="0904e-134">configurationManagerAction</span></span>](../resources/intune-devices-configurationmanageraction.md)|<span data-ttu-id="0904e-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0904e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0904e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0904e-136">Response</span></span>
<span data-ttu-id="0904e-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0904e-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0904e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0904e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0904e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0904e-139">Request</span></span>
<span data-ttu-id="0904e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0904e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction

Content-type: application/json
Content-length: 145

{
  "configurationManagerAction": {
    "@odata.type": "microsoft.graph.configurationManagerAction",
    "action": "refreshUserPolicy"
  }
}
```

### <a name="response"></a><span data-ttu-id="0904e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0904e-141">Response</span></span>
<span data-ttu-id="0904e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0904e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




