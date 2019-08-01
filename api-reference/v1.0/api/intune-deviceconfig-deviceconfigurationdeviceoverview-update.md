---
title: Обновление объекта deviceConfigurationDeviceOverview
description: Обновление свойств объекта deviceConfigurationDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e47f904a5ee1216a63ed304411fca708995cc1e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017521"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="390fc-103">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="390fc-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="390fc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="390fc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="390fc-105">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="390fc-105">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="390fc-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="390fc-106">Prerequisites</span></span>
<span data-ttu-id="390fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="390fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="390fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="390fc-109">Permission type</span></span>|<span data-ttu-id="390fc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="390fc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="390fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="390fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="390fc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="390fc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="390fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="390fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="390fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="390fc-114">Not supported.</span></span>|
|<span data-ttu-id="390fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="390fc-115">Application</span></span>|<span data-ttu-id="390fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="390fc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="390fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="390fc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="390fc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="390fc-118">Request headers</span></span>
|<span data-ttu-id="390fc-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="390fc-119">Header</span></span>|<span data-ttu-id="390fc-120">Значение</span><span class="sxs-lookup"><span data-stu-id="390fc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="390fc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="390fc-121">Authorization</span></span>|<span data-ttu-id="390fc-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="390fc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="390fc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="390fc-123">Accept</span></span>|<span data-ttu-id="390fc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="390fc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="390fc-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="390fc-125">Request body</span></span>
<span data-ttu-id="390fc-126">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="390fc-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="390fc-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="390fc-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="390fc-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="390fc-128">Property</span></span>|<span data-ttu-id="390fc-129">Тип</span><span class="sxs-lookup"><span data-stu-id="390fc-129">Type</span></span>|<span data-ttu-id="390fc-130">Описание</span><span class="sxs-lookup"><span data-stu-id="390fc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="390fc-131">id</span><span class="sxs-lookup"><span data-stu-id="390fc-131">id</span></span>|<span data-ttu-id="390fc-132">String</span><span class="sxs-lookup"><span data-stu-id="390fc-132">String</span></span>|<span data-ttu-id="390fc-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="390fc-133">Key of the entity.</span></span>|
|<span data-ttu-id="390fc-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="390fc-134">pendingCount</span></span>|<span data-ttu-id="390fc-135">Int32</span><span class="sxs-lookup"><span data-stu-id="390fc-135">Int32</span></span>|<span data-ttu-id="390fc-136">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="390fc-136">Number of pending devices</span></span>|
|<span data-ttu-id="390fc-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="390fc-137">notApplicableCount</span></span>|<span data-ttu-id="390fc-138">Int32</span><span class="sxs-lookup"><span data-stu-id="390fc-138">Int32</span></span>|<span data-ttu-id="390fc-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="390fc-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="390fc-140">successCount</span><span class="sxs-lookup"><span data-stu-id="390fc-140">successCount</span></span>|<span data-ttu-id="390fc-141">Int32</span><span class="sxs-lookup"><span data-stu-id="390fc-141">Int32</span></span>|<span data-ttu-id="390fc-142">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="390fc-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="390fc-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="390fc-143">errorCount</span></span>|<span data-ttu-id="390fc-144">Int32</span><span class="sxs-lookup"><span data-stu-id="390fc-144">Int32</span></span>|<span data-ttu-id="390fc-145">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="390fc-145">Number of error devices</span></span>|
|<span data-ttu-id="390fc-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="390fc-146">failedCount</span></span>|<span data-ttu-id="390fc-147">Int32</span><span class="sxs-lookup"><span data-stu-id="390fc-147">Int32</span></span>|<span data-ttu-id="390fc-148">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="390fc-148">Number of failed devices</span></span>|
|<span data-ttu-id="390fc-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="390fc-149">lastUpdateDateTime</span></span>|<span data-ttu-id="390fc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="390fc-150">DateTimeOffset</span></span>|<span data-ttu-id="390fc-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="390fc-151">Last update time</span></span>|
|<span data-ttu-id="390fc-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="390fc-152">configurationVersion</span></span>|<span data-ttu-id="390fc-153">Int32</span><span class="sxs-lookup"><span data-stu-id="390fc-153">Int32</span></span>|<span data-ttu-id="390fc-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="390fc-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="390fc-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="390fc-155">Response</span></span>
<span data-ttu-id="390fc-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="390fc-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="390fc-157">Пример</span><span class="sxs-lookup"><span data-stu-id="390fc-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="390fc-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="390fc-158">Request</span></span>
<span data-ttu-id="390fc-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="390fc-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="390fc-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="390fc-160">Response</span></span>
<span data-ttu-id="390fc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="390fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



