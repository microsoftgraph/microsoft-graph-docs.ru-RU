---
title: Обновление объекта deviceConfigurationDeviceOverview
description: Обновление свойств объекта deviceConfigurationDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f6aadd22c5762b2b8159a858014d6f374deabaf0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914208"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="bef2e-103">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bef2e-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="bef2e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bef2e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bef2e-105">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bef2e-105">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bef2e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bef2e-106">Prerequisites</span></span>
<span data-ttu-id="bef2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bef2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bef2e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bef2e-109">Permission type</span></span>|<span data-ttu-id="bef2e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bef2e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bef2e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bef2e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bef2e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bef2e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bef2e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bef2e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bef2e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bef2e-114">Not supported.</span></span>|
|<span data-ttu-id="bef2e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bef2e-115">Application</span></span>|<span data-ttu-id="bef2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bef2e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bef2e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bef2e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="bef2e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bef2e-118">Request headers</span></span>
|<span data-ttu-id="bef2e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bef2e-119">Header</span></span>|<span data-ttu-id="bef2e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bef2e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bef2e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bef2e-121">Authorization</span></span>|<span data-ttu-id="bef2e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bef2e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bef2e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bef2e-123">Accept</span></span>|<span data-ttu-id="bef2e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bef2e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bef2e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bef2e-125">Request body</span></span>
<span data-ttu-id="bef2e-126">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bef2e-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="bef2e-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bef2e-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="bef2e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bef2e-128">Property</span></span>|<span data-ttu-id="bef2e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bef2e-129">Type</span></span>|<span data-ttu-id="bef2e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bef2e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bef2e-131">id</span><span class="sxs-lookup"><span data-stu-id="bef2e-131">id</span></span>|<span data-ttu-id="bef2e-132">Строка</span><span class="sxs-lookup"><span data-stu-id="bef2e-132">String</span></span>|<span data-ttu-id="bef2e-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bef2e-133">Key of the entity.</span></span>|
|<span data-ttu-id="bef2e-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="bef2e-134">pendingCount</span></span>|<span data-ttu-id="bef2e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="bef2e-135">Int32</span></span>|<span data-ttu-id="bef2e-136">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="bef2e-136">Number of pending devices</span></span>|
|<span data-ttu-id="bef2e-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="bef2e-137">notApplicableCount</span></span>|<span data-ttu-id="bef2e-138">Int32</span><span class="sxs-lookup"><span data-stu-id="bef2e-138">Int32</span></span>|<span data-ttu-id="bef2e-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="bef2e-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="bef2e-140">successCount</span><span class="sxs-lookup"><span data-stu-id="bef2e-140">successCount</span></span>|<span data-ttu-id="bef2e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="bef2e-141">Int32</span></span>|<span data-ttu-id="bef2e-142">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="bef2e-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="bef2e-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="bef2e-143">errorCount</span></span>|<span data-ttu-id="bef2e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="bef2e-144">Int32</span></span>|<span data-ttu-id="bef2e-145">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="bef2e-145">Number of error devices</span></span>|
|<span data-ttu-id="bef2e-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="bef2e-146">failedCount</span></span>|<span data-ttu-id="bef2e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bef2e-147">Int32</span></span>|<span data-ttu-id="bef2e-148">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="bef2e-148">Number of failed devices</span></span>|
|<span data-ttu-id="bef2e-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="bef2e-149">lastUpdateDateTime</span></span>|<span data-ttu-id="bef2e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bef2e-150">DateTimeOffset</span></span>|<span data-ttu-id="bef2e-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="bef2e-151">Last update time</span></span>|
|<span data-ttu-id="bef2e-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="bef2e-152">configurationVersion</span></span>|<span data-ttu-id="bef2e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="bef2e-153">Int32</span></span>|<span data-ttu-id="bef2e-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="bef2e-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="bef2e-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="bef2e-155">Response</span></span>
<span data-ttu-id="bef2e-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bef2e-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bef2e-157">Пример</span><span class="sxs-lookup"><span data-stu-id="bef2e-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="bef2e-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="bef2e-158">Request</span></span>
<span data-ttu-id="bef2e-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bef2e-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bef2e-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="bef2e-160">Response</span></span>
<span data-ttu-id="bef2e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bef2e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



