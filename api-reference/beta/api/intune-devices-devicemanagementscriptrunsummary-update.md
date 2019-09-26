---
title: Обновление Девицеманажементскриптрунсуммари
description: Обновление свойств объекта Девицеманажементскриптрунсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 79938a72b84627cfa27c32e163034562d6737079
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180456"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="2563e-103">Обновление Девицеманажементскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="2563e-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="2563e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2563e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2563e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2563e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2563e-106">Обновление свойств объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="2563e-106">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2563e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2563e-107">Prerequisites</span></span>
<span data-ttu-id="2563e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2563e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2563e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2563e-110">Permission type</span></span>|<span data-ttu-id="2563e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2563e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2563e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2563e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2563e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2563e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2563e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2563e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2563e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2563e-115">Not supported.</span></span>|
|<span data-ttu-id="2563e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2563e-116">Application</span></span>|<span data-ttu-id="2563e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2563e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2563e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2563e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="2563e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2563e-119">Request headers</span></span>
|<span data-ttu-id="2563e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2563e-120">Header</span></span>|<span data-ttu-id="2563e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2563e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2563e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2563e-122">Authorization</span></span>|<span data-ttu-id="2563e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2563e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2563e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2563e-124">Accept</span></span>|<span data-ttu-id="2563e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2563e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2563e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2563e-126">Request body</span></span>
<span data-ttu-id="2563e-127">В тексте запроса добавьте представление объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2563e-127">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="2563e-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2563e-128">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="2563e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2563e-129">Property</span></span>|<span data-ttu-id="2563e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2563e-130">Type</span></span>|<span data-ttu-id="2563e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2563e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2563e-132">id</span><span class="sxs-lookup"><span data-stu-id="2563e-132">id</span></span>|<span data-ttu-id="2563e-133">String</span><span class="sxs-lookup"><span data-stu-id="2563e-133">String</span></span>|<span data-ttu-id="2563e-134">Key объекта сводки запуска сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="2563e-134">Key of the device management script run summary entity.</span></span> <span data-ttu-id="2563e-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2563e-135">This property is read-only.</span></span>|
|<span data-ttu-id="2563e-136">сукцессдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="2563e-136">successDeviceCount</span></span>|<span data-ttu-id="2563e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2563e-137">Int32</span></span>|<span data-ttu-id="2563e-138">Число устройств для успешной попытки.</span><span class="sxs-lookup"><span data-stu-id="2563e-138">Success device count.</span></span>|
|<span data-ttu-id="2563e-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2563e-139">errorDeviceCount</span></span>|<span data-ttu-id="2563e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2563e-140">Int32</span></span>|<span data-ttu-id="2563e-141">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="2563e-141">Error device count.</span></span>|
|<span data-ttu-id="2563e-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2563e-142">compliantDeviceCount</span></span>|<span data-ttu-id="2563e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2563e-143">Int32</span></span>|<span data-ttu-id="2563e-144">Число соответствующих устройств.</span><span class="sxs-lookup"><span data-stu-id="2563e-144">Compliant device count.</span></span>|
|<span data-ttu-id="2563e-145">ноткомплиантдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="2563e-145">notCompliantDeviceCount</span></span>|<span data-ttu-id="2563e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2563e-146">Int32</span></span>|<span data-ttu-id="2563e-147">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="2563e-147">Not Compliant device count.</span></span>|
|<span data-ttu-id="2563e-148">пендингдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="2563e-148">pendingDeviceCount</span></span>|<span data-ttu-id="2563e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2563e-149">Int32</span></span>|<span data-ttu-id="2563e-150">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="2563e-150">Pending device count.</span></span>|
|<span data-ttu-id="2563e-151">сукцессусеркаунт</span><span class="sxs-lookup"><span data-stu-id="2563e-151">successUserCount</span></span>|<span data-ttu-id="2563e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2563e-152">Int32</span></span>|<span data-ttu-id="2563e-153">Число пользователей Success.</span><span class="sxs-lookup"><span data-stu-id="2563e-153">Success user count.</span></span>|
|<span data-ttu-id="2563e-154">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="2563e-154">errorUserCount</span></span>|<span data-ttu-id="2563e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="2563e-155">Int32</span></span>|<span data-ttu-id="2563e-156">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="2563e-156">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="2563e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="2563e-157">Response</span></span>
<span data-ttu-id="2563e-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2563e-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2563e-159">Пример</span><span class="sxs-lookup"><span data-stu-id="2563e-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="2563e-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="2563e-160">Request</span></span>
<span data-ttu-id="2563e-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2563e-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
Content-type: application/json
Content-length: 270

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "compliantDeviceCount": 4,
  "notCompliantDeviceCount": 7,
  "pendingDeviceCount": 2,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="2563e-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="2563e-162">Response</span></span>
<span data-ttu-id="2563e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2563e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 319

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "compliantDeviceCount": 4,
  "notCompliantDeviceCount": 7,
  "pendingDeviceCount": 2,
  "successUserCount": 0,
  "errorUserCount": 14
}
```




