---
title: Обновление Девицеманажементскриптрунсуммари
description: Обновление свойств объекта Девицеманажементскриптрунсуммари.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ecb6ebfda52ad87a7ac75af8915e3b6b8023442a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43380126"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="07c1a-103">Обновление Девицеманажементскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="07c1a-103">Update deviceManagementScriptRunSummary</span></span>

<span data-ttu-id="07c1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07c1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07c1a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07c1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07c1a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07c1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07c1a-107">Обновление свойств объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="07c1a-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07c1a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="07c1a-108">Prerequisites</span></span>
<span data-ttu-id="07c1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07c1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07c1a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07c1a-111">Permission type</span></span>|<span data-ttu-id="07c1a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07c1a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07c1a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07c1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07c1a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c1a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="07c1a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07c1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07c1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07c1a-116">Not supported.</span></span>|
|<span data-ttu-id="07c1a-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="07c1a-117">Application</span></span>|<span data-ttu-id="07c1a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c1a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07c1a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07c1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="07c1a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="07c1a-120">Request headers</span></span>
|<span data-ttu-id="07c1a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07c1a-121">Header</span></span>|<span data-ttu-id="07c1a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="07c1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07c1a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07c1a-123">Authorization</span></span>|<span data-ttu-id="07c1a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07c1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07c1a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="07c1a-125">Accept</span></span>|<span data-ttu-id="07c1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07c1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07c1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07c1a-127">Request body</span></span>
<span data-ttu-id="07c1a-128">В тексте запроса добавьте представление объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07c1a-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="07c1a-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="07c1a-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="07c1a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="07c1a-130">Property</span></span>|<span data-ttu-id="07c1a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="07c1a-131">Type</span></span>|<span data-ttu-id="07c1a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="07c1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07c1a-133">id</span><span class="sxs-lookup"><span data-stu-id="07c1a-133">id</span></span>|<span data-ttu-id="07c1a-134">String</span><span class="sxs-lookup"><span data-stu-id="07c1a-134">String</span></span>|<span data-ttu-id="07c1a-135">Key объекта сводки запуска сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="07c1a-135">Key of the device management script run summary entity.</span></span> <span data-ttu-id="07c1a-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="07c1a-136">This property is read-only.</span></span>|
|<span data-ttu-id="07c1a-137">сукцессдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="07c1a-137">successDeviceCount</span></span>|<span data-ttu-id="07c1a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="07c1a-138">Int32</span></span>|<span data-ttu-id="07c1a-139">Число устройств для успешной попытки.</span><span class="sxs-lookup"><span data-stu-id="07c1a-139">Success device count.</span></span>|
|<span data-ttu-id="07c1a-140">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07c1a-140">errorDeviceCount</span></span>|<span data-ttu-id="07c1a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="07c1a-141">Int32</span></span>|<span data-ttu-id="07c1a-142">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="07c1a-142">Error device count.</span></span>|
|<span data-ttu-id="07c1a-143">сукцессусеркаунт</span><span class="sxs-lookup"><span data-stu-id="07c1a-143">successUserCount</span></span>|<span data-ttu-id="07c1a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="07c1a-144">Int32</span></span>|<span data-ttu-id="07c1a-145">Число пользователей Success.</span><span class="sxs-lookup"><span data-stu-id="07c1a-145">Success user count.</span></span>|
|<span data-ttu-id="07c1a-146">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="07c1a-146">errorUserCount</span></span>|<span data-ttu-id="07c1a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="07c1a-147">Int32</span></span>|<span data-ttu-id="07c1a-148">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="07c1a-148">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="07c1a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="07c1a-149">Response</span></span>
<span data-ttu-id="07c1a-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07c1a-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07c1a-151">Пример</span><span class="sxs-lookup"><span data-stu-id="07c1a-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="07c1a-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="07c1a-152">Request</span></span>
<span data-ttu-id="07c1a-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07c1a-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="07c1a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="07c1a-154">Response</span></span>
<span data-ttu-id="07c1a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07c1a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



