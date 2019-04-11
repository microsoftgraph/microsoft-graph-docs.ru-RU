---
title: Действие executeAction
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12fe1e0974fbbc9e2ae673a10fac20df0de2533f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806680"
---
# <a name="executeaction-action"></a><span data-ttu-id="b958b-103">Действие executeAction</span><span class="sxs-lookup"><span data-stu-id="b958b-103">executeAction action</span></span>

> <span data-ttu-id="b958b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b958b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b958b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b958b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b958b-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b958b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b958b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b958b-107">Prerequisites</span></span>
<span data-ttu-id="b958b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b958b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b958b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b958b-110">Permission type</span></span>|<span data-ttu-id="b958b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b958b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b958b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b958b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b958b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b958b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="b958b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b958b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b958b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b958b-115">Not supported.</span></span>|
|<span data-ttu-id="b958b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b958b-116">Application</span></span>|<span data-ttu-id="b958b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b958b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b958b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b958b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="b958b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b958b-119">Request headers</span></span>
|<span data-ttu-id="b958b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b958b-120">Header</span></span>|<span data-ttu-id="b958b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b958b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b958b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b958b-122">Authorization</span></span>|<span data-ttu-id="b958b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b958b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b958b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b958b-124">Accept</span></span>|<span data-ttu-id="b958b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b958b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b958b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b958b-126">Request body</span></span>
<span data-ttu-id="b958b-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b958b-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b958b-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b958b-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b958b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b958b-129">Property</span></span>|<span data-ttu-id="b958b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b958b-130">Type</span></span>|<span data-ttu-id="b958b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b958b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b958b-132">actionName</span><span class="sxs-lookup"><span data-stu-id="b958b-132">actionName</span></span>|[<span data-ttu-id="b958b-133">Манажеддевицеремотеактион</span><span class="sxs-lookup"><span data-stu-id="b958b-133">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="b958b-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b958b-134">Not yet documented</span></span>|
|<span data-ttu-id="b958b-135">Девицеидс</span><span class="sxs-lookup"><span data-stu-id="b958b-135">deviceIds</span></span>|<span data-ttu-id="b958b-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b958b-136">String collection</span></span>|<span data-ttu-id="b958b-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b958b-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b958b-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="b958b-138">Response</span></span>
<span data-ttu-id="b958b-139">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [булкманажеддевицеактионресулт](../resources/intune-devices-bulkmanageddeviceactionresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b958b-139">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b958b-140">Пример</span><span class="sxs-lookup"><span data-stu-id="b958b-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b958b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b958b-141">Request</span></span>
<span data-ttu-id="b958b-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b958b-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/executeAction

Content-type: application/json
Content-length: 78

{
  "actionName": "delete",
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b958b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b958b-143">Response</span></span>
<span data-ttu-id="b958b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b958b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





