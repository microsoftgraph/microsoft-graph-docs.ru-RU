---
title: действие Креатедевицелогколлектионрекуест
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 15deac0383992f2045599aff34d097c3555be7f0
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124301"
---
# <a name="createdevicelogcollectionrequest-action"></a><span data-ttu-id="c332a-103">действие Креатедевицелогколлектионрекуест</span><span class="sxs-lookup"><span data-stu-id="c332a-103">createDeviceLogCollectionRequest action</span></span>

<span data-ttu-id="c332a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c332a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c332a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c332a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c332a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c332a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c332a-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c332a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c332a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c332a-108">Prerequisites</span></span>
<span data-ttu-id="c332a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c332a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c332a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c332a-111">Permission type</span></span>|<span data-ttu-id="c332a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c332a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c332a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c332a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c332a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c332a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c332a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c332a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c332a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c332a-116">Not supported.</span></span>|
|<span data-ttu-id="c332a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c332a-117">Application</span></span>|<span data-ttu-id="c332a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c332a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c332a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c332a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/comanagedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
```

## <a name="request-headers"></a><span data-ttu-id="c332a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c332a-120">Request headers</span></span>
|<span data-ttu-id="c332a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c332a-121">Header</span></span>|<span data-ttu-id="c332a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c332a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c332a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c332a-123">Authorization</span></span>|<span data-ttu-id="c332a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c332a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c332a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c332a-125">Accept</span></span>|<span data-ttu-id="c332a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c332a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c332a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c332a-127">Request body</span></span>
<span data-ttu-id="c332a-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c332a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c332a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c332a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c332a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c332a-130">Property</span></span>|<span data-ttu-id="c332a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c332a-131">Type</span></span>|<span data-ttu-id="c332a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c332a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c332a-133">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="c332a-133">templateType</span></span>|[<span data-ttu-id="c332a-134">девицелогколлектионрекуест</span><span class="sxs-lookup"><span data-stu-id="c332a-134">deviceLogCollectionRequest</span></span>](../resources/intune-devices-devicelogcollectionrequest.md)|<span data-ttu-id="c332a-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c332a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c332a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c332a-136">Response</span></span>
<span data-ttu-id="c332a-137">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c332a-137">If successful, this action returns a `200 OK` response code and a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c332a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c332a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c332a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c332a-139">Request</span></span>
<span data-ttu-id="c332a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c332a-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest

Content-type: application/json
Content-length: 153

{
  "templateType": {
    "@odata.type": "microsoft.graph.deviceLogCollectionRequest",
    "id": "Id value",
    "templateType": "predefined"
  }
}
```

### <a name="response"></a><span data-ttu-id="c332a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c332a-141">Response</span></span>
<span data-ttu-id="c332a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c332a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
    "id": "05fb97dc-97dc-05fb-dc97-fb05dc97fb05",
    "status": "Status value",
    "managedDeviceId": "3b336f00-6f00-3b33-006f-333b006f333b",
    "errorCode": 9,
    "requestedDateTimeUTC": "2016-12-31T23:57:40.7845755-08:00",
    "receivedDateTimeUTC": "2016-12-31T23:59:48.6545758-08:00",
    "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
    "expirationDateTimeUTC": "2017-01-01T00:02:49.2157996-08:00",
    "size": 1.3333333333333333
  }
}
```



