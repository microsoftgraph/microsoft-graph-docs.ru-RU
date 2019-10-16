---
title: Получение Девицехеалсскриптдевицестате
description: Чтение свойств и связей объекта Девицехеалсскриптдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89ecc8374e7b71926164a63ddaf3075150d92146
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37531324"
---
# <a name="get-devicehealthscriptdevicestate"></a><span data-ttu-id="6e9ed-103">Получение Девицехеалсскриптдевицестате</span><span class="sxs-lookup"><span data-stu-id="6e9ed-103">Get deviceHealthScriptDeviceState</span></span>

> <span data-ttu-id="6e9ed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e9ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e9ed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e9ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e9ed-106">Чтение свойств и связей объекта [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="6e9ed-106">Read properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e9ed-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6e9ed-107">Prerequisites</span></span>
<span data-ttu-id="6e9ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e9ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e9ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e9ed-110">Permission type</span></span>|<span data-ttu-id="6e9ed-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e9ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e9ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e9ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e9ed-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e9ed-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6e9ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e9ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e9ed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e9ed-115">Not supported.</span></span>|
|<span data-ttu-id="6e9ed-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6e9ed-116">Application</span></span>|<span data-ttu-id="6e9ed-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e9ed-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e9ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e9ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e9ed-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6e9ed-119">Optional query parameters</span></span>
<span data-ttu-id="6e9ed-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6e9ed-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e9ed-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e9ed-121">Request headers</span></span>
|<span data-ttu-id="6e9ed-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e9ed-122">Header</span></span>|<span data-ttu-id="6e9ed-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6e9ed-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e9ed-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e9ed-124">Authorization</span></span>|<span data-ttu-id="6e9ed-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e9ed-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e9ed-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6e9ed-126">Accept</span></span>|<span data-ttu-id="6e9ed-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6e9ed-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e9ed-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e9ed-128">Request body</span></span>
<span data-ttu-id="6e9ed-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e9ed-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e9ed-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e9ed-130">Response</span></span>
<span data-ttu-id="6e9ed-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6e9ed-131">If successful, this method returns a `200 OK` response code and [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e9ed-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6e9ed-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e9ed-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e9ed-133">Request</span></span>
<span data-ttu-id="6e9ed-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e9ed-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="6e9ed-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e9ed-135">Response</span></span>
<span data-ttu-id="6e9ed-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e9ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
    "id": "fd2e4505-4505-fd2e-0545-2efd05452efd",
    "detectionState": "success",
    "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
    "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
    "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
    "remediationScriptError": "Remediation Script Error value",
    "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
    "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
    "remediationState": "skipped"
  }
}
```






