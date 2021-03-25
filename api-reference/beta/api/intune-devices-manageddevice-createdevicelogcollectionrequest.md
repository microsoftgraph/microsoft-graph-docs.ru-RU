---
title: createDeviceLogCollectionRequest action
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb303df2b0590d1986b7853992a2c2aa2c741573
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150117"
---
# <a name="createdevicelogcollectionrequest-action"></a><span data-ttu-id="45d1a-103">createDeviceLogCollectionRequest action</span><span class="sxs-lookup"><span data-stu-id="45d1a-103">createDeviceLogCollectionRequest action</span></span>

<span data-ttu-id="45d1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45d1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45d1a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45d1a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45d1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45d1a-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="45d1a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45d1a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="45d1a-108">Prerequisites</span></span>
<span data-ttu-id="45d1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45d1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45d1a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45d1a-111">Permission type</span></span>|<span data-ttu-id="45d1a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45d1a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45d1a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45d1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45d1a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45d1a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="45d1a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45d1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45d1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d1a-116">Not supported.</span></span>|
|<span data-ttu-id="45d1a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="45d1a-117">Application</span></span>|<span data-ttu-id="45d1a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45d1a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45d1a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45d1a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="45d1a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45d1a-120">Request headers</span></span>
|<span data-ttu-id="45d1a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45d1a-121">Header</span></span>|<span data-ttu-id="45d1a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45d1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45d1a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45d1a-123">Authorization</span></span>|<span data-ttu-id="45d1a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45d1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45d1a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45d1a-125">Accept</span></span>|<span data-ttu-id="45d1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45d1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45d1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45d1a-127">Request body</span></span>
<span data-ttu-id="45d1a-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45d1a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="45d1a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="45d1a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="45d1a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="45d1a-130">Property</span></span>|<span data-ttu-id="45d1a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="45d1a-131">Type</span></span>|<span data-ttu-id="45d1a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="45d1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45d1a-133">templateType</span><span class="sxs-lookup"><span data-stu-id="45d1a-133">templateType</span></span>|[<span data-ttu-id="45d1a-134">deviceLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="45d1a-134">deviceLogCollectionRequest</span></span>](../resources/intune-devices-devicelogcollectionrequest.md)|<span data-ttu-id="45d1a-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="45d1a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="45d1a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="45d1a-136">Response</span></span>
<span data-ttu-id="45d1a-137">В случае успеха это действие возвращает код отклика и `200 OK` [устройствоLogCollectionResponse в](../resources/intune-devices-devicelogcollectionresponse.md) тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="45d1a-137">If successful, this action returns a `200 OK` response code and a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45d1a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="45d1a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="45d1a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="45d1a-139">Request</span></span>
<span data-ttu-id="45d1a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45d1a-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45d1a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="45d1a-141">Response</span></span>
<span data-ttu-id="45d1a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45d1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




