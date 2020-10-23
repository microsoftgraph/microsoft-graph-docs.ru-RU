---
title: действие Упдатедевицепропертиес
description: Обновляет свойства устройств с автопилотом.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3601d117de7e273344e9c27cfd52b095243e2ed7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726754"
---
# <a name="updatedeviceproperties-action"></a><span data-ttu-id="d5ec2-103">действие Упдатедевицепропертиес</span><span class="sxs-lookup"><span data-stu-id="d5ec2-103">updateDeviceProperties action</span></span>

<span data-ttu-id="d5ec2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5ec2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5ec2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5ec2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5ec2-107">Обновляет свойства устройств с автопилотом.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-107">Updates properties on Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5ec2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d5ec2-108">Prerequisites</span></span>
<span data-ttu-id="d5ec2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5ec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5ec2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5ec2-111">Permission type</span></span>|<span data-ttu-id="d5ec2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5ec2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5ec2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5ec2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5ec2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5ec2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d5ec2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5ec2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5ec2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-116">Not supported.</span></span>|
|<span data-ttu-id="d5ec2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5ec2-117">Application</span></span>|<span data-ttu-id="d5ec2-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5ec2-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5ec2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5ec2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/updateDeviceProperties
```

## <a name="request-headers"></a><span data-ttu-id="d5ec2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5ec2-120">Request headers</span></span>
|<span data-ttu-id="d5ec2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5ec2-121">Header</span></span>|<span data-ttu-id="d5ec2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d5ec2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5ec2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5ec2-123">Authorization</span></span>|<span data-ttu-id="d5ec2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5ec2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5ec2-125">Accept</span></span>|<span data-ttu-id="d5ec2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5ec2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5ec2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5ec2-127">Request body</span></span>
<span data-ttu-id="d5ec2-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d5ec2-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d5ec2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5ec2-130">Property</span></span>|<span data-ttu-id="d5ec2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d5ec2-131">Type</span></span>|<span data-ttu-id="d5ec2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d5ec2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5ec2-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d5ec2-133">userPrincipalName</span></span>|<span data-ttu-id="d5ec2-134">String</span><span class="sxs-lookup"><span data-stu-id="d5ec2-134">String</span></span>|<span data-ttu-id="d5ec2-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-135">Not yet documented</span></span>|
|<span data-ttu-id="d5ec2-136">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="d5ec2-136">addressableUserName</span></span>|<span data-ttu-id="d5ec2-137">String</span><span class="sxs-lookup"><span data-stu-id="d5ec2-137">String</span></span>|<span data-ttu-id="d5ec2-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-138">Not yet documented</span></span>|
|<span data-ttu-id="d5ec2-139">грауптаг</span><span class="sxs-lookup"><span data-stu-id="d5ec2-139">groupTag</span></span>|<span data-ttu-id="d5ec2-140">String</span><span class="sxs-lookup"><span data-stu-id="d5ec2-140">String</span></span>|<span data-ttu-id="d5ec2-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-141">Not yet documented</span></span>|
|<span data-ttu-id="d5ec2-142">displayName</span><span class="sxs-lookup"><span data-stu-id="d5ec2-142">displayName</span></span>|<span data-ttu-id="d5ec2-143">Строка</span><span class="sxs-lookup"><span data-stu-id="d5ec2-143">String</span></span>|<span data-ttu-id="d5ec2-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d5ec2-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5ec2-145">Response</span></span>
<span data-ttu-id="d5ec2-146">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d5ec2-147">Пример</span><span class="sxs-lookup"><span data-stu-id="d5ec2-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5ec2-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5ec2-148">Request</span></span>
<span data-ttu-id="d5ec2-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d5ec2-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5ec2-150">Response</span></span>
<span data-ttu-id="d5ec2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5ec2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





