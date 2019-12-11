---
title: Обновление Девицеманажементскриптрунсуммари
description: Обновление свойств объекта Девицеманажементскриптрунсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 707f3dd56ea68de21116fd9558be0d260344ab04
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944920"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="f3642-103">Обновление Девицеманажементскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="f3642-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="f3642-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3642-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3642-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3642-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3642-106">Обновление свойств объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f3642-106">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3642-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3642-107">Prerequisites</span></span>
<span data-ttu-id="f3642-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3642-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3642-110">Permission type</span></span>|<span data-ttu-id="f3642-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3642-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3642-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3642-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3642-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3642-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f3642-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3642-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3642-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3642-115">Not supported.</span></span>|
|<span data-ttu-id="f3642-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3642-116">Application</span></span>|<span data-ttu-id="f3642-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3642-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3642-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3642-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="f3642-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3642-119">Request headers</span></span>
|<span data-ttu-id="f3642-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3642-120">Header</span></span>|<span data-ttu-id="f3642-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f3642-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3642-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3642-122">Authorization</span></span>|<span data-ttu-id="f3642-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3642-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3642-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f3642-124">Accept</span></span>|<span data-ttu-id="f3642-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3642-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3642-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f3642-126">Request body</span></span>
<span data-ttu-id="f3642-127">В тексте запроса добавьте представление объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3642-127">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="f3642-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f3642-128">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="f3642-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3642-129">Property</span></span>|<span data-ttu-id="f3642-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f3642-130">Type</span></span>|<span data-ttu-id="f3642-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f3642-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3642-132">id</span><span class="sxs-lookup"><span data-stu-id="f3642-132">id</span></span>|<span data-ttu-id="f3642-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f3642-133">String</span></span>|<span data-ttu-id="f3642-134">Key объекта сводки запуска сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="f3642-134">Key of the device management script run summary entity.</span></span> <span data-ttu-id="f3642-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3642-135">This property is read-only.</span></span>|
|<span data-ttu-id="f3642-136">сукцессдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f3642-136">successDeviceCount</span></span>|<span data-ttu-id="f3642-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f3642-137">Int32</span></span>|<span data-ttu-id="f3642-138">Число устройств для успешной попытки.</span><span class="sxs-lookup"><span data-stu-id="f3642-138">Success device count.</span></span>|
|<span data-ttu-id="f3642-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f3642-139">errorDeviceCount</span></span>|<span data-ttu-id="f3642-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f3642-140">Int32</span></span>|<span data-ttu-id="f3642-141">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="f3642-141">Error device count.</span></span>|
|<span data-ttu-id="f3642-142">сукцессусеркаунт</span><span class="sxs-lookup"><span data-stu-id="f3642-142">successUserCount</span></span>|<span data-ttu-id="f3642-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f3642-143">Int32</span></span>|<span data-ttu-id="f3642-144">Число пользователей Success.</span><span class="sxs-lookup"><span data-stu-id="f3642-144">Success user count.</span></span>|
|<span data-ttu-id="f3642-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="f3642-145">errorUserCount</span></span>|<span data-ttu-id="f3642-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f3642-146">Int32</span></span>|<span data-ttu-id="f3642-147">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="f3642-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="f3642-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3642-148">Response</span></span>
<span data-ttu-id="f3642-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3642-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3642-150">Пример</span><span class="sxs-lookup"><span data-stu-id="f3642-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3642-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3642-151">Request</span></span>
<span data-ttu-id="f3642-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3642-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="f3642-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3642-153">Response</span></span>
<span data-ttu-id="f3642-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3642-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```





