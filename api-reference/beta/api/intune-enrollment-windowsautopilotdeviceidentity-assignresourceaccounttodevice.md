---
title: Действие assignResourceAccountToDevice
description: Назначение учетной записи ресурса автопилотным устройствам.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0310aa83288b1f6e5548fac664e15792218e7989
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466362"
---
# <a name="assignresourceaccounttodevice-action"></a><span data-ttu-id="26e7f-103">Действие assignResourceAccountToDevice</span><span class="sxs-lookup"><span data-stu-id="26e7f-103">assignResourceAccountToDevice action</span></span>

<span data-ttu-id="26e7f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="26e7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26e7f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26e7f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26e7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26e7f-107">Назначение учетной записи ресурса автопилотным устройствам.</span><span class="sxs-lookup"><span data-stu-id="26e7f-107">Assigns resource account to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26e7f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="26e7f-108">Prerequisites</span></span>
<span data-ttu-id="26e7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26e7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26e7f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26e7f-111">Permission type</span></span>|<span data-ttu-id="26e7f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26e7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26e7f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26e7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26e7f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26e7f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="26e7f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26e7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26e7f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e7f-116">Not supported.</span></span>|
|<span data-ttu-id="26e7f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26e7f-117">Application</span></span>|<span data-ttu-id="26e7f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26e7f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26e7f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26e7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
```

## <a name="request-headers"></a><span data-ttu-id="26e7f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26e7f-120">Request headers</span></span>
|<span data-ttu-id="26e7f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26e7f-121">Header</span></span>|<span data-ttu-id="26e7f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="26e7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26e7f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26e7f-123">Authorization</span></span>|<span data-ttu-id="26e7f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26e7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26e7f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26e7f-125">Accept</span></span>|<span data-ttu-id="26e7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26e7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26e7f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26e7f-127">Request body</span></span>
<span data-ttu-id="26e7f-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26e7f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="26e7f-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="26e7f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="26e7f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="26e7f-130">Property</span></span>|<span data-ttu-id="26e7f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="26e7f-131">Type</span></span>|<span data-ttu-id="26e7f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="26e7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e7f-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="26e7f-133">userPrincipalName</span></span>|<span data-ttu-id="26e7f-134">String</span><span class="sxs-lookup"><span data-stu-id="26e7f-134">String</span></span>|<span data-ttu-id="26e7f-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="26e7f-135">Not yet documented</span></span>|
|<span data-ttu-id="26e7f-136">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="26e7f-136">addressableUserName</span></span>|<span data-ttu-id="26e7f-137">String</span><span class="sxs-lookup"><span data-stu-id="26e7f-137">String</span></span>|<span data-ttu-id="26e7f-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="26e7f-138">Not yet documented</span></span>|
|<span data-ttu-id="26e7f-139">ресаурцеаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="26e7f-139">resourceAccountName</span></span>|<span data-ttu-id="26e7f-140">String</span><span class="sxs-lookup"><span data-stu-id="26e7f-140">String</span></span>|<span data-ttu-id="26e7f-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="26e7f-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="26e7f-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="26e7f-142">Response</span></span>
<span data-ttu-id="26e7f-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="26e7f-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="26e7f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="26e7f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="26e7f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="26e7f-145">Request</span></span>
<span data-ttu-id="26e7f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26e7f-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26e7f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e7f-147">Response</span></span>
<span data-ttu-id="26e7f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26e7f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





