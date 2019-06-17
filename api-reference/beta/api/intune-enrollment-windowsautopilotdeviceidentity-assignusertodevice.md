---
title: Действие assignUserToDevice
description: Назначение пользователям автопилотных устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20618d933935ff515aa0d022dbfd1e9d237a99b2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982842"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="a6f72-103">Действие assignUserToDevice</span><span class="sxs-lookup"><span data-stu-id="a6f72-103">assignUserToDevice action</span></span>

> <span data-ttu-id="a6f72-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6f72-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6f72-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6f72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6f72-106">Назначение пользователям автопилотных устройств.</span><span class="sxs-lookup"><span data-stu-id="a6f72-106">Assigns user to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6f72-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a6f72-107">Prerequisites</span></span>
<span data-ttu-id="a6f72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6f72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6f72-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6f72-110">Permission type</span></span>|<span data-ttu-id="a6f72-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6f72-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6f72-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6f72-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6f72-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6f72-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a6f72-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6f72-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6f72-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6f72-115">Not supported.</span></span>|
|<span data-ttu-id="a6f72-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6f72-116">Application</span></span>|<span data-ttu-id="a6f72-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6f72-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6f72-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6f72-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="a6f72-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6f72-119">Request headers</span></span>
|<span data-ttu-id="a6f72-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6f72-120">Header</span></span>|<span data-ttu-id="a6f72-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a6f72-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6f72-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6f72-122">Authorization</span></span>|<span data-ttu-id="a6f72-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6f72-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6f72-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a6f72-124">Accept</span></span>|<span data-ttu-id="a6f72-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6f72-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6f72-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6f72-126">Request body</span></span>
<span data-ttu-id="a6f72-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6f72-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a6f72-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a6f72-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a6f72-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6f72-129">Property</span></span>|<span data-ttu-id="a6f72-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a6f72-130">Type</span></span>|<span data-ttu-id="a6f72-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a6f72-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6f72-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a6f72-132">userPrincipalName</span></span>|<span data-ttu-id="a6f72-133">String</span><span class="sxs-lookup"><span data-stu-id="a6f72-133">String</span></span>|<span data-ttu-id="a6f72-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a6f72-134">Not yet documented</span></span>|
|<span data-ttu-id="a6f72-135">Аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="a6f72-135">addressableUserName</span></span>|<span data-ttu-id="a6f72-136">String</span><span class="sxs-lookup"><span data-stu-id="a6f72-136">String</span></span>|<span data-ttu-id="a6f72-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a6f72-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a6f72-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6f72-138">Response</span></span>
<span data-ttu-id="a6f72-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a6f72-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a6f72-140">Пример</span><span class="sxs-lookup"><span data-stu-id="a6f72-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6f72-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6f72-141">Request</span></span>
<span data-ttu-id="a6f72-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6f72-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="a6f72-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6f72-143">Response</span></span>
<span data-ttu-id="a6f72-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6f72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





