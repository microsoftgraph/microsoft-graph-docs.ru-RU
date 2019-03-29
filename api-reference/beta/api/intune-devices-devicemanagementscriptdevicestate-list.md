---
title: Список Девицеманажементскриптдевицестатес
description: Список свойств и связей объектов Девицеманажементскриптдевицестате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35f649d022694b7943153fd592aba2b3694b73d2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973595"
---
# <a name="list-devicemanagementscriptdevicestates"></a><span data-ttu-id="078bc-103">Список Девицеманажементскриптдевицестатес</span><span class="sxs-lookup"><span data-stu-id="078bc-103">List deviceManagementScriptDeviceStates</span></span>

> <span data-ttu-id="078bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="078bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="078bc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="078bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="078bc-106">Список свойств и связей объектов [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="078bc-106">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="078bc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="078bc-107">Prerequisites</span></span>
<span data-ttu-id="078bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="078bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="078bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="078bc-110">Permission type</span></span>|<span data-ttu-id="078bc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="078bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="078bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="078bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="078bc-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="078bc-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="078bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="078bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="078bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="078bc-115">Not supported.</span></span>|
|<span data-ttu-id="078bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="078bc-116">Application</span></span>|<span data-ttu-id="078bc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="078bc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="078bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="078bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="078bc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="078bc-119">Request headers</span></span>
|<span data-ttu-id="078bc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="078bc-120">Header</span></span>|<span data-ttu-id="078bc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="078bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="078bc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="078bc-122">Authorization</span></span>|<span data-ttu-id="078bc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="078bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="078bc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="078bc-124">Accept</span></span>|<span data-ttu-id="078bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="078bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="078bc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="078bc-126">Request body</span></span>
<span data-ttu-id="078bc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="078bc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="078bc-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="078bc-128">Response</span></span>
<span data-ttu-id="078bc-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="078bc-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="078bc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="078bc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="078bc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="078bc-131">Request</span></span>
<span data-ttu-id="078bc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="078bc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="078bc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="078bc-133">Response</span></span>
<span data-ttu-id="078bc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="078bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
      "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
      "runState": "success",
      "resultMessage": "Result Message value",
      "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
      "errorCode": 9,
      "errorDescription": "Error Description value"
    }
  ]
}
```




