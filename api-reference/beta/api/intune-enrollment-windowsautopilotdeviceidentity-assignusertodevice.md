---
title: Действие assignUserToDevice
description: Назначение пользователям автопилотных устройств.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60e21b15d239c3485bf1e09880a188ed80d4de84
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452425"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="884e4-103">Действие assignUserToDevice</span><span class="sxs-lookup"><span data-stu-id="884e4-103">assignUserToDevice action</span></span>

<span data-ttu-id="884e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="884e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="884e4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="884e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="884e4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="884e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="884e4-107">Назначение пользователям автопилотных устройств.</span><span class="sxs-lookup"><span data-stu-id="884e4-107">Assigns user to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="884e4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="884e4-108">Prerequisites</span></span>
<span data-ttu-id="884e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="884e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="884e4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="884e4-111">Permission type</span></span>|<span data-ttu-id="884e4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="884e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="884e4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="884e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="884e4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="884e4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="884e4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="884e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="884e4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="884e4-116">Not supported.</span></span>|
|<span data-ttu-id="884e4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="884e4-117">Application</span></span>|<span data-ttu-id="884e4-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="884e4-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="884e4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="884e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="884e4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="884e4-120">Request headers</span></span>
|<span data-ttu-id="884e4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="884e4-121">Header</span></span>|<span data-ttu-id="884e4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="884e4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="884e4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="884e4-123">Authorization</span></span>|<span data-ttu-id="884e4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="884e4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="884e4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="884e4-125">Accept</span></span>|<span data-ttu-id="884e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="884e4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="884e4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="884e4-127">Request body</span></span>
<span data-ttu-id="884e4-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="884e4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="884e4-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="884e4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="884e4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="884e4-130">Property</span></span>|<span data-ttu-id="884e4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="884e4-131">Type</span></span>|<span data-ttu-id="884e4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="884e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="884e4-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="884e4-133">userPrincipalName</span></span>|<span data-ttu-id="884e4-134">String</span><span class="sxs-lookup"><span data-stu-id="884e4-134">String</span></span>|<span data-ttu-id="884e4-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="884e4-135">Not yet documented</span></span>|
|<span data-ttu-id="884e4-136">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="884e4-136">addressableUserName</span></span>|<span data-ttu-id="884e4-137">String</span><span class="sxs-lookup"><span data-stu-id="884e4-137">String</span></span>|<span data-ttu-id="884e4-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="884e4-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="884e4-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="884e4-139">Response</span></span>
<span data-ttu-id="884e4-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="884e4-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="884e4-141">Пример</span><span class="sxs-lookup"><span data-stu-id="884e4-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="884e4-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="884e4-142">Request</span></span>
<span data-ttu-id="884e4-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="884e4-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="884e4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="884e4-144">Response</span></span>
<span data-ttu-id="884e4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="884e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



