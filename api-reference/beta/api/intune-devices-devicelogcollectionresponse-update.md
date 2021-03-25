---
title: Обновление deviceLogCollectionResponse
description: Обновление свойств объекта deviceLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed85268897942ba953ccdd5240d120829f6ea400
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154366"
---
# <a name="update-devicelogcollectionresponse"></a><span data-ttu-id="f6d5d-103">Обновление deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="f6d5d-103">Update deviceLogCollectionResponse</span></span>

<span data-ttu-id="f6d5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6d5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6d5d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6d5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6d5d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6d5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6d5d-107">Обновление свойств объекта [deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="f6d5d-107">Update the properties of a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6d5d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f6d5d-108">Prerequisites</span></span>
<span data-ttu-id="f6d5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6d5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6d5d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6d5d-111">Permission type</span></span>|<span data-ttu-id="f6d5d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6d5d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6d5d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6d5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6d5d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6d5d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f6d5d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6d5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6d5d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6d5d-116">Not supported.</span></span>|
|<span data-ttu-id="f6d5d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f6d5d-117">Application</span></span>|<span data-ttu-id="f6d5d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6d5d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6d5d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6d5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

## <a name="request-headers"></a><span data-ttu-id="f6d5d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f6d5d-120">Request headers</span></span>
|<span data-ttu-id="f6d5d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6d5d-121">Header</span></span>|<span data-ttu-id="f6d5d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f6d5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6d5d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6d5d-123">Authorization</span></span>|<span data-ttu-id="f6d5d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6d5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6d5d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f6d5d-125">Accept</span></span>|<span data-ttu-id="f6d5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6d5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6d5d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6d5d-127">Request body</span></span>
<span data-ttu-id="f6d5d-128">В теле запроса поставляем представление JSON для [объекта deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="f6d5d-128">In the request body, supply a JSON representation for the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

<span data-ttu-id="f6d5d-129">В следующей таблице показаны свойства, необходимые при создании [устройстваLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="f6d5d-129">The following table shows the properties that are required when you create the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md).</span></span>

|<span data-ttu-id="f6d5d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6d5d-130">Property</span></span>|<span data-ttu-id="f6d5d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f6d5d-131">Type</span></span>|<span data-ttu-id="f6d5d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f6d5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6d5d-133">id</span><span class="sxs-lookup"><span data-stu-id="f6d5d-133">id</span></span>|<span data-ttu-id="f6d5d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f6d5d-134">String</span></span>|<span data-ttu-id="f6d5d-135">Уникальный идентификатор в виде tenantId_deviceId_requestId</span><span class="sxs-lookup"><span data-stu-id="f6d5d-135">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="f6d5d-136">status</span><span class="sxs-lookup"><span data-stu-id="f6d5d-136">status</span></span>|<span data-ttu-id="f6d5d-137">String</span><span class="sxs-lookup"><span data-stu-id="f6d5d-137">String</span></span>|<span data-ttu-id="f6d5d-138">Состояние запроса на коллекцию журналов</span><span class="sxs-lookup"><span data-stu-id="f6d5d-138">The status of the log collection request</span></span>|
|<span data-ttu-id="f6d5d-139">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f6d5d-139">managedDeviceId</span></span>|<span data-ttu-id="f6d5d-140">Guid</span><span class="sxs-lookup"><span data-stu-id="f6d5d-140">Guid</span></span>|<span data-ttu-id="f6d5d-141">Id устройства</span><span class="sxs-lookup"><span data-stu-id="f6d5d-141">The device Id</span></span>|
|<span data-ttu-id="f6d5d-142">errorCode</span><span class="sxs-lookup"><span data-stu-id="f6d5d-142">errorCode</span></span>|<span data-ttu-id="f6d5d-143">Int64</span><span class="sxs-lookup"><span data-stu-id="f6d5d-143">Int64</span></span>|<span data-ttu-id="f6d5d-144">Код ошибки, если таковое есть.</span><span class="sxs-lookup"><span data-stu-id="f6d5d-144">The error code, if any.</span></span> <span data-ttu-id="f6d5d-145">Допустимые значения -9.2237203685478E+18 до 9.22337203685478E+18</span><span class="sxs-lookup"><span data-stu-id="f6d5d-145">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="f6d5d-146">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="f6d5d-146">requestedDateTimeUTC</span></span>|<span data-ttu-id="f6d5d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6d5d-147">DateTimeOffset</span></span>|<span data-ttu-id="f6d5d-148">DateTime запроса</span><span class="sxs-lookup"><span data-stu-id="f6d5d-148">The DateTime of the request</span></span>|
|<span data-ttu-id="f6d5d-149">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="f6d5d-149">receivedDateTimeUTC</span></span>|<span data-ttu-id="f6d5d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6d5d-150">DateTimeOffset</span></span>|<span data-ttu-id="f6d5d-151">DateTime, в который был получен запрос</span><span class="sxs-lookup"><span data-stu-id="f6d5d-151">The DateTime the request was received</span></span>|
|<span data-ttu-id="f6d5d-152">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6d5d-152">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="f6d5d-153">Строка</span><span class="sxs-lookup"><span data-stu-id="f6d5d-153">String</span></span>|<span data-ttu-id="f6d5d-154">UpN для тех, кто инициировал запрос</span><span class="sxs-lookup"><span data-stu-id="f6d5d-154">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="f6d5d-155">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="f6d5d-155">expirationDateTimeUTC</span></span>|<span data-ttu-id="f6d5d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6d5d-156">DateTimeOffset</span></span>|<span data-ttu-id="f6d5d-157">DateTime истечения срока действия журналов</span><span class="sxs-lookup"><span data-stu-id="f6d5d-157">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="f6d5d-158">size</span><span class="sxs-lookup"><span data-stu-id="f6d5d-158">size</span></span>|<span data-ttu-id="f6d5d-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="f6d5d-159">Double</span></span>|<span data-ttu-id="f6d5d-160">Размер журналов.</span><span class="sxs-lookup"><span data-stu-id="f6d5d-160">The size of the logs.</span></span> <span data-ttu-id="f6d5d-161">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="f6d5d-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="f6d5d-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6d5d-162">Response</span></span>
<span data-ttu-id="f6d5d-163">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f6d5d-163">If successful, this method returns a `200 OK` response code and an updated [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6d5d-164">Пример</span><span class="sxs-lookup"><span data-stu-id="f6d5d-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6d5d-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6d5d-165">Request</span></span>
<span data-ttu-id="f6d5d-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6d5d-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6d5d-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6d5d-167">Response</span></span>
<span data-ttu-id="f6d5d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6d5d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




