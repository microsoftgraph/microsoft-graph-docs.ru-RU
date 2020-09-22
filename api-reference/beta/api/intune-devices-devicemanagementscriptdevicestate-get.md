---
title: Получение Девицеманажементскриптдевицестате
description: Чтение свойств и связей объекта Девицеманажементскриптдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f22d0a19615eec4d6d05a0d99a1a21f41019f23
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036599"
---
# <a name="get-devicemanagementscriptdevicestate"></a><span data-ttu-id="cc0be-103">Получение Девицеманажементскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="cc0be-103">Get deviceManagementScriptDeviceState</span></span>

<span data-ttu-id="cc0be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc0be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc0be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc0be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc0be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc0be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc0be-107">Чтение свойств и связей объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="cc0be-107">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc0be-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cc0be-108">Prerequisites</span></span>
<span data-ttu-id="cc0be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc0be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc0be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc0be-111">Permission type</span></span>|<span data-ttu-id="cc0be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc0be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc0be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc0be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc0be-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc0be-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cc0be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc0be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc0be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc0be-116">Not supported.</span></span>|
|<span data-ttu-id="cc0be-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc0be-117">Application</span></span>|<span data-ttu-id="cc0be-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc0be-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc0be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc0be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc0be-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cc0be-120">Optional query parameters</span></span>
<span data-ttu-id="cc0be-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cc0be-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc0be-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc0be-122">Request headers</span></span>
|<span data-ttu-id="cc0be-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc0be-123">Header</span></span>|<span data-ttu-id="cc0be-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cc0be-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc0be-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc0be-125">Authorization</span></span>|<span data-ttu-id="cc0be-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc0be-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc0be-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cc0be-127">Accept</span></span>|<span data-ttu-id="cc0be-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cc0be-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc0be-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc0be-129">Request body</span></span>
<span data-ttu-id="cc0be-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc0be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc0be-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc0be-131">Response</span></span>
<span data-ttu-id="cc0be-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc0be-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc0be-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cc0be-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc0be-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc0be-134">Request</span></span>
<span data-ttu-id="cc0be-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc0be-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="cc0be-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc0be-136">Response</span></span>
<span data-ttu-id="cc0be-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc0be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
    "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
    "runState": "success",
    "resultMessage": "Result Message value",
    "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
    "errorCode": 9,
    "errorDescription": "Error Description value"
  }
}
```






