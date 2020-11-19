---
title: Действие resetPasscode
description: Сброс секретного кода
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7638b2fcdee88128adfc31a0d1ce5cd41f26cf6c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49234903"
---
# <a name="resetpasscode-action"></a><span data-ttu-id="a99bf-103">Действие resetPasscode</span><span class="sxs-lookup"><span data-stu-id="a99bf-103">resetPasscode action</span></span>

<span data-ttu-id="a99bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a99bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a99bf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a99bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a99bf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a99bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a99bf-107">Сброс секретного кода</span><span class="sxs-lookup"><span data-stu-id="a99bf-107">Reset passcode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a99bf-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a99bf-108">Prerequisites</span></span>
<span data-ttu-id="a99bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a99bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a99bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a99bf-111">Permission type</span></span>|<span data-ttu-id="a99bf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a99bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a99bf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a99bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a99bf-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a99bf-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a99bf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a99bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a99bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a99bf-116">Not supported.</span></span>|
|<span data-ttu-id="a99bf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a99bf-117">Application</span></span>|<span data-ttu-id="a99bf-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a99bf-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a99bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a99bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/resetPasscode
POST /deviceManagement/comanagedDevices/{managedDeviceId}/resetPasscode
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/resetPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/resetPasscode
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/resetPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/resetPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/resetPasscode
```

## <a name="request-headers"></a><span data-ttu-id="a99bf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a99bf-120">Request headers</span></span>
|<span data-ttu-id="a99bf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a99bf-121">Header</span></span>|<span data-ttu-id="a99bf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a99bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a99bf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a99bf-123">Authorization</span></span>|<span data-ttu-id="a99bf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a99bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a99bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a99bf-125">Accept</span></span>|<span data-ttu-id="a99bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a99bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a99bf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a99bf-127">Request body</span></span>
<span data-ttu-id="a99bf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a99bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a99bf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a99bf-129">Response</span></span>
<span data-ttu-id="a99bf-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a99bf-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a99bf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a99bf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a99bf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a99bf-132">Request</span></span>
<span data-ttu-id="a99bf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a99bf-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/resetPasscode
```

### <a name="response"></a><span data-ttu-id="a99bf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a99bf-134">Response</span></span>
<span data-ttu-id="a99bf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a99bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




