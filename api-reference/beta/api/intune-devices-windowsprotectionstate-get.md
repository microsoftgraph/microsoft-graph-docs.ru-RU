---
title: Получение windowsProtectionState
description: Чтение свойств и связей объекта windowsProtectionState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35fb6f7c57e3d526db0a4dfeb4e9639d5c329597
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790090"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="7e2a2-103">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="7e2a2-103">Get windowsProtectionState</span></span>

> <span data-ttu-id="7e2a2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e2a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e2a2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e2a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e2a2-106">Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="7e2a2-106">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e2a2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7e2a2-107">Prerequisites</span></span>
<span data-ttu-id="7e2a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e2a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e2a2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e2a2-110">Permission type</span></span>|<span data-ttu-id="7e2a2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e2a2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e2a2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e2a2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e2a2-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e2a2-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7e2a2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e2a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e2a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e2a2-115">Not supported.</span></span>|
|<span data-ttu-id="7e2a2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e2a2-116">Application</span></span>|<span data-ttu-id="7e2a2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e2a2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e2a2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e2a2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e2a2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7e2a2-119">Optional query parameters</span></span>
<span data-ttu-id="7e2a2-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7e2a2-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e2a2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e2a2-121">Request headers</span></span>
|<span data-ttu-id="7e2a2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e2a2-122">Header</span></span>|<span data-ttu-id="7e2a2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7e2a2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e2a2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e2a2-124">Authorization</span></span>|<span data-ttu-id="7e2a2-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e2a2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e2a2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7e2a2-126">Accept</span></span>|<span data-ttu-id="7e2a2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7e2a2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e2a2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e2a2-128">Request body</span></span>
<span data-ttu-id="7e2a2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e2a2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e2a2-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e2a2-130">Response</span></span>
<span data-ttu-id="7e2a2-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e2a2-131">If successful, this method returns a `200 OK` response code and [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e2a2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7e2a2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e2a2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e2a2-133">Request</span></span>
<span data-ttu-id="7e2a2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e2a2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
```

### <a name="response"></a><span data-ttu-id="7e2a2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e2a2-135">Response</span></span>
<span data-ttu-id="7e2a2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e2a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 971

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
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
  }
}
```





