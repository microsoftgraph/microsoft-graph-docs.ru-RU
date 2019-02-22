---
title: Обновление Девицеманажементскриптрунсуммари
description: Обновление свойств объекта Девицеманажементскриптрунсуммари.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd41b6c7dbb7a2bb361175de564904c11e7e5e80
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141722"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="69f09-103">Обновление Девицеманажементскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="69f09-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="69f09-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69f09-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69f09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69f09-106">Обновление свойств объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="69f09-106">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69f09-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="69f09-107">Prerequisites</span></span>
<span data-ttu-id="69f09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="69f09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="69f09-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69f09-110">Permission type</span></span>|<span data-ttu-id="69f09-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69f09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f09-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69f09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69f09-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f09-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="69f09-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69f09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f09-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f09-115">Not supported.</span></span>|
|<span data-ttu-id="69f09-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69f09-116">Application</span></span>|<span data-ttu-id="69f09-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f09-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f09-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69f09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="69f09-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69f09-119">Request headers</span></span>
|<span data-ttu-id="69f09-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69f09-120">Header</span></span>|<span data-ttu-id="69f09-121">Значение</span><span class="sxs-lookup"><span data-stu-id="69f09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69f09-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69f09-122">Authorization</span></span>|<span data-ttu-id="69f09-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="69f09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69f09-124">Accept</span><span class="sxs-lookup"><span data-stu-id="69f09-124">Accept</span></span>|<span data-ttu-id="69f09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69f09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f09-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69f09-126">Request body</span></span>
<span data-ttu-id="69f09-127">В тексте запроса добавьте представление объекта [Девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69f09-127">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="69f09-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="69f09-128">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="69f09-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="69f09-129">Property</span></span>|<span data-ttu-id="69f09-130">Тип</span><span class="sxs-lookup"><span data-stu-id="69f09-130">Type</span></span>|<span data-ttu-id="69f09-131">Описание</span><span class="sxs-lookup"><span data-stu-id="69f09-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69f09-132">id</span><span class="sxs-lookup"><span data-stu-id="69f09-132">id</span></span>|<span data-ttu-id="69f09-133">String</span><span class="sxs-lookup"><span data-stu-id="69f09-133">String</span></span>|<span data-ttu-id="69f09-134">Key объекта сводки запуска сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="69f09-134">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="69f09-135">Сукцессдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="69f09-135">successDeviceCount</span></span>|<span data-ttu-id="69f09-136">Int32</span><span class="sxs-lookup"><span data-stu-id="69f09-136">Int32</span></span>|<span data-ttu-id="69f09-137">Число устройств для успешной попытки.</span><span class="sxs-lookup"><span data-stu-id="69f09-137">Success device count.</span></span>|
|<span data-ttu-id="69f09-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69f09-138">errorDeviceCount</span></span>|<span data-ttu-id="69f09-139">Int32</span><span class="sxs-lookup"><span data-stu-id="69f09-139">Int32</span></span>|<span data-ttu-id="69f09-140">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="69f09-140">Error device count.</span></span>|
|<span data-ttu-id="69f09-141">Сукцессусеркаунт</span><span class="sxs-lookup"><span data-stu-id="69f09-141">successUserCount</span></span>|<span data-ttu-id="69f09-142">Int32</span><span class="sxs-lookup"><span data-stu-id="69f09-142">Int32</span></span>|<span data-ttu-id="69f09-143">Число пользователей Success.</span><span class="sxs-lookup"><span data-stu-id="69f09-143">Success user count.</span></span>|
|<span data-ttu-id="69f09-144">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="69f09-144">errorUserCount</span></span>|<span data-ttu-id="69f09-145">Int32</span><span class="sxs-lookup"><span data-stu-id="69f09-145">Int32</span></span>|<span data-ttu-id="69f09-146">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="69f09-146">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="69f09-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f09-147">Response</span></span>
<span data-ttu-id="69f09-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69f09-148">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f09-149">Пример</span><span class="sxs-lookup"><span data-stu-id="69f09-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="69f09-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="69f09-150">Request</span></span>
<span data-ttu-id="69f09-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69f09-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
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

### <a name="response"></a><span data-ttu-id="69f09-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f09-152">Response</span></span>
<span data-ttu-id="69f09-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69f09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




