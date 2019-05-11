---
title: Действие retire
description: Прекращение использования устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: abe9e189fe3f27357c4cd0407d0c1fbec34a5f12
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909598"
---
# <a name="retire-action"></a><span data-ttu-id="5eabe-103">Действие retire</span><span class="sxs-lookup"><span data-stu-id="5eabe-103">retire action</span></span>

> <span data-ttu-id="5eabe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eabe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5eabe-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5eabe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5eabe-106">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="5eabe-106">Retire a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5eabe-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5eabe-107">Prerequisites</span></span>
<span data-ttu-id="5eabe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eabe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eabe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5eabe-110">Permission type</span></span>|<span data-ttu-id="5eabe-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5eabe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5eabe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5eabe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5eabe-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5eabe-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="5eabe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5eabe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5eabe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eabe-115">Not supported.</span></span>|
|<span data-ttu-id="5eabe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5eabe-116">Application</span></span>|<span data-ttu-id="5eabe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eabe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5eabe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5eabe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/retire
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/retire
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/retire
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/retire
```

## <a name="request-headers"></a><span data-ttu-id="5eabe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5eabe-119">Request headers</span></span>
|<span data-ttu-id="5eabe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5eabe-120">Header</span></span>|<span data-ttu-id="5eabe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5eabe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5eabe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5eabe-122">Authorization</span></span>|<span data-ttu-id="5eabe-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5eabe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5eabe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5eabe-124">Accept</span></span>|<span data-ttu-id="5eabe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5eabe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eabe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5eabe-126">Request body</span></span>
<span data-ttu-id="5eabe-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5eabe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eabe-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5eabe-128">Response</span></span>
<span data-ttu-id="5eabe-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5eabe-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5eabe-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5eabe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5eabe-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5eabe-131">Request</span></span>
<span data-ttu-id="5eabe-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5eabe-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/retire
```

### <a name="response"></a><span data-ttu-id="5eabe-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5eabe-133">Response</span></span>
<span data-ttu-id="5eabe-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5eabe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




