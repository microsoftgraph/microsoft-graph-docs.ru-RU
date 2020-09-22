---
title: действие Упдатедевицепропертиес
description: Обновляет свойства устройств с автопилотом.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f92f1d67ac1315a68c5f909a8fbd25a7deab5e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056032"
---
# <a name="updatedeviceproperties-action"></a><span data-ttu-id="4d8e8-103">действие Упдатедевицепропертиес</span><span class="sxs-lookup"><span data-stu-id="4d8e8-103">updateDeviceProperties action</span></span>

<span data-ttu-id="4d8e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d8e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d8e8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d8e8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d8e8-107">Обновляет свойства устройств с автопилотом.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-107">Updates properties on Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d8e8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4d8e8-108">Prerequisites</span></span>
<span data-ttu-id="4d8e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d8e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d8e8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d8e8-111">Permission type</span></span>|<span data-ttu-id="4d8e8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d8e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d8e8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d8e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d8e8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d8e8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4d8e8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d8e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d8e8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-116">Not supported.</span></span>|
|<span data-ttu-id="4d8e8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d8e8-117">Application</span></span>|<span data-ttu-id="4d8e8-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d8e8-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d8e8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d8e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
```

## <a name="request-headers"></a><span data-ttu-id="4d8e8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4d8e8-120">Request headers</span></span>
|<span data-ttu-id="4d8e8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d8e8-121">Header</span></span>|<span data-ttu-id="4d8e8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4d8e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d8e8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d8e8-123">Authorization</span></span>|<span data-ttu-id="4d8e8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d8e8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4d8e8-125">Accept</span></span>|<span data-ttu-id="4d8e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d8e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d8e8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d8e8-127">Request body</span></span>
<span data-ttu-id="4d8e8-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4d8e8-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4d8e8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d8e8-130">Property</span></span>|<span data-ttu-id="4d8e8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4d8e8-131">Type</span></span>|<span data-ttu-id="4d8e8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4d8e8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d8e8-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4d8e8-133">userPrincipalName</span></span>|<span data-ttu-id="4d8e8-134">String</span><span class="sxs-lookup"><span data-stu-id="4d8e8-134">String</span></span>|<span data-ttu-id="4d8e8-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-135">Not yet documented</span></span>|
|<span data-ttu-id="4d8e8-136">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="4d8e8-136">addressableUserName</span></span>|<span data-ttu-id="4d8e8-137">String</span><span class="sxs-lookup"><span data-stu-id="4d8e8-137">String</span></span>|<span data-ttu-id="4d8e8-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-138">Not yet documented</span></span>|
|<span data-ttu-id="4d8e8-139">грауптаг</span><span class="sxs-lookup"><span data-stu-id="4d8e8-139">groupTag</span></span>|<span data-ttu-id="4d8e8-140">String</span><span class="sxs-lookup"><span data-stu-id="4d8e8-140">String</span></span>|<span data-ttu-id="4d8e8-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-141">Not yet documented</span></span>|
|<span data-ttu-id="4d8e8-142">displayName</span><span class="sxs-lookup"><span data-stu-id="4d8e8-142">displayName</span></span>|<span data-ttu-id="4d8e8-143">String</span><span class="sxs-lookup"><span data-stu-id="4d8e8-143">String</span></span>|<span data-ttu-id="4d8e8-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4d8e8-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d8e8-145">Response</span></span>
<span data-ttu-id="4d8e8-146">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4d8e8-147">Пример</span><span class="sxs-lookup"><span data-stu-id="4d8e8-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d8e8-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d8e8-148">Request</span></span>
<span data-ttu-id="4d8e8-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d8e8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d8e8-150">Response</span></span>
<span data-ttu-id="4d8e8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






