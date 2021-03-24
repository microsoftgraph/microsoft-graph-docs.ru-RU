---
title: Get deviceComplianceScriptDeviceState
description: Чтение свойств и связей объекта deviceComplianceScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9389ed4659b8fd29376b0803b75682267058949d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128609"
---
# <a name="get-devicecompliancescriptdevicestate"></a><span data-ttu-id="4ecab-103">Get deviceComplianceScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="4ecab-103">Get deviceComplianceScriptDeviceState</span></span>

<span data-ttu-id="4ecab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ecab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ecab-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ecab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ecab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ecab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ecab-107">Чтение свойств и связей [объекта deviceComplianceScriptDeviceState.](../resources/intune-devices-devicecompliancescriptdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="4ecab-107">Read properties and relationships of the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ecab-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ecab-108">Prerequisites</span></span>
<span data-ttu-id="4ecab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ecab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ecab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ecab-111">Permission type</span></span>|<span data-ttu-id="4ecab-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ecab-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ecab-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ecab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ecab-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ecab-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4ecab-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ecab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ecab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ecab-116">Not supported.</span></span>|
|<span data-ttu-id="4ecab-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4ecab-117">Application</span></span>|<span data-ttu-id="4ecab-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ecab-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ecab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ecab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ecab-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ecab-120">Optional query parameters</span></span>
<span data-ttu-id="4ecab-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4ecab-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ecab-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ecab-122">Request headers</span></span>
|<span data-ttu-id="4ecab-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ecab-123">Header</span></span>|<span data-ttu-id="4ecab-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4ecab-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ecab-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ecab-125">Authorization</span></span>|<span data-ttu-id="4ecab-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ecab-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ecab-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4ecab-127">Accept</span></span>|<span data-ttu-id="4ecab-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4ecab-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ecab-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ecab-129">Request body</span></span>
<span data-ttu-id="4ecab-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ecab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ecab-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ecab-131">Response</span></span>
<span data-ttu-id="4ecab-132">В случае успешного использования этот метод возвращает код отклика и `200 OK` [объект deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4ecab-132">If successful, this method returns a `200 OK` response code and [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ecab-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4ecab-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ecab-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ecab-134">Request</span></span>
<span data-ttu-id="4ecab-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ecab-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="4ecab-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ecab-136">Response</span></span>
<span data-ttu-id="4ecab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ecab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
    "id": "7bd39c86-9c86-7bd3-869c-d37b869cd37b",
    "detectionState": "success",
    "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
    "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "scriptOutput": "Script Output value",
    "scriptError": "Script Error value"
  }
}
```




