---
title: Действие wipe
description: Очистка устройства
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 91b04311692609687792ce22c5cc81074239ba23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842842"
---
# <a name="wipe-action"></a><span data-ttu-id="66957-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="66957-103">wipe action</span></span>

> <span data-ttu-id="66957-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="66957-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66957-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66957-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66957-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="66957-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66957-107">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="66957-107">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66957-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="66957-108">Prerequisites</span></span>
<span data-ttu-id="66957-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66957-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66957-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66957-111">Permission type</span></span>|<span data-ttu-id="66957-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66957-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66957-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66957-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66957-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="66957-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="66957-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66957-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66957-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66957-116">Not supported.</span></span>|
|<span data-ttu-id="66957-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66957-117">Application</span></span>|<span data-ttu-id="66957-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66957-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66957-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66957-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="66957-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66957-120">Request headers</span></span>
|<span data-ttu-id="66957-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66957-121">Header</span></span>|<span data-ttu-id="66957-122">Значение</span><span class="sxs-lookup"><span data-stu-id="66957-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66957-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66957-123">Authorization</span></span>|<span data-ttu-id="66957-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="66957-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66957-125">Accept</span><span class="sxs-lookup"><span data-stu-id="66957-125">Accept</span></span>|<span data-ttu-id="66957-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66957-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66957-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="66957-127">Request body</span></span>
<span data-ttu-id="66957-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66957-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="66957-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="66957-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="66957-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="66957-130">Property</span></span>|<span data-ttu-id="66957-131">Тип</span><span class="sxs-lookup"><span data-stu-id="66957-131">Type</span></span>|<span data-ttu-id="66957-132">Описание</span><span class="sxs-lookup"><span data-stu-id="66957-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66957-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="66957-133">keepEnrollmentData</span></span>|<span data-ttu-id="66957-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="66957-134">Boolean</span></span>|<span data-ttu-id="66957-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="66957-135">Not yet documented</span></span>|
|<span data-ttu-id="66957-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="66957-136">keepUserData</span></span>|<span data-ttu-id="66957-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="66957-137">Boolean</span></span>|<span data-ttu-id="66957-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="66957-138">Not yet documented</span></span>|
|<span data-ttu-id="66957-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="66957-139">macOsUnlockCode</span></span>|<span data-ttu-id="66957-140">String</span><span class="sxs-lookup"><span data-stu-id="66957-140">String</span></span>|<span data-ttu-id="66957-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="66957-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="66957-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="66957-142">Response</span></span>
<span data-ttu-id="66957-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="66957-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="66957-144">Пример</span><span class="sxs-lookup"><span data-stu-id="66957-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="66957-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="66957-145">Request</span></span>
<span data-ttu-id="66957-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66957-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="66957-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="66957-147">Response</span></span>
<span data-ttu-id="66957-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="66957-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





