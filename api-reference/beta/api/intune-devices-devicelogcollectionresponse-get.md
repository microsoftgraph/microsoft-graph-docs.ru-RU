---
title: Получение Девицелогколлектионреспонсе
description: Чтение свойств и связей объекта Девицелогколлектионреспонсе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1cb0b477e3d6885cbdd359145b99ce03d4914e32
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732813"
---
# <a name="get-devicelogcollectionresponse"></a><span data-ttu-id="6a941-103">Получение Девицелогколлектионреспонсе</span><span class="sxs-lookup"><span data-stu-id="6a941-103">Get deviceLogCollectionResponse</span></span>

<span data-ttu-id="6a941-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a941-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a941-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a941-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a941-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a941-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a941-107">Чтение свойств и связей объекта [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="6a941-107">Read properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a941-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6a941-108">Prerequisites</span></span>
<span data-ttu-id="6a941-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a941-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a941-111">Permission type</span></span>|<span data-ttu-id="6a941-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a941-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a941-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a941-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a941-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a941-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6a941-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a941-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a941-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a941-116">Not supported.</span></span>|
|<span data-ttu-id="6a941-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a941-117">Application</span></span>|<span data-ttu-id="6a941-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a941-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a941-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a941-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a941-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6a941-120">Optional query parameters</span></span>
<span data-ttu-id="6a941-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6a941-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a941-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a941-122">Request headers</span></span>
|<span data-ttu-id="6a941-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a941-123">Header</span></span>|<span data-ttu-id="6a941-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6a941-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a941-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a941-125">Authorization</span></span>|<span data-ttu-id="6a941-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a941-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a941-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6a941-127">Accept</span></span>|<span data-ttu-id="6a941-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6a941-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a941-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6a941-129">Request body</span></span>
<span data-ttu-id="6a941-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a941-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a941-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a941-131">Response</span></span>
<span data-ttu-id="6a941-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a941-132">If successful, this method returns a `200 OK` response code and [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a941-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6a941-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a941-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a941-134">Request</span></span>
<span data-ttu-id="6a941-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a941-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

### <a name="response"></a><span data-ttu-id="6a941-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a941-136">Response</span></span>
<span data-ttu-id="6a941-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a941-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





