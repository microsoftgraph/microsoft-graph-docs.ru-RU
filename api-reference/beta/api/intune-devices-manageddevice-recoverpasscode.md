---
title: Действие recoverPasscode
description: Восстановление секретного кода
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 510f6db344364cb95b67692c937e3a484b16641f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944752"
---
# <a name="recoverpasscode-action"></a><span data-ttu-id="2744a-103">Действие recoverPasscode</span><span class="sxs-lookup"><span data-stu-id="2744a-103">recoverPasscode action</span></span>

> <span data-ttu-id="2744a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2744a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2744a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2744a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2744a-106">Восстановление секретного кода</span><span class="sxs-lookup"><span data-stu-id="2744a-106">Recover passcode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2744a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2744a-107">Prerequisites</span></span>
<span data-ttu-id="2744a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2744a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2744a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2744a-110">Permission type</span></span>|<span data-ttu-id="2744a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2744a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2744a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2744a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2744a-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="2744a-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="2744a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2744a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2744a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2744a-115">Not supported.</span></span>|
|<span data-ttu-id="2744a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2744a-116">Application</span></span>|<span data-ttu-id="2744a-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="2744a-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2744a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2744a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/recoverPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/recoverPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/recoverPasscode
```

## <a name="request-headers"></a><span data-ttu-id="2744a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2744a-119">Request headers</span></span>
|<span data-ttu-id="2744a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2744a-120">Header</span></span>|<span data-ttu-id="2744a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2744a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2744a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2744a-122">Authorization</span></span>|<span data-ttu-id="2744a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2744a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2744a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2744a-124">Accept</span></span>|<span data-ttu-id="2744a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2744a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2744a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2744a-126">Request body</span></span>
<span data-ttu-id="2744a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2744a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2744a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2744a-128">Response</span></span>
<span data-ttu-id="2744a-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2744a-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2744a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2744a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2744a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2744a-131">Request</span></span>
<span data-ttu-id="2744a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2744a-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/recoverPasscode
```

### <a name="response"></a><span data-ttu-id="2744a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2744a-133">Response</span></span>
<span data-ttu-id="2744a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2744a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





