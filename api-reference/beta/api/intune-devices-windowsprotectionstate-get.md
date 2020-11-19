---
title: Получение windowsProtectionState
description: Чтение свойств и связей объекта windowsProtectionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 814965ef400e42cf941873c79b09266ffb8c855f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49218644"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="ba1f2-103">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="ba1f2-103">Get windowsProtectionState</span></span>

<span data-ttu-id="ba1f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba1f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba1f2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba1f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba1f2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba1f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba1f2-107">Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="ba1f2-107">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba1f2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ba1f2-108">Prerequisites</span></span>
<span data-ttu-id="ba1f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba1f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba1f2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba1f2-111">Permission type</span></span>|<span data-ttu-id="ba1f2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba1f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba1f2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba1f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba1f2-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba1f2-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ba1f2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba1f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba1f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba1f2-116">Not supported.</span></span>|
|<span data-ttu-id="ba1f2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ba1f2-117">Application</span></span>|<span data-ttu-id="ba1f2-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba1f2-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba1f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba1f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba1f2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba1f2-120">Optional query parameters</span></span>
<span data-ttu-id="ba1f2-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ba1f2-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba1f2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba1f2-122">Request headers</span></span>
|<span data-ttu-id="ba1f2-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba1f2-123">Header</span></span>|<span data-ttu-id="ba1f2-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ba1f2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba1f2-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba1f2-125">Authorization</span></span>|<span data-ttu-id="ba1f2-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba1f2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba1f2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ba1f2-127">Accept</span></span>|<span data-ttu-id="ba1f2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ba1f2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba1f2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba1f2-129">Request body</span></span>
<span data-ttu-id="ba1f2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba1f2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba1f2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba1f2-131">Response</span></span>
<span data-ttu-id="ba1f2-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba1f2-132">If successful, this method returns a `200 OK` response code and [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba1f2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ba1f2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba1f2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba1f2-134">Request</span></span>
<span data-ttu-id="ba1f2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba1f2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

### <a name="response"></a><span data-ttu-id="ba1f2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba1f2-136">Response</span></span>
<span data-ttu-id="ba1f2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba1f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1083

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsProtectionState",
    "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
    "malwareProtectionEnabled": true,
    "deviceState": "fullScanPending",
    "realTimeProtectionEnabled": true,
    "networkInspectionSystemEnabled": true,
    "quickScanOverdue": true,
    "fullScanOverdue": true,
    "signatureUpdateOverdue": true,
    "rebootRequired": true,
    "fullScanRequired": true,
    "engineVersion": "Engine Version value",
    "signatureVersion": "Signature Version value",
    "antiMalwareVersion": "Anti Malware Version value",
    "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
    "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
    "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
    "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "productStatus": "serviceNotRunning",
    "isVirtualMachine": true,
    "tamperProtectionEnabled": true
  }
}
```




