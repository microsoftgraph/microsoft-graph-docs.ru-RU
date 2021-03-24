---
title: Get deviceHealthScriptDeviceState
description: Чтение свойств и связей объекта deviceHealthScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 395a160ad3ef0416e57dc43cefc98a9901dc07da
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130688"
---
# <a name="get-devicehealthscriptdevicestate"></a><span data-ttu-id="4f78f-103">Get deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="4f78f-103">Get deviceHealthScriptDeviceState</span></span>

<span data-ttu-id="4f78f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f78f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f78f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f78f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f78f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f78f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f78f-107">Чтение свойств и связей [объекта deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="4f78f-107">Read properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f78f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f78f-108">Prerequisites</span></span>
<span data-ttu-id="4f78f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f78f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f78f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f78f-111">Permission type</span></span>|<span data-ttu-id="4f78f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f78f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f78f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f78f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f78f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f78f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f78f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f78f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f78f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f78f-116">Not supported.</span></span>|
|<span data-ttu-id="4f78f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f78f-117">Application</span></span>|<span data-ttu-id="4f78f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f78f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f78f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f78f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f78f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f78f-120">Optional query parameters</span></span>
<span data-ttu-id="4f78f-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f78f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f78f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f78f-122">Request headers</span></span>
|<span data-ttu-id="4f78f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f78f-123">Header</span></span>|<span data-ttu-id="4f78f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4f78f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f78f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f78f-125">Authorization</span></span>|<span data-ttu-id="4f78f-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f78f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f78f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4f78f-127">Accept</span></span>|<span data-ttu-id="4f78f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4f78f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f78f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f78f-129">Request body</span></span>
<span data-ttu-id="4f78f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f78f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f78f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f78f-131">Response</span></span>
<span data-ttu-id="4f78f-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4f78f-132">If successful, this method returns a `200 OK` response code and [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f78f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4f78f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f78f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f78f-134">Request</span></span>
<span data-ttu-id="4f78f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f78f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="4f78f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f78f-136">Response</span></span>
<span data-ttu-id="4f78f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f78f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




