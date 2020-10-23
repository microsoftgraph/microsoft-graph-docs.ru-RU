---
title: Создание Девицелогколлектионреспонсе
description: Создание нового объекта Девицелогколлектионреспонсе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e39cf4af0af0ad183b262d524429bc52a2122cb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693250"
---
# <a name="create-devicelogcollectionresponse"></a><span data-ttu-id="52764-103">Создание Девицелогколлектионреспонсе</span><span class="sxs-lookup"><span data-stu-id="52764-103">Create deviceLogCollectionResponse</span></span>

<span data-ttu-id="52764-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52764-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52764-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52764-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52764-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52764-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52764-107">Создание нового объекта [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="52764-107">Create a new [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52764-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="52764-108">Prerequisites</span></span>
<span data-ttu-id="52764-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52764-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52764-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52764-111">Permission type</span></span>|<span data-ttu-id="52764-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52764-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52764-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52764-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52764-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52764-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="52764-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52764-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52764-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52764-116">Not supported.</span></span>|
|<span data-ttu-id="52764-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52764-117">Application</span></span>|<span data-ttu-id="52764-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52764-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52764-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52764-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="52764-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="52764-120">Request headers</span></span>
|<span data-ttu-id="52764-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52764-121">Header</span></span>|<span data-ttu-id="52764-122">Значение</span><span class="sxs-lookup"><span data-stu-id="52764-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52764-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52764-123">Authorization</span></span>|<span data-ttu-id="52764-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52764-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52764-125">Accept</span><span class="sxs-lookup"><span data-stu-id="52764-125">Accept</span></span>|<span data-ttu-id="52764-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52764-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52764-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="52764-127">Request body</span></span>
<span data-ttu-id="52764-128">В тексте запроса добавьте представление объекта Девицелогколлектионреспонсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52764-128">In the request body, supply a JSON representation for the deviceLogCollectionResponse object.</span></span>

<span data-ttu-id="52764-129">В следующей таблице приведены свойства, необходимые при создании Девицелогколлектионреспонсе.</span><span class="sxs-lookup"><span data-stu-id="52764-129">The following table shows the properties that are required when you create the deviceLogCollectionResponse.</span></span>

|<span data-ttu-id="52764-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="52764-130">Property</span></span>|<span data-ttu-id="52764-131">Тип</span><span class="sxs-lookup"><span data-stu-id="52764-131">Type</span></span>|<span data-ttu-id="52764-132">Описание</span><span class="sxs-lookup"><span data-stu-id="52764-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52764-133">id</span><span class="sxs-lookup"><span data-stu-id="52764-133">id</span></span>|<span data-ttu-id="52764-134">Строка</span><span class="sxs-lookup"><span data-stu-id="52764-134">String</span></span>|<span data-ttu-id="52764-135">Уникальный идентификатор в виде tenantId_deviceId_requestId</span><span class="sxs-lookup"><span data-stu-id="52764-135">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="52764-136">status</span><span class="sxs-lookup"><span data-stu-id="52764-136">status</span></span>|<span data-ttu-id="52764-137">String</span><span class="sxs-lookup"><span data-stu-id="52764-137">String</span></span>|<span data-ttu-id="52764-138">Состояние запроса на сбор журналов</span><span class="sxs-lookup"><span data-stu-id="52764-138">The status of the log collection request</span></span>|
|<span data-ttu-id="52764-139">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="52764-139">managedDeviceId</span></span>|<span data-ttu-id="52764-140">Guid</span><span class="sxs-lookup"><span data-stu-id="52764-140">Guid</span></span>|<span data-ttu-id="52764-141">Идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="52764-141">The device Id</span></span>|
|<span data-ttu-id="52764-142">errorCode</span><span class="sxs-lookup"><span data-stu-id="52764-142">errorCode</span></span>|<span data-ttu-id="52764-143">Int64</span><span class="sxs-lookup"><span data-stu-id="52764-143">Int64</span></span>|<span data-ttu-id="52764-144">Код ошибки (при наличии).</span><span class="sxs-lookup"><span data-stu-id="52764-144">The error code, if any.</span></span> <span data-ttu-id="52764-145">Допустимые значения — 9.22337203685478 E + 18 — 9.22337203685478 E + 18</span><span class="sxs-lookup"><span data-stu-id="52764-145">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="52764-146">рекуестеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="52764-146">requestedDateTimeUTC</span></span>|<span data-ttu-id="52764-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52764-147">DateTimeOffset</span></span>|<span data-ttu-id="52764-148">Дата и время запроса</span><span class="sxs-lookup"><span data-stu-id="52764-148">The DateTime of the request</span></span>|
|<span data-ttu-id="52764-149">рецеиведдатетимеутк</span><span class="sxs-lookup"><span data-stu-id="52764-149">receivedDateTimeUTC</span></span>|<span data-ttu-id="52764-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52764-150">DateTimeOffset</span></span>|<span data-ttu-id="52764-151">Дата и время получения запроса</span><span class="sxs-lookup"><span data-stu-id="52764-151">The DateTime the request was received</span></span>|
|<span data-ttu-id="52764-152">Свойства initiatedbyuserprincipalname</span><span class="sxs-lookup"><span data-stu-id="52764-152">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="52764-153">Строка</span><span class="sxs-lookup"><span data-stu-id="52764-153">String</span></span>|<span data-ttu-id="52764-154">Имя участника-пользователя, который инициировал запрос.</span><span class="sxs-lookup"><span data-stu-id="52764-154">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="52764-155">експиратиондатетимеутк</span><span class="sxs-lookup"><span data-stu-id="52764-155">expirationDateTimeUTC</span></span>|<span data-ttu-id="52764-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52764-156">DateTimeOffset</span></span>|<span data-ttu-id="52764-157">Дата и время истечения срока действия журналов</span><span class="sxs-lookup"><span data-stu-id="52764-157">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="52764-158">size</span><span class="sxs-lookup"><span data-stu-id="52764-158">size</span></span>|<span data-ttu-id="52764-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="52764-159">Double</span></span>|<span data-ttu-id="52764-160">Размер журналов.</span><span class="sxs-lookup"><span data-stu-id="52764-160">The size of the logs.</span></span> <span data-ttu-id="52764-161">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="52764-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="52764-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="52764-162">Response</span></span>
<span data-ttu-id="52764-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52764-163">If successful, this method returns a `201 Created` response code and a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52764-164">Пример</span><span class="sxs-lookup"><span data-stu-id="52764-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="52764-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="52764-165">Request</span></span>
<span data-ttu-id="52764-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52764-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
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

### <a name="response"></a><span data-ttu-id="52764-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="52764-167">Response</span></span>
<span data-ttu-id="52764-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52764-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





