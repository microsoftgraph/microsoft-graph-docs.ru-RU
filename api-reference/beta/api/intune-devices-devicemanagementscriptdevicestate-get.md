---
title: Получение Девицеманажементскриптдевицестате
description: Чтение свойств и связей объекта Девицеманажементскриптдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9135e1e185f4c3e4b6c8b06743b93f6d6d6ed7b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731787"
---
# <a name="get-devicemanagementscriptdevicestate"></a><span data-ttu-id="910f0-103">Получение Девицеманажементскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="910f0-103">Get deviceManagementScriptDeviceState</span></span>

<span data-ttu-id="910f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="910f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="910f0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="910f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="910f0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="910f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="910f0-107">Чтение свойств и связей объекта [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="910f0-107">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="910f0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="910f0-108">Prerequisites</span></span>
<span data-ttu-id="910f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="910f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="910f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="910f0-111">Permission type</span></span>|<span data-ttu-id="910f0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="910f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="910f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="910f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="910f0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="910f0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="910f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="910f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="910f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="910f0-116">Not supported.</span></span>|
|<span data-ttu-id="910f0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="910f0-117">Application</span></span>|<span data-ttu-id="910f0-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="910f0-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="910f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="910f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="910f0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="910f0-120">Optional query parameters</span></span>
<span data-ttu-id="910f0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="910f0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="910f0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="910f0-122">Request headers</span></span>
|<span data-ttu-id="910f0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="910f0-123">Header</span></span>|<span data-ttu-id="910f0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="910f0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="910f0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="910f0-125">Authorization</span></span>|<span data-ttu-id="910f0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="910f0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="910f0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="910f0-127">Accept</span></span>|<span data-ttu-id="910f0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="910f0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="910f0-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="910f0-129">Request body</span></span>
<span data-ttu-id="910f0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="910f0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="910f0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="910f0-131">Response</span></span>
<span data-ttu-id="910f0-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="910f0-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="910f0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="910f0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="910f0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="910f0-134">Request</span></span>
<span data-ttu-id="910f0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="910f0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="910f0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="910f0-136">Response</span></span>
<span data-ttu-id="910f0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="910f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





