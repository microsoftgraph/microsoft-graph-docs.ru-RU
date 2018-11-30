---
title: Действие executeAction
description: Н/Д
ms.openlocfilehash: 1358b95bbb61aaef71df44c87ab6aeb0bc210761
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081986"
---
# <a name="executeaction-action"></a><span data-ttu-id="33326-103">Действие executeAction</span><span class="sxs-lookup"><span data-stu-id="33326-103">executeAction action</span></span>

> <span data-ttu-id="33326-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="33326-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33326-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33326-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33326-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="33326-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33326-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="33326-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33326-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="33326-108">Prerequisites</span></span>
<span data-ttu-id="33326-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33326-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33326-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33326-111">Permission type</span></span>|<span data-ttu-id="33326-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33326-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33326-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33326-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33326-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="33326-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="33326-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33326-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33326-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33326-116">Not supported.</span></span>|
|<span data-ttu-id="33326-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33326-117">Application</span></span>|<span data-ttu-id="33326-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33326-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33326-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33326-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/executeAction
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="33326-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33326-120">Request headers</span></span>
|<span data-ttu-id="33326-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33326-121">Header</span></span>|<span data-ttu-id="33326-122">Значение</span><span class="sxs-lookup"><span data-stu-id="33326-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33326-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33326-123">Authorization</span></span>|<span data-ttu-id="33326-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="33326-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33326-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33326-125">Accept</span></span>|<span data-ttu-id="33326-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33326-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33326-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33326-127">Request body</span></span>
<span data-ttu-id="33326-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33326-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="33326-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="33326-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="33326-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="33326-130">Property</span></span>|<span data-ttu-id="33326-131">Тип</span><span class="sxs-lookup"><span data-stu-id="33326-131">Type</span></span>|<span data-ttu-id="33326-132">Описание</span><span class="sxs-lookup"><span data-stu-id="33326-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33326-133">actionName</span><span class="sxs-lookup"><span data-stu-id="33326-133">actionName</span></span>|[<span data-ttu-id="33326-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="33326-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="33326-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="33326-135">Not yet documented</span></span>|
|<span data-ttu-id="33326-136">deviceIds</span><span class="sxs-lookup"><span data-stu-id="33326-136">deviceIds</span></span>|<span data-ttu-id="33326-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="33326-137">String collection</span></span>|<span data-ttu-id="33326-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="33326-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="33326-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="33326-139">Response</span></span>
<span data-ttu-id="33326-140">Если успешно завершена, это действие возвращает `200 OK` код ответа и [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="33326-140">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33326-141">Пример</span><span class="sxs-lookup"><span data-stu-id="33326-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="33326-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="33326-142">Request</span></span>
<span data-ttu-id="33326-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33326-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/executeAction

Content-type: application/json
Content-length: 78

{
  "actionName": "delete",
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="33326-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="33326-144">Response</span></span>
<span data-ttu-id="33326-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="33326-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult",
    "successfulDeviceIds": [
      "Successful Device Ids value"
    ],
    "failedDeviceIds": [
      "Failed Device Ids value"
    ],
    "notFoundDeviceIds": [
      "Not Found Device Ids value"
    ],
    "notSupportedDeviceIds": [
      "Not Supported Device Ids value"
    ]
  }
}
```





