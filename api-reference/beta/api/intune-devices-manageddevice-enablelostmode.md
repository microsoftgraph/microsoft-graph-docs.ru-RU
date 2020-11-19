---
title: Действие enableLostMode
description: Включение режима потери
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f60fbccec12c879ba8f212766521c1566cf83b51
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49310491"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="9a9ab-103">Действие enableLostMode</span><span class="sxs-lookup"><span data-stu-id="9a9ab-103">enableLostMode action</span></span>

<span data-ttu-id="9a9ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a9ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a9ab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a9ab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a9ab-107">Включение режима потери</span><span class="sxs-lookup"><span data-stu-id="9a9ab-107">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a9ab-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9a9ab-108">Prerequisites</span></span>
<span data-ttu-id="9a9ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a9ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a9ab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a9ab-111">Permission type</span></span>|<span data-ttu-id="9a9ab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a9ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a9ab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a9ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a9ab-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9a9ab-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="9a9ab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a9ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a9ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-116">Not supported.</span></span>|
|<span data-ttu-id="9a9ab-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a9ab-117">Application</span></span>|<span data-ttu-id="9a9ab-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9a9ab-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a9ab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a9ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/comanagedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="9a9ab-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9a9ab-120">Request headers</span></span>
|<span data-ttu-id="9a9ab-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a9ab-121">Header</span></span>|<span data-ttu-id="9a9ab-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9a9ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a9ab-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a9ab-123">Authorization</span></span>|<span data-ttu-id="9a9ab-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a9ab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a9ab-125">Accept</span></span>|<span data-ttu-id="9a9ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a9ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a9ab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a9ab-127">Request body</span></span>
<span data-ttu-id="9a9ab-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9a9ab-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9a9ab-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a9ab-130">Property</span></span>|<span data-ttu-id="9a9ab-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9a9ab-131">Type</span></span>|<span data-ttu-id="9a9ab-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9a9ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a9ab-133">message</span><span class="sxs-lookup"><span data-stu-id="9a9ab-133">message</span></span>|<span data-ttu-id="9a9ab-134">String</span><span class="sxs-lookup"><span data-stu-id="9a9ab-134">String</span></span>|<span data-ttu-id="9a9ab-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-135">Not yet documented</span></span>|
|<span data-ttu-id="9a9ab-136">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="9a9ab-136">phoneNumber</span></span>|<span data-ttu-id="9a9ab-137">String</span><span class="sxs-lookup"><span data-stu-id="9a9ab-137">String</span></span>|<span data-ttu-id="9a9ab-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-138">Not yet documented</span></span>|
|<span data-ttu-id="9a9ab-139">нижний колонтитул</span><span class="sxs-lookup"><span data-stu-id="9a9ab-139">footer</span></span>|<span data-ttu-id="9a9ab-140">String</span><span class="sxs-lookup"><span data-stu-id="9a9ab-140">String</span></span>|<span data-ttu-id="9a9ab-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9a9ab-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a9ab-142">Response</span></span>
<span data-ttu-id="9a9ab-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9a9ab-144">Пример</span><span class="sxs-lookup"><span data-stu-id="9a9ab-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a9ab-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a9ab-145">Request</span></span>
<span data-ttu-id="9a9ab-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="9a9ab-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a9ab-147">Response</span></span>
<span data-ttu-id="9a9ab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a9ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




