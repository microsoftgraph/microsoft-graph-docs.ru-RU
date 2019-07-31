---
title: Действие remoteLock
description: Удаленная блокировка
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60bef7349d74340e96c485bbe55a5e1c3ce21a95
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981404"
---
# <a name="remotelock-action"></a><span data-ttu-id="253aa-103">Действие remoteLock</span><span class="sxs-lookup"><span data-stu-id="253aa-103">remoteLock action</span></span>

> <span data-ttu-id="253aa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="253aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="253aa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="253aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="253aa-106">Удаленная блокировка</span><span class="sxs-lookup"><span data-stu-id="253aa-106">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="253aa-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="253aa-107">Prerequisites</span></span>
<span data-ttu-id="253aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="253aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="253aa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="253aa-110">Permission type</span></span>|<span data-ttu-id="253aa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="253aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="253aa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="253aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="253aa-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="253aa-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="253aa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="253aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="253aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="253aa-115">Not supported.</span></span>|
|<span data-ttu-id="253aa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="253aa-116">Application</span></span>|<span data-ttu-id="253aa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="253aa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="253aa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="253aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/remoteLock
```

## <a name="request-headers"></a><span data-ttu-id="253aa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="253aa-119">Request headers</span></span>
|<span data-ttu-id="253aa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="253aa-120">Header</span></span>|<span data-ttu-id="253aa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="253aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="253aa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="253aa-122">Authorization</span></span>|<span data-ttu-id="253aa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="253aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="253aa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="253aa-124">Accept</span></span>|<span data-ttu-id="253aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="253aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="253aa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="253aa-126">Request body</span></span>
<span data-ttu-id="253aa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="253aa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="253aa-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="253aa-128">Response</span></span>
<span data-ttu-id="253aa-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="253aa-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="253aa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="253aa-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="253aa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="253aa-131">Request</span></span>
<span data-ttu-id="253aa-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="253aa-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="253aa-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="253aa-133">Response</span></span>
<span data-ttu-id="253aa-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="253aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





