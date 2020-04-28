---
title: Действие assignResourceAccountToDevice
description: Назначение учетной записи ресурса автопилотным устройствам.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: deb3eeaf2070b1ae673f7e8223c02787e20e9178
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452448"
---
# <a name="assignresourceaccounttodevice-action"></a><span data-ttu-id="f15e5-103">Действие assignResourceAccountToDevice</span><span class="sxs-lookup"><span data-stu-id="f15e5-103">assignResourceAccountToDevice action</span></span>

<span data-ttu-id="f15e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f15e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f15e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f15e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f15e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f15e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f15e5-107">Назначение учетной записи ресурса автопилотным устройствам.</span><span class="sxs-lookup"><span data-stu-id="f15e5-107">Assigns resource account to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f15e5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f15e5-108">Prerequisites</span></span>
<span data-ttu-id="f15e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f15e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f15e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f15e5-111">Permission type</span></span>|<span data-ttu-id="f15e5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f15e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f15e5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f15e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f15e5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f15e5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f15e5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f15e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f15e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f15e5-116">Not supported.</span></span>|
|<span data-ttu-id="f15e5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f15e5-117">Application</span></span>|<span data-ttu-id="f15e5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f15e5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f15e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f15e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
```

## <a name="request-headers"></a><span data-ttu-id="f15e5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f15e5-120">Request headers</span></span>
|<span data-ttu-id="f15e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f15e5-121">Header</span></span>|<span data-ttu-id="f15e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f15e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f15e5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f15e5-123">Authorization</span></span>|<span data-ttu-id="f15e5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f15e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f15e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f15e5-125">Accept</span></span>|<span data-ttu-id="f15e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f15e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f15e5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f15e5-127">Request body</span></span>
<span data-ttu-id="f15e5-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f15e5-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f15e5-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f15e5-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f15e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f15e5-130">Property</span></span>|<span data-ttu-id="f15e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f15e5-131">Type</span></span>|<span data-ttu-id="f15e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f15e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f15e5-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f15e5-133">userPrincipalName</span></span>|<span data-ttu-id="f15e5-134">String</span><span class="sxs-lookup"><span data-stu-id="f15e5-134">String</span></span>|<span data-ttu-id="f15e5-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f15e5-135">Not yet documented</span></span>|
|<span data-ttu-id="f15e5-136">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="f15e5-136">addressableUserName</span></span>|<span data-ttu-id="f15e5-137">String</span><span class="sxs-lookup"><span data-stu-id="f15e5-137">String</span></span>|<span data-ttu-id="f15e5-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f15e5-138">Not yet documented</span></span>|
|<span data-ttu-id="f15e5-139">ресаурцеаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="f15e5-139">resourceAccountName</span></span>|<span data-ttu-id="f15e5-140">String</span><span class="sxs-lookup"><span data-stu-id="f15e5-140">String</span></span>|<span data-ttu-id="f15e5-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f15e5-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f15e5-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="f15e5-142">Response</span></span>
<span data-ttu-id="f15e5-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f15e5-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f15e5-144">Пример</span><span class="sxs-lookup"><span data-stu-id="f15e5-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="f15e5-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="f15e5-145">Request</span></span>
<span data-ttu-id="f15e5-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f15e5-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f15e5-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f15e5-147">Response</span></span>
<span data-ttu-id="f15e5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f15e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



