---
title: Создание deviceLogCollectionResponse
description: Создайте новый объект deviceLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9e01048af19572e26c7ba017c65ac6664b8fbc9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127069"
---
# <a name="create-devicelogcollectionresponse"></a><span data-ttu-id="03ba8-103">Создание deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="03ba8-103">Create deviceLogCollectionResponse</span></span>

<span data-ttu-id="03ba8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03ba8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03ba8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03ba8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03ba8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03ba8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03ba8-107">Создайте новый [объект deviceLogCollectionResponse.](../resources/intune-devices-devicelogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="03ba8-107">Create a new [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03ba8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03ba8-108">Prerequisites</span></span>
<span data-ttu-id="03ba8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03ba8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03ba8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03ba8-111">Permission type</span></span>|<span data-ttu-id="03ba8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03ba8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03ba8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03ba8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03ba8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03ba8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="03ba8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03ba8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03ba8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03ba8-116">Not supported.</span></span>|
|<span data-ttu-id="03ba8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="03ba8-117">Application</span></span>|<span data-ttu-id="03ba8-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03ba8-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03ba8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03ba8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="03ba8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03ba8-120">Request headers</span></span>
|<span data-ttu-id="03ba8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03ba8-121">Header</span></span>|<span data-ttu-id="03ba8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="03ba8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03ba8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03ba8-123">Authorization</span></span>|<span data-ttu-id="03ba8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03ba8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03ba8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03ba8-125">Accept</span></span>|<span data-ttu-id="03ba8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03ba8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03ba8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03ba8-127">Request body</span></span>
<span data-ttu-id="03ba8-128">В теле запроса поставляем представление JSON для объекта deviceLogCollectionResponse.</span><span class="sxs-lookup"><span data-stu-id="03ba8-128">In the request body, supply a JSON representation for the deviceLogCollectionResponse object.</span></span>

<span data-ttu-id="03ba8-129">В следующей таблице показаны свойства, необходимые при создании устройстваLogCollectionResponse.</span><span class="sxs-lookup"><span data-stu-id="03ba8-129">The following table shows the properties that are required when you create the deviceLogCollectionResponse.</span></span>

|<span data-ttu-id="03ba8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="03ba8-130">Property</span></span>|<span data-ttu-id="03ba8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="03ba8-131">Type</span></span>|<span data-ttu-id="03ba8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="03ba8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03ba8-133">id</span><span class="sxs-lookup"><span data-stu-id="03ba8-133">id</span></span>|<span data-ttu-id="03ba8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="03ba8-134">String</span></span>|<span data-ttu-id="03ba8-135">Уникальный идентификатор в виде tenantId_deviceId_requestId</span><span class="sxs-lookup"><span data-stu-id="03ba8-135">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="03ba8-136">status</span><span class="sxs-lookup"><span data-stu-id="03ba8-136">status</span></span>|<span data-ttu-id="03ba8-137">String</span><span class="sxs-lookup"><span data-stu-id="03ba8-137">String</span></span>|<span data-ttu-id="03ba8-138">Состояние запроса на коллекцию журналов</span><span class="sxs-lookup"><span data-stu-id="03ba8-138">The status of the log collection request</span></span>|
|<span data-ttu-id="03ba8-139">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="03ba8-139">managedDeviceId</span></span>|<span data-ttu-id="03ba8-140">Guid</span><span class="sxs-lookup"><span data-stu-id="03ba8-140">Guid</span></span>|<span data-ttu-id="03ba8-141">Id устройства</span><span class="sxs-lookup"><span data-stu-id="03ba8-141">The device Id</span></span>|
|<span data-ttu-id="03ba8-142">errorCode</span><span class="sxs-lookup"><span data-stu-id="03ba8-142">errorCode</span></span>|<span data-ttu-id="03ba8-143">Int64</span><span class="sxs-lookup"><span data-stu-id="03ba8-143">Int64</span></span>|<span data-ttu-id="03ba8-144">Код ошибки, если таковое есть.</span><span class="sxs-lookup"><span data-stu-id="03ba8-144">The error code, if any.</span></span> <span data-ttu-id="03ba8-145">Допустимые значения -9.2237203685478E+18 до 9.22337203685478E+18</span><span class="sxs-lookup"><span data-stu-id="03ba8-145">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="03ba8-146">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="03ba8-146">requestedDateTimeUTC</span></span>|<span data-ttu-id="03ba8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03ba8-147">DateTimeOffset</span></span>|<span data-ttu-id="03ba8-148">DateTime запроса</span><span class="sxs-lookup"><span data-stu-id="03ba8-148">The DateTime of the request</span></span>|
|<span data-ttu-id="03ba8-149">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="03ba8-149">receivedDateTimeUTC</span></span>|<span data-ttu-id="03ba8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03ba8-150">DateTimeOffset</span></span>|<span data-ttu-id="03ba8-151">DateTime, в который был получен запрос</span><span class="sxs-lookup"><span data-stu-id="03ba8-151">The DateTime the request was received</span></span>|
|<span data-ttu-id="03ba8-152">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="03ba8-152">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="03ba8-153">Строка</span><span class="sxs-lookup"><span data-stu-id="03ba8-153">String</span></span>|<span data-ttu-id="03ba8-154">UpN для тех, кто инициировал запрос</span><span class="sxs-lookup"><span data-stu-id="03ba8-154">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="03ba8-155">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="03ba8-155">expirationDateTimeUTC</span></span>|<span data-ttu-id="03ba8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03ba8-156">DateTimeOffset</span></span>|<span data-ttu-id="03ba8-157">DateTime истечения срока действия журналов</span><span class="sxs-lookup"><span data-stu-id="03ba8-157">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="03ba8-158">size</span><span class="sxs-lookup"><span data-stu-id="03ba8-158">size</span></span>|<span data-ttu-id="03ba8-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="03ba8-159">Double</span></span>|<span data-ttu-id="03ba8-160">Размер журналов.</span><span class="sxs-lookup"><span data-stu-id="03ba8-160">The size of the logs.</span></span> <span data-ttu-id="03ba8-161">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="03ba8-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="03ba8-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="03ba8-162">Response</span></span>
<span data-ttu-id="03ba8-163">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="03ba8-163">If successful, this method returns a `201 Created` response code and a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03ba8-164">Пример</span><span class="sxs-lookup"><span data-stu-id="03ba8-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="03ba8-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="03ba8-165">Request</span></span>
<span data-ttu-id="03ba8-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03ba8-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03ba8-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="03ba8-167">Response</span></span>
<span data-ttu-id="03ba8-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03ba8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




