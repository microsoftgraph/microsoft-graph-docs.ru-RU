---
title: Действие assignResourceAccountToDevice
description: Назначение учетной записи ресурса автопилотным устройствам.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4cdf4a176e18b6f68328e6eba286e3298e2a9be1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943721"
---
# <a name="assignresourceaccounttodevice-action"></a><span data-ttu-id="b3e46-103">Действие assignResourceAccountToDevice</span><span class="sxs-lookup"><span data-stu-id="b3e46-103">assignResourceAccountToDevice action</span></span>

> <span data-ttu-id="b3e46-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3e46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3e46-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3e46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3e46-106">Назначение учетной записи ресурса автопилотным устройствам.</span><span class="sxs-lookup"><span data-stu-id="b3e46-106">Assigns resource account to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3e46-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b3e46-107">Prerequisites</span></span>
<span data-ttu-id="b3e46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3e46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3e46-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3e46-110">Permission type</span></span>|<span data-ttu-id="b3e46-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3e46-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3e46-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3e46-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3e46-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3e46-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b3e46-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3e46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3e46-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3e46-115">Not supported.</span></span>|
|<span data-ttu-id="b3e46-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3e46-116">Application</span></span>|<span data-ttu-id="b3e46-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3e46-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3e46-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3e46-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
```

## <a name="request-headers"></a><span data-ttu-id="b3e46-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b3e46-119">Request headers</span></span>
|<span data-ttu-id="b3e46-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3e46-120">Header</span></span>|<span data-ttu-id="b3e46-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b3e46-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3e46-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3e46-122">Authorization</span></span>|<span data-ttu-id="b3e46-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3e46-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3e46-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b3e46-124">Accept</span></span>|<span data-ttu-id="b3e46-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3e46-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3e46-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b3e46-126">Request body</span></span>
<span data-ttu-id="b3e46-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3e46-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b3e46-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b3e46-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b3e46-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3e46-129">Property</span></span>|<span data-ttu-id="b3e46-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b3e46-130">Type</span></span>|<span data-ttu-id="b3e46-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b3e46-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3e46-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b3e46-132">userPrincipalName</span></span>|<span data-ttu-id="b3e46-133">String</span><span class="sxs-lookup"><span data-stu-id="b3e46-133">String</span></span>|<span data-ttu-id="b3e46-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b3e46-134">Not yet documented</span></span>|
|<span data-ttu-id="b3e46-135">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="b3e46-135">addressableUserName</span></span>|<span data-ttu-id="b3e46-136">String</span><span class="sxs-lookup"><span data-stu-id="b3e46-136">String</span></span>|<span data-ttu-id="b3e46-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b3e46-137">Not yet documented</span></span>|
|<span data-ttu-id="b3e46-138">ресаурцеаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="b3e46-138">resourceAccountName</span></span>|<span data-ttu-id="b3e46-139">String</span><span class="sxs-lookup"><span data-stu-id="b3e46-139">String</span></span>|<span data-ttu-id="b3e46-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b3e46-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b3e46-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3e46-141">Response</span></span>
<span data-ttu-id="b3e46-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b3e46-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b3e46-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b3e46-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3e46-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3e46-144">Request</span></span>
<span data-ttu-id="b3e46-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3e46-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b3e46-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3e46-146">Response</span></span>
<span data-ttu-id="b3e46-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3e46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





