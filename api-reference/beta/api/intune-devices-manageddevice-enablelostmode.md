---
title: Действие enableLostMode
description: Включение режима потери
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22f75fb0c9dd4405717584de77b06a89eaf33bb8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958482"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="35e2c-103">Действие enableLostMode</span><span class="sxs-lookup"><span data-stu-id="35e2c-103">enableLostMode action</span></span>

> <span data-ttu-id="35e2c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35e2c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35e2c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35e2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35e2c-106">Включение режима потери</span><span class="sxs-lookup"><span data-stu-id="35e2c-106">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35e2c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="35e2c-107">Prerequisites</span></span>
<span data-ttu-id="35e2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35e2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35e2c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35e2c-110">Permission type</span></span>|<span data-ttu-id="35e2c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35e2c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35e2c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35e2c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35e2c-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="35e2c-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="35e2c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35e2c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35e2c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35e2c-115">Not supported.</span></span>|
|<span data-ttu-id="35e2c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35e2c-116">Application</span></span>|<span data-ttu-id="35e2c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35e2c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35e2c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35e2c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="35e2c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35e2c-119">Request headers</span></span>
|<span data-ttu-id="35e2c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35e2c-120">Header</span></span>|<span data-ttu-id="35e2c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="35e2c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35e2c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35e2c-122">Authorization</span></span>|<span data-ttu-id="35e2c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35e2c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35e2c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="35e2c-124">Accept</span></span>|<span data-ttu-id="35e2c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35e2c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35e2c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35e2c-126">Request body</span></span>
<span data-ttu-id="35e2c-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35e2c-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="35e2c-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="35e2c-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="35e2c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="35e2c-129">Property</span></span>|<span data-ttu-id="35e2c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="35e2c-130">Type</span></span>|<span data-ttu-id="35e2c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="35e2c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35e2c-132">message</span><span class="sxs-lookup"><span data-stu-id="35e2c-132">message</span></span>|<span data-ttu-id="35e2c-133">String</span><span class="sxs-lookup"><span data-stu-id="35e2c-133">String</span></span>|<span data-ttu-id="35e2c-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="35e2c-134">Not yet documented</span></span>|
|<span data-ttu-id="35e2c-135">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="35e2c-135">phoneNumber</span></span>|<span data-ttu-id="35e2c-136">String</span><span class="sxs-lookup"><span data-stu-id="35e2c-136">String</span></span>|<span data-ttu-id="35e2c-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="35e2c-137">Not yet documented</span></span>|
|<span data-ttu-id="35e2c-138">нижний колонтитул</span><span class="sxs-lookup"><span data-stu-id="35e2c-138">footer</span></span>|<span data-ttu-id="35e2c-139">String</span><span class="sxs-lookup"><span data-stu-id="35e2c-139">String</span></span>|<span data-ttu-id="35e2c-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="35e2c-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="35e2c-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="35e2c-141">Response</span></span>
<span data-ttu-id="35e2c-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="35e2c-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="35e2c-143">Пример</span><span class="sxs-lookup"><span data-stu-id="35e2c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="35e2c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="35e2c-144">Request</span></span>
<span data-ttu-id="35e2c-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35e2c-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="35e2c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="35e2c-146">Response</span></span>
<span data-ttu-id="35e2c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35e2c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





