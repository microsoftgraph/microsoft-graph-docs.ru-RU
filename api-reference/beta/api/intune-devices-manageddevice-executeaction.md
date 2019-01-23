---
title: Действие executeAction
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 24311c198127b2ac8fb618285e6a6eba8b44c12d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404416"
---
# <a name="executeaction-action"></a><span data-ttu-id="ef766-103">Действие executeAction</span><span class="sxs-lookup"><span data-stu-id="ef766-103">executeAction action</span></span>

> <span data-ttu-id="ef766-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef766-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ef766-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef766-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef766-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef766-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef766-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ef766-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef766-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ef766-108">Prerequisites</span></span>
<span data-ttu-id="ef766-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ef766-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ef766-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef766-111">Permission type</span></span>|<span data-ttu-id="ef766-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef766-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef766-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef766-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef766-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ef766-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ef766-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef766-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef766-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef766-116">Not supported.</span></span>|
|<span data-ttu-id="ef766-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef766-117">Application</span></span>|<span data-ttu-id="ef766-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef766-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef766-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef766-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/executeAction
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="ef766-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef766-120">Request headers</span></span>
|<span data-ttu-id="ef766-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef766-121">Header</span></span>|<span data-ttu-id="ef766-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ef766-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef766-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef766-123">Authorization</span></span>|<span data-ttu-id="ef766-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ef766-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef766-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef766-125">Accept</span></span>|<span data-ttu-id="ef766-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef766-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef766-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef766-127">Request body</span></span>
<span data-ttu-id="ef766-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef766-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ef766-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ef766-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ef766-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef766-130">Property</span></span>|<span data-ttu-id="ef766-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ef766-131">Type</span></span>|<span data-ttu-id="ef766-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ef766-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef766-133">actionName</span><span class="sxs-lookup"><span data-stu-id="ef766-133">actionName</span></span>|[<span data-ttu-id="ef766-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="ef766-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="ef766-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ef766-135">Not yet documented</span></span>|
|<span data-ttu-id="ef766-136">deviceIds</span><span class="sxs-lookup"><span data-stu-id="ef766-136">deviceIds</span></span>|<span data-ttu-id="ef766-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ef766-137">String collection</span></span>|<span data-ttu-id="ef766-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ef766-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ef766-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef766-139">Response</span></span>
<span data-ttu-id="ef766-140">Если успешно завершена, это действие возвращает `200 OK` код ответа и [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ef766-140">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef766-141">Пример</span><span class="sxs-lookup"><span data-stu-id="ef766-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef766-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef766-142">Request</span></span>
<span data-ttu-id="ef766-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef766-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef766-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef766-144">Response</span></span>
<span data-ttu-id="ef766-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ef766-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




