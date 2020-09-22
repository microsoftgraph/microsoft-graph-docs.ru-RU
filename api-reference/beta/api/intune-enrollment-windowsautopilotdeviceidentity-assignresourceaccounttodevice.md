---
title: Действие assignResourceAccountToDevice
description: Назначение учетной записи ресурса автопилотным устройствам.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9b8c51e15785088d9f9d8e388168690f8f7fcc4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011160"
---
# <a name="assignresourceaccounttodevice-action"></a><span data-ttu-id="26f32-103">Действие assignResourceAccountToDevice</span><span class="sxs-lookup"><span data-stu-id="26f32-103">assignResourceAccountToDevice action</span></span>

<span data-ttu-id="26f32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26f32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26f32-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26f32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26f32-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26f32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26f32-107">Назначение учетной записи ресурса автопилотным устройствам.</span><span class="sxs-lookup"><span data-stu-id="26f32-107">Assigns resource account to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26f32-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="26f32-108">Prerequisites</span></span>
<span data-ttu-id="26f32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26f32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26f32-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26f32-111">Permission type</span></span>|<span data-ttu-id="26f32-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26f32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26f32-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26f32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26f32-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26f32-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="26f32-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26f32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26f32-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26f32-116">Not supported.</span></span>|
|<span data-ttu-id="26f32-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26f32-117">Application</span></span>|<span data-ttu-id="26f32-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26f32-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26f32-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26f32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
```

## <a name="request-headers"></a><span data-ttu-id="26f32-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26f32-120">Request headers</span></span>
|<span data-ttu-id="26f32-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26f32-121">Header</span></span>|<span data-ttu-id="26f32-122">Значение</span><span class="sxs-lookup"><span data-stu-id="26f32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26f32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26f32-123">Authorization</span></span>|<span data-ttu-id="26f32-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26f32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26f32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26f32-125">Accept</span></span>|<span data-ttu-id="26f32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26f32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26f32-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26f32-127">Request body</span></span>
<span data-ttu-id="26f32-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26f32-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="26f32-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="26f32-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="26f32-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="26f32-130">Property</span></span>|<span data-ttu-id="26f32-131">Тип</span><span class="sxs-lookup"><span data-stu-id="26f32-131">Type</span></span>|<span data-ttu-id="26f32-132">Описание</span><span class="sxs-lookup"><span data-stu-id="26f32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26f32-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="26f32-133">userPrincipalName</span></span>|<span data-ttu-id="26f32-134">String</span><span class="sxs-lookup"><span data-stu-id="26f32-134">String</span></span>|<span data-ttu-id="26f32-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="26f32-135">Not yet documented</span></span>|
|<span data-ttu-id="26f32-136">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="26f32-136">addressableUserName</span></span>|<span data-ttu-id="26f32-137">String</span><span class="sxs-lookup"><span data-stu-id="26f32-137">String</span></span>|<span data-ttu-id="26f32-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="26f32-138">Not yet documented</span></span>|
|<span data-ttu-id="26f32-139">ресаурцеаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="26f32-139">resourceAccountName</span></span>|<span data-ttu-id="26f32-140">String</span><span class="sxs-lookup"><span data-stu-id="26f32-140">String</span></span>|<span data-ttu-id="26f32-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="26f32-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="26f32-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="26f32-142">Response</span></span>
<span data-ttu-id="26f32-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="26f32-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="26f32-144">Пример</span><span class="sxs-lookup"><span data-stu-id="26f32-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="26f32-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="26f32-145">Request</span></span>
<span data-ttu-id="26f32-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26f32-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice

Content-type: application/json
Content-length: 170

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value",
  "resourceAccountName": "Resource Account Name value"
}
```

### <a name="response"></a><span data-ttu-id="26f32-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="26f32-147">Response</span></span>
<span data-ttu-id="26f32-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26f32-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






