---
title: Действие enableLostMode
description: Включение режима потери
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 735ee2659c603b03718a0e0031973dd5addb21eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520223"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="65cef-103">Действие enableLostMode</span><span class="sxs-lookup"><span data-stu-id="65cef-103">enableLostMode action</span></span>

> <span data-ttu-id="65cef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65cef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65cef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65cef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65cef-106">Включение режима потери</span><span class="sxs-lookup"><span data-stu-id="65cef-106">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65cef-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="65cef-107">Prerequisites</span></span>
<span data-ttu-id="65cef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65cef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65cef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65cef-110">Permission type</span></span>|<span data-ttu-id="65cef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65cef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65cef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65cef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65cef-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="65cef-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="65cef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65cef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65cef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65cef-115">Not supported.</span></span>|
|<span data-ttu-id="65cef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65cef-116">Application</span></span>|<span data-ttu-id="65cef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65cef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65cef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65cef-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="65cef-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65cef-119">Request headers</span></span>
|<span data-ttu-id="65cef-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65cef-120">Header</span></span>|<span data-ttu-id="65cef-121">Значение</span><span class="sxs-lookup"><span data-stu-id="65cef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65cef-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65cef-122">Authorization</span></span>|<span data-ttu-id="65cef-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65cef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65cef-124">Accept</span><span class="sxs-lookup"><span data-stu-id="65cef-124">Accept</span></span>|<span data-ttu-id="65cef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65cef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65cef-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65cef-126">Request body</span></span>
<span data-ttu-id="65cef-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65cef-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="65cef-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="65cef-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="65cef-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="65cef-129">Property</span></span>|<span data-ttu-id="65cef-130">Тип</span><span class="sxs-lookup"><span data-stu-id="65cef-130">Type</span></span>|<span data-ttu-id="65cef-131">Описание</span><span class="sxs-lookup"><span data-stu-id="65cef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65cef-132">message</span><span class="sxs-lookup"><span data-stu-id="65cef-132">message</span></span>|<span data-ttu-id="65cef-133">String</span><span class="sxs-lookup"><span data-stu-id="65cef-133">String</span></span>|<span data-ttu-id="65cef-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="65cef-134">Not yet documented</span></span>|
|<span data-ttu-id="65cef-135">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="65cef-135">phoneNumber</span></span>|<span data-ttu-id="65cef-136">String</span><span class="sxs-lookup"><span data-stu-id="65cef-136">String</span></span>|<span data-ttu-id="65cef-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="65cef-137">Not yet documented</span></span>|
|<span data-ttu-id="65cef-138">нижний колонтитул</span><span class="sxs-lookup"><span data-stu-id="65cef-138">footer</span></span>|<span data-ttu-id="65cef-139">String</span><span class="sxs-lookup"><span data-stu-id="65cef-139">String</span></span>|<span data-ttu-id="65cef-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="65cef-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="65cef-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="65cef-141">Response</span></span>
<span data-ttu-id="65cef-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="65cef-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="65cef-143">Пример</span><span class="sxs-lookup"><span data-stu-id="65cef-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="65cef-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="65cef-144">Request</span></span>
<span data-ttu-id="65cef-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65cef-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="65cef-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="65cef-146">Response</span></span>
<span data-ttu-id="65cef-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65cef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





