---
title: Получение Девицеманажементскриптдевицестате
description: Чтение свойств и связей объекта Девицеманажементскриптдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f4880a158dd7aaaef131f3cdf22c68d7fa36f72e
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37530491"
---
# <a name="get-devicemanagementscriptdevicestate"></a><span data-ttu-id="6dc18-103">Получение Девицеманажементскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="6dc18-103">Get deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="6dc18-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dc18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dc18-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6dc18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dc18-106">Чтение свойств и связей объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="6dc18-106">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dc18-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6dc18-107">Prerequisites</span></span>
<span data-ttu-id="6dc18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dc18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dc18-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dc18-110">Permission type</span></span>|<span data-ttu-id="6dc18-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dc18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dc18-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dc18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6dc18-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dc18-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6dc18-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dc18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dc18-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dc18-115">Not supported.</span></span>|
|<span data-ttu-id="6dc18-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6dc18-116">Application</span></span>|<span data-ttu-id="6dc18-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dc18-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dc18-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dc18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dc18-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6dc18-119">Optional query parameters</span></span>
<span data-ttu-id="6dc18-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6dc18-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dc18-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dc18-121">Request headers</span></span>
|<span data-ttu-id="6dc18-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6dc18-122">Header</span></span>|<span data-ttu-id="6dc18-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6dc18-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dc18-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dc18-124">Authorization</span></span>|<span data-ttu-id="6dc18-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dc18-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dc18-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6dc18-126">Accept</span></span>|<span data-ttu-id="6dc18-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6dc18-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dc18-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6dc18-128">Request body</span></span>
<span data-ttu-id="6dc18-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dc18-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dc18-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6dc18-130">Response</span></span>
<span data-ttu-id="6dc18-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6dc18-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dc18-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6dc18-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dc18-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dc18-133">Request</span></span>
<span data-ttu-id="6dc18-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dc18-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="6dc18-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dc18-135">Response</span></span>
<span data-ttu-id="6dc18-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6dc18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






