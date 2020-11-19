---
title: действие Упдатедевицепропертиес
description: Обновляет свойства устройств с автопилотом.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 09598a47f945878ccd815f497e30df207db79040
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212372"
---
# <a name="updatedeviceproperties-action"></a><span data-ttu-id="43b64-103">действие Упдатедевицепропертиес</span><span class="sxs-lookup"><span data-stu-id="43b64-103">updateDeviceProperties action</span></span>

<span data-ttu-id="43b64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43b64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43b64-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43b64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43b64-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43b64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43b64-107">Обновляет свойства устройств с автопилотом.</span><span class="sxs-lookup"><span data-stu-id="43b64-107">Updates properties on Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43b64-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43b64-108">Prerequisites</span></span>
<span data-ttu-id="43b64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43b64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43b64-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43b64-111">Permission type</span></span>|<span data-ttu-id="43b64-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43b64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43b64-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43b64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43b64-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43b64-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="43b64-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43b64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43b64-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43b64-116">Not supported.</span></span>|
|<span data-ttu-id="43b64-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="43b64-117">Application</span></span>|<span data-ttu-id="43b64-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43b64-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43b64-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43b64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
```

## <a name="request-headers"></a><span data-ttu-id="43b64-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="43b64-120">Request headers</span></span>
|<span data-ttu-id="43b64-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43b64-121">Header</span></span>|<span data-ttu-id="43b64-122">Значение</span><span class="sxs-lookup"><span data-stu-id="43b64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43b64-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43b64-123">Authorization</span></span>|<span data-ttu-id="43b64-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43b64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43b64-125">Accept</span><span class="sxs-lookup"><span data-stu-id="43b64-125">Accept</span></span>|<span data-ttu-id="43b64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43b64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43b64-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43b64-127">Request body</span></span>
<span data-ttu-id="43b64-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43b64-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="43b64-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="43b64-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="43b64-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="43b64-130">Property</span></span>|<span data-ttu-id="43b64-131">Тип</span><span class="sxs-lookup"><span data-stu-id="43b64-131">Type</span></span>|<span data-ttu-id="43b64-132">Описание</span><span class="sxs-lookup"><span data-stu-id="43b64-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43b64-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="43b64-133">userPrincipalName</span></span>|<span data-ttu-id="43b64-134">String</span><span class="sxs-lookup"><span data-stu-id="43b64-134">String</span></span>|<span data-ttu-id="43b64-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="43b64-135">Not yet documented</span></span>|
|<span data-ttu-id="43b64-136">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="43b64-136">addressableUserName</span></span>|<span data-ttu-id="43b64-137">String</span><span class="sxs-lookup"><span data-stu-id="43b64-137">String</span></span>|<span data-ttu-id="43b64-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="43b64-138">Not yet documented</span></span>|
|<span data-ttu-id="43b64-139">грауптаг</span><span class="sxs-lookup"><span data-stu-id="43b64-139">groupTag</span></span>|<span data-ttu-id="43b64-140">String</span><span class="sxs-lookup"><span data-stu-id="43b64-140">String</span></span>|<span data-ttu-id="43b64-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="43b64-141">Not yet documented</span></span>|
|<span data-ttu-id="43b64-142">displayName</span><span class="sxs-lookup"><span data-stu-id="43b64-142">displayName</span></span>|<span data-ttu-id="43b64-143">String</span><span class="sxs-lookup"><span data-stu-id="43b64-143">String</span></span>|<span data-ttu-id="43b64-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="43b64-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="43b64-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="43b64-145">Response</span></span>
<span data-ttu-id="43b64-146">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="43b64-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43b64-147">Пример</span><span class="sxs-lookup"><span data-stu-id="43b64-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="43b64-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="43b64-148">Request</span></span>
<span data-ttu-id="43b64-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43b64-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties

Content-type: application/json
Content-length: 187

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value",
  "groupTag": "Group Tag value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="43b64-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="43b64-150">Response</span></span>
<span data-ttu-id="43b64-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43b64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




