---
title: Действие assignUserToDevice
description: Назначение пользователям автопилотных устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f655dd107e0a6c17ef772951ee1c146686059bf5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532592"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="21b09-103">Действие assignUserToDevice</span><span class="sxs-lookup"><span data-stu-id="21b09-103">assignUserToDevice action</span></span>

> <span data-ttu-id="21b09-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21b09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21b09-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21b09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21b09-106">Назначение пользователям автопилотных устройств.</span><span class="sxs-lookup"><span data-stu-id="21b09-106">Assigns user to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21b09-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="21b09-107">Prerequisites</span></span>
<span data-ttu-id="21b09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21b09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21b09-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21b09-110">Permission type</span></span>|<span data-ttu-id="21b09-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21b09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21b09-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21b09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21b09-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21b09-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21b09-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21b09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21b09-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21b09-115">Not supported.</span></span>|
|<span data-ttu-id="21b09-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21b09-116">Application</span></span>|<span data-ttu-id="21b09-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21b09-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21b09-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21b09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="21b09-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21b09-119">Request headers</span></span>
|<span data-ttu-id="21b09-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21b09-120">Header</span></span>|<span data-ttu-id="21b09-121">Значение</span><span class="sxs-lookup"><span data-stu-id="21b09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21b09-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21b09-122">Authorization</span></span>|<span data-ttu-id="21b09-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21b09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21b09-124">Accept</span><span class="sxs-lookup"><span data-stu-id="21b09-124">Accept</span></span>|<span data-ttu-id="21b09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21b09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21b09-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21b09-126">Request body</span></span>
<span data-ttu-id="21b09-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21b09-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="21b09-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="21b09-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="21b09-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="21b09-129">Property</span></span>|<span data-ttu-id="21b09-130">Тип</span><span class="sxs-lookup"><span data-stu-id="21b09-130">Type</span></span>|<span data-ttu-id="21b09-131">Описание</span><span class="sxs-lookup"><span data-stu-id="21b09-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21b09-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="21b09-132">userPrincipalName</span></span>|<span data-ttu-id="21b09-133">String</span><span class="sxs-lookup"><span data-stu-id="21b09-133">String</span></span>|<span data-ttu-id="21b09-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="21b09-134">Not yet documented</span></span>|
|<span data-ttu-id="21b09-135">Аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="21b09-135">addressableUserName</span></span>|<span data-ttu-id="21b09-136">String</span><span class="sxs-lookup"><span data-stu-id="21b09-136">String</span></span>|<span data-ttu-id="21b09-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="21b09-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="21b09-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="21b09-138">Response</span></span>
<span data-ttu-id="21b09-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="21b09-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="21b09-140">Пример</span><span class="sxs-lookup"><span data-stu-id="21b09-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="21b09-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="21b09-141">Request</span></span>
<span data-ttu-id="21b09-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21b09-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="21b09-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="21b09-143">Response</span></span>
<span data-ttu-id="21b09-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21b09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





