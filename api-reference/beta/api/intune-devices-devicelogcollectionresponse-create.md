---
title: Создание Девицелогколлектионреспонсе
description: Создание нового объекта Девицелогколлектионреспонсе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c11917ab1501aeebf7629cddf96ec9ea7f6d0fa
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124326"
---
# <a name="create-devicelogcollectionresponse"></a><span data-ttu-id="3988b-103">Создание Девицелогколлектионреспонсе</span><span class="sxs-lookup"><span data-stu-id="3988b-103">Create deviceLogCollectionResponse</span></span>

<span data-ttu-id="3988b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3988b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3988b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3988b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3988b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3988b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3988b-107">Создание нового объекта [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="3988b-107">Create a new [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3988b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3988b-108">Prerequisites</span></span>
<span data-ttu-id="3988b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3988b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3988b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3988b-111">Permission type</span></span>|<span data-ttu-id="3988b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3988b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3988b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3988b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3988b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3988b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3988b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3988b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3988b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3988b-116">Not supported.</span></span>|
|<span data-ttu-id="3988b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3988b-117">Application</span></span>|<span data-ttu-id="3988b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3988b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3988b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3988b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="3988b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3988b-120">Request headers</span></span>
|<span data-ttu-id="3988b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3988b-121">Header</span></span>|<span data-ttu-id="3988b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3988b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3988b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3988b-123">Authorization</span></span>|<span data-ttu-id="3988b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3988b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3988b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3988b-125">Accept</span></span>|<span data-ttu-id="3988b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3988b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3988b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3988b-127">Request body</span></span>
<span data-ttu-id="3988b-128">В тексте запроса добавьте представление объекта Девицелогколлектионреспонсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3988b-128">In the request body, supply a JSON representation for the deviceLogCollectionResponse object.</span></span>

<span data-ttu-id="3988b-129">В следующей таблице приведены свойства, необходимые при создании Девицелогколлектионреспонсе.</span><span class="sxs-lookup"><span data-stu-id="3988b-129">The following table shows the properties that are required when you create the deviceLogCollectionResponse.</span></span>

|<span data-ttu-id="3988b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3988b-130">Property</span></span>|<span data-ttu-id="3988b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3988b-131">Type</span></span>|<span data-ttu-id="3988b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3988b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3988b-133">id</span><span class="sxs-lookup"><span data-stu-id="3988b-133">id</span></span>|<span data-ttu-id="3988b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3988b-134">String</span></span>|<span data-ttu-id="3988b-135">Уникальный идентификатор в виде tenantId_deviceId_requestId</span><span class="sxs-lookup"><span data-stu-id="3988b-135">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="3988b-136">status</span><span class="sxs-lookup"><span data-stu-id="3988b-136">status</span></span>|<span data-ttu-id="3988b-137">String</span><span class="sxs-lookup"><span data-stu-id="3988b-137">String</span></span>|<span data-ttu-id="3988b-138">Состояние запроса на сбор журналов</span><span class="sxs-lookup"><span data-stu-id="3988b-138">The status of the log collection request</span></span>|
|<span data-ttu-id="3988b-139">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="3988b-139">managedDeviceId</span></span>|<span data-ttu-id="3988b-140">Guid</span><span class="sxs-lookup"><span data-stu-id="3988b-140">Guid</span></span>|<span data-ttu-id="3988b-141">Идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="3988b-141">The device Id</span></span>|
|<span data-ttu-id="3988b-142">errorCode</span><span class="sxs-lookup"><span data-stu-id="3988b-142">errorCode</span></span>|<span data-ttu-id="3988b-143">Int64</span><span class="sxs-lookup"><span data-stu-id="3988b-143">Int64</span></span>|<span data-ttu-id="3988b-144">Код ошибки (при наличии).</span><span class="sxs-lookup"><span data-stu-id="3988b-144">The error code, if any.</span></span> <span data-ttu-id="3988b-145">Допустимые значения — 9.22337203685478 E + 18 — 9.22337203685478 E + 18</span><span class="sxs-lookup"><span data-stu-id="3988b-145">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="3988b-146">рекуестеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="3988b-146">requestedDateTimeUTC</span></span>|<span data-ttu-id="3988b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3988b-147">DateTimeOffset</span></span>|<span data-ttu-id="3988b-148">Дата и время запроса</span><span class="sxs-lookup"><span data-stu-id="3988b-148">The DateTime of the request</span></span>|
|<span data-ttu-id="3988b-149">рецеиведдатетимеутк</span><span class="sxs-lookup"><span data-stu-id="3988b-149">receivedDateTimeUTC</span></span>|<span data-ttu-id="3988b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3988b-150">DateTimeOffset</span></span>|<span data-ttu-id="3988b-151">Дата и время получения запроса</span><span class="sxs-lookup"><span data-stu-id="3988b-151">The DateTime the request was received</span></span>|
|<span data-ttu-id="3988b-152">Свойства initiatedbyuserprincipalname</span><span class="sxs-lookup"><span data-stu-id="3988b-152">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="3988b-153">String</span><span class="sxs-lookup"><span data-stu-id="3988b-153">String</span></span>|<span data-ttu-id="3988b-154">Имя участника-пользователя, который инициировал запрос.</span><span class="sxs-lookup"><span data-stu-id="3988b-154">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="3988b-155">експиратиондатетимеутк</span><span class="sxs-lookup"><span data-stu-id="3988b-155">expirationDateTimeUTC</span></span>|<span data-ttu-id="3988b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3988b-156">DateTimeOffset</span></span>|<span data-ttu-id="3988b-157">Дата и время истечения срока действия журналов</span><span class="sxs-lookup"><span data-stu-id="3988b-157">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="3988b-158">size</span><span class="sxs-lookup"><span data-stu-id="3988b-158">size</span></span>|<span data-ttu-id="3988b-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="3988b-159">Double</span></span>|<span data-ttu-id="3988b-160">Размер журналов.</span><span class="sxs-lookup"><span data-stu-id="3988b-160">The size of the logs.</span></span> <span data-ttu-id="3988b-161">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="3988b-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="3988b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="3988b-162">Response</span></span>
<span data-ttu-id="3988b-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицелогколлектионреспонсе](../resources/intune-devices-devicelogcollectionresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3988b-163">If successful, this method returns a `201 Created` response code and a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3988b-164">Пример</span><span class="sxs-lookup"><span data-stu-id="3988b-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="3988b-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="3988b-165">Request</span></span>
<span data-ttu-id="3988b-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3988b-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3988b-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="3988b-167">Response</span></span>
<span data-ttu-id="3988b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3988b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



