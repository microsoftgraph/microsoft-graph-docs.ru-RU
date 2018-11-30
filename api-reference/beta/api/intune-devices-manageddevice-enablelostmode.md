---
title: Действие enableLostMode
description: Включение режима потеряны
ms.openlocfilehash: de49cffccf3f87e91644a33128dfdfaa74b3f233
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078679"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="6bf80-103">Действие enableLostMode</span><span class="sxs-lookup"><span data-stu-id="6bf80-103">enableLostMode action</span></span>

> <span data-ttu-id="6bf80-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6bf80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bf80-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bf80-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bf80-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6bf80-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bf80-107">Включение режима потеряны</span><span class="sxs-lookup"><span data-stu-id="6bf80-107">Enable lost mode</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6bf80-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6bf80-108">Prerequisites</span></span>
<span data-ttu-id="6bf80-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bf80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bf80-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bf80-111">Permission type</span></span>|<span data-ttu-id="6bf80-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bf80-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bf80-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bf80-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6bf80-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6bf80-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="6bf80-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bf80-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bf80-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bf80-116">Not supported.</span></span>|
|<span data-ttu-id="6bf80-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bf80-117">Application</span></span>|<span data-ttu-id="6bf80-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bf80-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bf80-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bf80-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="6bf80-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bf80-120">Request headers</span></span>
|<span data-ttu-id="6bf80-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6bf80-121">Header</span></span>|<span data-ttu-id="6bf80-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6bf80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bf80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bf80-123">Authorization</span></span>|<span data-ttu-id="6bf80-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6bf80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bf80-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6bf80-125">Accept</span></span>|<span data-ttu-id="6bf80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6bf80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bf80-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6bf80-127">Request body</span></span>
<span data-ttu-id="6bf80-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bf80-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6bf80-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="6bf80-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6bf80-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bf80-130">Property</span></span>|<span data-ttu-id="6bf80-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6bf80-131">Type</span></span>|<span data-ttu-id="6bf80-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6bf80-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bf80-133">message</span><span class="sxs-lookup"><span data-stu-id="6bf80-133">message</span></span>|<span data-ttu-id="6bf80-134">String</span><span class="sxs-lookup"><span data-stu-id="6bf80-134">String</span></span>|<span data-ttu-id="6bf80-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6bf80-135">Not yet documented</span></span>|
|<span data-ttu-id="6bf80-136">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="6bf80-136">phoneNumber</span></span>|<span data-ttu-id="6bf80-137">String</span><span class="sxs-lookup"><span data-stu-id="6bf80-137">String</span></span>|<span data-ttu-id="6bf80-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6bf80-138">Not yet documented</span></span>|
|<span data-ttu-id="6bf80-139">нижний колонтитул</span><span class="sxs-lookup"><span data-stu-id="6bf80-139">footer</span></span>|<span data-ttu-id="6bf80-140">String</span><span class="sxs-lookup"><span data-stu-id="6bf80-140">String</span></span>|<span data-ttu-id="6bf80-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6bf80-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6bf80-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="6bf80-142">Response</span></span>
<span data-ttu-id="6bf80-143">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6bf80-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6bf80-144">Пример</span><span class="sxs-lookup"><span data-stu-id="6bf80-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="6bf80-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bf80-145">Request</span></span>
<span data-ttu-id="6bf80-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bf80-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="6bf80-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="6bf80-147">Response</span></span>
<span data-ttu-id="6bf80-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6bf80-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





