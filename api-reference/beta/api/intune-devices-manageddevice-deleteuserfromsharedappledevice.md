---
title: Действие deleteUserFromSharedAppleDevice
description: Удаление пользователя на общем устройстве Apple
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c2d8d04e816cac4becf85f3ad565b7be0da6518
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978264"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="32a15-103">Действие deleteUserFromSharedAppleDevice</span><span class="sxs-lookup"><span data-stu-id="32a15-103">deleteUserFromSharedAppleDevice action</span></span>

> <span data-ttu-id="32a15-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32a15-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32a15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32a15-106">Удаление пользователя на общем устройстве Apple</span><span class="sxs-lookup"><span data-stu-id="32a15-106">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32a15-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="32a15-107">Prerequisites</span></span>
<span data-ttu-id="32a15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32a15-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32a15-110">Permission type</span></span>|<span data-ttu-id="32a15-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32a15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32a15-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32a15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32a15-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="32a15-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="32a15-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32a15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32a15-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a15-115">Not supported.</span></span>|
|<span data-ttu-id="32a15-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32a15-116">Application</span></span>|<span data-ttu-id="32a15-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a15-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32a15-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32a15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="32a15-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32a15-119">Request headers</span></span>
|<span data-ttu-id="32a15-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32a15-120">Header</span></span>|<span data-ttu-id="32a15-121">Значение</span><span class="sxs-lookup"><span data-stu-id="32a15-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32a15-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32a15-122">Authorization</span></span>|<span data-ttu-id="32a15-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32a15-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32a15-124">Accept</span><span class="sxs-lookup"><span data-stu-id="32a15-124">Accept</span></span>|<span data-ttu-id="32a15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32a15-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32a15-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32a15-126">Request body</span></span>
<span data-ttu-id="32a15-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32a15-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="32a15-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="32a15-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="32a15-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="32a15-129">Property</span></span>|<span data-ttu-id="32a15-130">Тип</span><span class="sxs-lookup"><span data-stu-id="32a15-130">Type</span></span>|<span data-ttu-id="32a15-131">Описание</span><span class="sxs-lookup"><span data-stu-id="32a15-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32a15-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="32a15-132">userPrincipalName</span></span>|<span data-ttu-id="32a15-133">String</span><span class="sxs-lookup"><span data-stu-id="32a15-133">String</span></span>|<span data-ttu-id="32a15-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="32a15-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="32a15-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="32a15-135">Response</span></span>
<span data-ttu-id="32a15-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="32a15-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="32a15-137">Пример</span><span class="sxs-lookup"><span data-stu-id="32a15-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="32a15-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="32a15-138">Request</span></span>
<span data-ttu-id="32a15-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32a15-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="32a15-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="32a15-140">Response</span></span>
<span data-ttu-id="32a15-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32a15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





