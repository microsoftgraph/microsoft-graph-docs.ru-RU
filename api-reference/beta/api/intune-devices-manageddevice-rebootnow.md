---
title: Действие rebootNow
description: Перезагрузка устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 781742036efcb88141434c1763c6dd0a9daff37d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806694"
---
# <a name="rebootnow-action"></a><span data-ttu-id="2385c-103">Действие rebootNow</span><span class="sxs-lookup"><span data-stu-id="2385c-103">rebootNow action</span></span>

> <span data-ttu-id="2385c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2385c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2385c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2385c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2385c-106">Перезагрузка устройства</span><span class="sxs-lookup"><span data-stu-id="2385c-106">Reboot device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2385c-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2385c-107">Prerequisites</span></span>
<span data-ttu-id="2385c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2385c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2385c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2385c-110">Permission type</span></span>|<span data-ttu-id="2385c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2385c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2385c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2385c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2385c-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="2385c-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="2385c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2385c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2385c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2385c-115">Not supported.</span></span>|
|<span data-ttu-id="2385c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2385c-116">Application</span></span>|<span data-ttu-id="2385c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2385c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2385c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2385c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rebootNow
```

## <a name="request-headers"></a><span data-ttu-id="2385c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2385c-119">Request headers</span></span>
|<span data-ttu-id="2385c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2385c-120">Header</span></span>|<span data-ttu-id="2385c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2385c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2385c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2385c-122">Authorization</span></span>|<span data-ttu-id="2385c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2385c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2385c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2385c-124">Accept</span></span>|<span data-ttu-id="2385c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2385c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2385c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2385c-126">Request body</span></span>
<span data-ttu-id="2385c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2385c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2385c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2385c-128">Response</span></span>
<span data-ttu-id="2385c-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2385c-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2385c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2385c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2385c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2385c-131">Request</span></span>
<span data-ttu-id="2385c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2385c-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/rebootNow
```

### <a name="response"></a><span data-ttu-id="2385c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2385c-133">Response</span></span>
<span data-ttu-id="2385c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2385c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





