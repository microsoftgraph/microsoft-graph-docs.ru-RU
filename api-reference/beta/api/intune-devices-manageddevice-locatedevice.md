---
title: Действие locateDevice
description: Поиск устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20a1c0548605f17242d017dedf0e85d7c691abb7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958405"
---
# <a name="locatedevice-action"></a><span data-ttu-id="98faf-103">Действие locateDevice</span><span class="sxs-lookup"><span data-stu-id="98faf-103">locateDevice action</span></span>

> <span data-ttu-id="98faf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98faf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98faf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98faf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98faf-106">Поиск устройства</span><span class="sxs-lookup"><span data-stu-id="98faf-106">Locate a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98faf-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="98faf-107">Prerequisites</span></span>
<span data-ttu-id="98faf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98faf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98faf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98faf-110">Permission type</span></span>|<span data-ttu-id="98faf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98faf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98faf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98faf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98faf-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="98faf-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="98faf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98faf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98faf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98faf-115">Not supported.</span></span>|
|<span data-ttu-id="98faf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98faf-116">Application</span></span>|<span data-ttu-id="98faf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98faf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98faf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98faf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/locateDevice
```

## <a name="request-headers"></a><span data-ttu-id="98faf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98faf-119">Request headers</span></span>
|<span data-ttu-id="98faf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98faf-120">Header</span></span>|<span data-ttu-id="98faf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="98faf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98faf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98faf-122">Authorization</span></span>|<span data-ttu-id="98faf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98faf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98faf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="98faf-124">Accept</span></span>|<span data-ttu-id="98faf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98faf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98faf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98faf-126">Request body</span></span>
<span data-ttu-id="98faf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98faf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98faf-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="98faf-128">Response</span></span>
<span data-ttu-id="98faf-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="98faf-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="98faf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="98faf-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="98faf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="98faf-131">Request</span></span>
<span data-ttu-id="98faf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98faf-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/locateDevice
```

### <a name="response"></a><span data-ttu-id="98faf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="98faf-133">Response</span></span>
<span data-ttu-id="98faf-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98faf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





