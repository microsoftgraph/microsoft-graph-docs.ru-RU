---
title: activateDeviceEsim action
description: Активируйте eSIM на устройстве.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10b57e0a9c337f1c82cbc30547e57edd3c08f002
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868791"
---
# <a name="activatedeviceesim-action"></a><span data-ttu-id="99b71-103">activateDeviceEsim action</span><span class="sxs-lookup"><span data-stu-id="99b71-103">activateDeviceEsim action</span></span>

<span data-ttu-id="99b71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99b71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99b71-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99b71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99b71-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99b71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99b71-107">Активируйте eSIM на устройстве.</span><span class="sxs-lookup"><span data-stu-id="99b71-107">Activate eSIM on the device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99b71-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="99b71-108">Prerequisites</span></span>
<span data-ttu-id="99b71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99b71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99b71-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99b71-111">Permission type</span></span>|<span data-ttu-id="99b71-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99b71-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99b71-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99b71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99b71-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="99b71-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="99b71-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99b71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99b71-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99b71-116">Not supported.</span></span>|
|<span data-ttu-id="99b71-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="99b71-117">Application</span></span>|<span data-ttu-id="99b71-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="99b71-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99b71-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99b71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/activateDeviceEsim
POST /deviceManagement/comanagedDevices/{managedDeviceId}/activateDeviceEsim
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/activateDeviceEsim
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/activateDeviceEsim
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/activateDeviceEsim
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/activateDeviceEsim
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/activateDeviceEsim
```

## <a name="request-headers"></a><span data-ttu-id="99b71-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="99b71-120">Request headers</span></span>
|<span data-ttu-id="99b71-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99b71-121">Header</span></span>|<span data-ttu-id="99b71-122">Значение</span><span class="sxs-lookup"><span data-stu-id="99b71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99b71-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99b71-123">Authorization</span></span>|<span data-ttu-id="99b71-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99b71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99b71-125">Accept</span><span class="sxs-lookup"><span data-stu-id="99b71-125">Accept</span></span>|<span data-ttu-id="99b71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99b71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99b71-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99b71-127">Request body</span></span>
<span data-ttu-id="99b71-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99b71-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="99b71-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="99b71-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="99b71-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="99b71-130">Property</span></span>|<span data-ttu-id="99b71-131">Тип</span><span class="sxs-lookup"><span data-stu-id="99b71-131">Type</span></span>|<span data-ttu-id="99b71-132">Описание</span><span class="sxs-lookup"><span data-stu-id="99b71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99b71-133">carrierUrl</span><span class="sxs-lookup"><span data-stu-id="99b71-133">carrierUrl</span></span>|<span data-ttu-id="99b71-134">String</span><span class="sxs-lookup"><span data-stu-id="99b71-134">String</span></span>|<span data-ttu-id="99b71-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="99b71-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="99b71-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="99b71-136">Response</span></span>
<span data-ttu-id="99b71-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="99b71-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="99b71-138">Пример</span><span class="sxs-lookup"><span data-stu-id="99b71-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="99b71-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="99b71-139">Request</span></span>
<span data-ttu-id="99b71-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99b71-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/activateDeviceEsim

Content-type: application/json
Content-length: 55

{
  "carrierUrl": "https://example.com/carrierUrl/"
}
```

### <a name="response"></a><span data-ttu-id="99b71-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="99b71-141">Response</span></span>
<span data-ttu-id="99b71-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99b71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




