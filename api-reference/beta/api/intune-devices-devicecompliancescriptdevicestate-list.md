---
title: Список Девицекомплианцескриптдевицестатес
description: Список свойств и связей объектов Девицекомплианцескриптдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 167db3f083198e8f9103cff3f6237eac5bc739ff
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228934"
---
# <a name="list-devicecompliancescriptdevicestates"></a><span data-ttu-id="f4216-103">Список Девицекомплианцескриптдевицестатес</span><span class="sxs-lookup"><span data-stu-id="f4216-103">List deviceComplianceScriptDeviceStates</span></span>

<span data-ttu-id="f4216-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4216-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4216-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4216-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4216-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4216-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4216-107">Список свойств и связей объектов [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="f4216-107">List properties and relationships of the [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4216-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f4216-108">Prerequisites</span></span>
<span data-ttu-id="f4216-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4216-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4216-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4216-111">Permission type</span></span>|<span data-ttu-id="f4216-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4216-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4216-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4216-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4216-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4216-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f4216-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4216-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4216-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4216-116">Not supported.</span></span>|
|<span data-ttu-id="f4216-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f4216-117">Application</span></span>|<span data-ttu-id="f4216-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4216-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4216-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4216-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="f4216-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f4216-120">Request headers</span></span>
|<span data-ttu-id="f4216-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4216-121">Header</span></span>|<span data-ttu-id="f4216-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f4216-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4216-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4216-123">Authorization</span></span>|<span data-ttu-id="f4216-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4216-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4216-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4216-125">Accept</span></span>|<span data-ttu-id="f4216-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4216-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4216-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4216-127">Request body</span></span>
<span data-ttu-id="f4216-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4216-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4216-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4216-129">Response</span></span>
<span data-ttu-id="f4216-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4216-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4216-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f4216-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4216-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4216-132">Request</span></span>
<span data-ttu-id="f4216-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4216-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="f4216-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4216-134">Response</span></span>
<span data-ttu-id="f4216-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4216-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 501

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScriptDeviceState",
      "id": "7bd39c86-9c86-7bd3-869c-d37b869cd37b",
      "detectionState": "success",
      "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
      "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "scriptOutput": "Script Output value",
      "scriptError": "Script Error value"
    }
  ]
}
```




