---
title: Обновление Девицелогколлектионреспонсе
description: Обновление свойств объекта Девицелогколлектионреспонсе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6dade84eeb03fbfedc846d6ef7740579146fff8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696841"
---
# <a name="update-devicelogcollectionresponse"></a><span data-ttu-id="8c8ca-103">Обновление Девицелогколлектионреспонсе</span><span class="sxs-lookup"><span data-stu-id="8c8ca-103">Update deviceLogCollectionResponse</span></span>

<span data-ttu-id="8c8ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c8ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c8ca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c8ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c8ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c8ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c8ca-107">Обновление свойств объекта [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="8c8ca-107">Update the properties of a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c8ca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8c8ca-108">Prerequisites</span></span>
<span data-ttu-id="8c8ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c8ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c8ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c8ca-111">Permission type</span></span>|<span data-ttu-id="8c8ca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c8ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c8ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c8ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c8ca-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c8ca-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8c8ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c8ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c8ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c8ca-116">Not supported.</span></span>|
|<span data-ttu-id="8c8ca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c8ca-117">Application</span></span>|<span data-ttu-id="8c8ca-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c8ca-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c8ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c8ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

## <a name="request-headers"></a><span data-ttu-id="8c8ca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8c8ca-120">Request headers</span></span>
|<span data-ttu-id="8c8ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c8ca-121">Header</span></span>|<span data-ttu-id="8c8ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8c8ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c8ca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c8ca-123">Authorization</span></span>|<span data-ttu-id="8c8ca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c8ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c8ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c8ca-125">Accept</span></span>|<span data-ttu-id="8c8ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c8ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c8ca-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c8ca-127">Request body</span></span>
<span data-ttu-id="8c8ca-128">В тексте запроса добавьте представление объекта [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c8ca-128">In the request body, supply a JSON representation for the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

<span data-ttu-id="8c8ca-129">В следующей таблице приведены свойства, необходимые при создании [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md).</span><span class="sxs-lookup"><span data-stu-id="8c8ca-129">The following table shows the properties that are required when you create the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md).</span></span>

|<span data-ttu-id="8c8ca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c8ca-130">Property</span></span>|<span data-ttu-id="8c8ca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8c8ca-131">Type</span></span>|<span data-ttu-id="8c8ca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c8ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c8ca-133">id</span><span class="sxs-lookup"><span data-stu-id="8c8ca-133">id</span></span>|<span data-ttu-id="8c8ca-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8c8ca-134">String</span></span>|<span data-ttu-id="8c8ca-135">Уникальный идентификатор в виде tenantId_deviceId_requestId</span><span class="sxs-lookup"><span data-stu-id="8c8ca-135">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="8c8ca-136">status</span><span class="sxs-lookup"><span data-stu-id="8c8ca-136">status</span></span>|<span data-ttu-id="8c8ca-137">String</span><span class="sxs-lookup"><span data-stu-id="8c8ca-137">String</span></span>|<span data-ttu-id="8c8ca-138">Состояние запроса на сбор журналов</span><span class="sxs-lookup"><span data-stu-id="8c8ca-138">The status of the log collection request</span></span>|
|<span data-ttu-id="8c8ca-139">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="8c8ca-139">managedDeviceId</span></span>|<span data-ttu-id="8c8ca-140">Guid</span><span class="sxs-lookup"><span data-stu-id="8c8ca-140">Guid</span></span>|<span data-ttu-id="8c8ca-141">Идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="8c8ca-141">The device Id</span></span>|
|<span data-ttu-id="8c8ca-142">errorCode</span><span class="sxs-lookup"><span data-stu-id="8c8ca-142">errorCode</span></span>|<span data-ttu-id="8c8ca-143">Int64</span><span class="sxs-lookup"><span data-stu-id="8c8ca-143">Int64</span></span>|<span data-ttu-id="8c8ca-144">Код ошибки (при наличии).</span><span class="sxs-lookup"><span data-stu-id="8c8ca-144">The error code, if any.</span></span> <span data-ttu-id="8c8ca-145">Допустимые значения — 9.22337203685478 E + 18 — 9.22337203685478 E + 18</span><span class="sxs-lookup"><span data-stu-id="8c8ca-145">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="8c8ca-146">рекуестеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="8c8ca-146">requestedDateTimeUTC</span></span>|<span data-ttu-id="8c8ca-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c8ca-147">DateTimeOffset</span></span>|<span data-ttu-id="8c8ca-148">Дата и время запроса</span><span class="sxs-lookup"><span data-stu-id="8c8ca-148">The DateTime of the request</span></span>|
|<span data-ttu-id="8c8ca-149">рецеиведдатетимеутк</span><span class="sxs-lookup"><span data-stu-id="8c8ca-149">receivedDateTimeUTC</span></span>|<span data-ttu-id="8c8ca-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c8ca-150">DateTimeOffset</span></span>|<span data-ttu-id="8c8ca-151">Дата и время получения запроса</span><span class="sxs-lookup"><span data-stu-id="8c8ca-151">The DateTime the request was received</span></span>|
|<span data-ttu-id="8c8ca-152">Свойства initiatedbyuserprincipalname</span><span class="sxs-lookup"><span data-stu-id="8c8ca-152">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="8c8ca-153">Строка</span><span class="sxs-lookup"><span data-stu-id="8c8ca-153">String</span></span>|<span data-ttu-id="8c8ca-154">Имя участника-пользователя, который инициировал запрос.</span><span class="sxs-lookup"><span data-stu-id="8c8ca-154">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="8c8ca-155">експиратиондатетимеутк</span><span class="sxs-lookup"><span data-stu-id="8c8ca-155">expirationDateTimeUTC</span></span>|<span data-ttu-id="8c8ca-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c8ca-156">DateTimeOffset</span></span>|<span data-ttu-id="8c8ca-157">Дата и время истечения срока действия журналов</span><span class="sxs-lookup"><span data-stu-id="8c8ca-157">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="8c8ca-158">size</span><span class="sxs-lookup"><span data-stu-id="8c8ca-158">size</span></span>|<span data-ttu-id="8c8ca-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8c8ca-159">Double</span></span>|<span data-ttu-id="8c8ca-160">Размер журналов.</span><span class="sxs-lookup"><span data-stu-id="8c8ca-160">The size of the logs.</span></span> <span data-ttu-id="8c8ca-161">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="8c8ca-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="8c8ca-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c8ca-162">Response</span></span>
<span data-ttu-id="8c8ca-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c8ca-163">If successful, this method returns a `200 OK` response code and an updated [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c8ca-164">Пример</span><span class="sxs-lookup"><span data-stu-id="8c8ca-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c8ca-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c8ca-165">Request</span></span>
<span data-ttu-id="8c8ca-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c8ca-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
Content-type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "status": "Status value",
  "managedDeviceId": "3b336f00-6f00-3b33-006f-333b006f333b",
  "errorCode": 9,
  "requestedDateTimeUTC": "2016-12-31T23:57:40.7845755-08:00",
  "receivedDateTimeUTC": "2016-12-31T23:59:48.6545758-08:00",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "expirationDateTimeUTC": "2017-01-01T00:02:49.2157996-08:00",
  "size": 1.3333333333333333
}
```

### <a name="response"></a><span data-ttu-id="8c8ca-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c8ca-167">Response</span></span>
<span data-ttu-id="8c8ca-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c8ca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 528

{
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
```





