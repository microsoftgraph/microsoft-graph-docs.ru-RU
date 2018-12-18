---
title: Действие setDeviceName
description: Задайте имя устройства устройства.
author: tfitzmac
ms.openlocfilehash: 9856e9698da807e3bb3af1a3c30fa7e138569f48
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352173"
---
# <a name="setdevicename-action"></a><span data-ttu-id="44ab7-103">Действие setDeviceName</span><span class="sxs-lookup"><span data-stu-id="44ab7-103">setDeviceName action</span></span>

> <span data-ttu-id="44ab7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44ab7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44ab7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44ab7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44ab7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="44ab7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44ab7-107">Задайте имя устройства устройства.</span><span class="sxs-lookup"><span data-stu-id="44ab7-107">Set device name of the device.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44ab7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44ab7-108">Prerequisites</span></span>
<span data-ttu-id="44ab7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44ab7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44ab7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44ab7-111">Permission type</span></span>|<span data-ttu-id="44ab7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44ab7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44ab7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44ab7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44ab7-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="44ab7-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="44ab7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44ab7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44ab7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44ab7-116">Not supported.</span></span>|
|<span data-ttu-id="44ab7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44ab7-117">Application</span></span>|<span data-ttu-id="44ab7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44ab7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44ab7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44ab7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/setDeviceName
```

## <a name="request-headers"></a><span data-ttu-id="44ab7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44ab7-120">Request headers</span></span>
|<span data-ttu-id="44ab7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44ab7-121">Header</span></span>|<span data-ttu-id="44ab7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="44ab7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44ab7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44ab7-123">Authorization</span></span>|<span data-ttu-id="44ab7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="44ab7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44ab7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44ab7-125">Accept</span></span>|<span data-ttu-id="44ab7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44ab7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44ab7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44ab7-127">Request body</span></span>
<span data-ttu-id="44ab7-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44ab7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="44ab7-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="44ab7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="44ab7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="44ab7-130">Property</span></span>|<span data-ttu-id="44ab7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="44ab7-131">Type</span></span>|<span data-ttu-id="44ab7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="44ab7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ab7-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="44ab7-133">deviceName</span></span>|<span data-ttu-id="44ab7-134">String</span><span class="sxs-lookup"><span data-stu-id="44ab7-134">String</span></span>|<span data-ttu-id="44ab7-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="44ab7-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="44ab7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="44ab7-136">Response</span></span>
<span data-ttu-id="44ab7-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="44ab7-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="44ab7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="44ab7-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="44ab7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="44ab7-139">Request</span></span>
<span data-ttu-id="44ab7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44ab7-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/setDeviceName

Content-type: application/json
Content-length: 41

{
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="44ab7-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="44ab7-141">Response</span></span>
<span data-ttu-id="44ab7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="44ab7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





