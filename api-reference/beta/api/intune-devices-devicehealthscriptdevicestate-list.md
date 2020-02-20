---
title: Список Девицехеалсскриптдевицестатес
description: Список свойств и связей объектов Девицехеалсскриптдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 061d8d2b4096a27403a368b28e27b53772807424
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162122"
---
# <a name="list-devicehealthscriptdevicestates"></a><span data-ttu-id="7b3f5-103">Список Девицехеалсскриптдевицестатес</span><span class="sxs-lookup"><span data-stu-id="7b3f5-103">List deviceHealthScriptDeviceStates</span></span>

> <span data-ttu-id="7b3f5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b3f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b3f5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b3f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b3f5-106">Список свойств и связей объектов [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="7b3f5-106">List properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b3f5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7b3f5-107">Prerequisites</span></span>
<span data-ttu-id="7b3f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b3f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b3f5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b3f5-110">Permission type</span></span>|<span data-ttu-id="7b3f5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b3f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b3f5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b3f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7b3f5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b3f5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7b3f5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b3f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b3f5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b3f5-115">Not supported.</span></span>|
|<span data-ttu-id="7b3f5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b3f5-116">Application</span></span>|<span data-ttu-id="7b3f5-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b3f5-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b3f5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b3f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="7b3f5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7b3f5-119">Request headers</span></span>
|<span data-ttu-id="7b3f5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b3f5-120">Header</span></span>|<span data-ttu-id="7b3f5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7b3f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b3f5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b3f5-122">Authorization</span></span>|<span data-ttu-id="7b3f5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b3f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b3f5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7b3f5-124">Accept</span></span>|<span data-ttu-id="7b3f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7b3f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b3f5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b3f5-126">Request body</span></span>
<span data-ttu-id="7b3f5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b3f5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b3f5-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b3f5-128">Response</span></span>
<span data-ttu-id="7b3f5-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b3f5-129">If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b3f5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7b3f5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b3f5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b3f5-131">Request</span></span>
<span data-ttu-id="7b3f5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b3f5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="7b3f5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b3f5-133">Response</span></span>
<span data-ttu-id="7b3f5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b3f5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 892

{
  "value": [
    {
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
  ]
}
```





