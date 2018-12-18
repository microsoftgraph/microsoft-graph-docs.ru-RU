---
title: Обновление объекта deviceConfigurationDeviceOverview
description: Обновление свойств объекта deviceConfigurationDeviceOverview.
author: tfitzmac
ms.openlocfilehash: 5b47dfc9b3a716abcea1d77d093e2cce1d927efe
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301143"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="b0e34-103">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b0e34-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="b0e34-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b0e34-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0e34-105">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b0e34-105">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0e34-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b0e34-106">Prerequisites</span></span>
<span data-ttu-id="b0e34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0e34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0e34-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0e34-109">Permission type</span></span>|<span data-ttu-id="b0e34-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0e34-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0e34-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0e34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0e34-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0e34-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0e34-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0e34-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0e34-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0e34-114">Not supported.</span></span>|
|<span data-ttu-id="b0e34-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0e34-115">Application</span></span>|<span data-ttu-id="b0e34-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0e34-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0e34-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0e34-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="b0e34-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0e34-118">Request headers</span></span>
|<span data-ttu-id="b0e34-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0e34-119">Header</span></span>|<span data-ttu-id="b0e34-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b0e34-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0e34-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0e34-121">Authorization</span></span>|<span data-ttu-id="b0e34-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b0e34-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0e34-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b0e34-123">Accept</span></span>|<span data-ttu-id="b0e34-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b0e34-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0e34-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0e34-125">Request body</span></span>
<span data-ttu-id="b0e34-126">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0e34-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="b0e34-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b0e34-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="b0e34-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0e34-128">Property</span></span>|<span data-ttu-id="b0e34-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b0e34-129">Type</span></span>|<span data-ttu-id="b0e34-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b0e34-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0e34-131">id</span><span class="sxs-lookup"><span data-stu-id="b0e34-131">id</span></span>|<span data-ttu-id="b0e34-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b0e34-132">String</span></span>|<span data-ttu-id="b0e34-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b0e34-133">Key of the entity.</span></span>|
|<span data-ttu-id="b0e34-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="b0e34-134">pendingCount</span></span>|<span data-ttu-id="b0e34-135">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e34-135">Int32</span></span>|<span data-ttu-id="b0e34-136">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="b0e34-136">Number of pending devices</span></span>|
|<span data-ttu-id="b0e34-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b0e34-137">notApplicableCount</span></span>|<span data-ttu-id="b0e34-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e34-138">Int32</span></span>|<span data-ttu-id="b0e34-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="b0e34-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="b0e34-140">successCount</span><span class="sxs-lookup"><span data-stu-id="b0e34-140">successCount</span></span>|<span data-ttu-id="b0e34-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e34-141">Int32</span></span>|<span data-ttu-id="b0e34-142">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="b0e34-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="b0e34-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="b0e34-143">errorCount</span></span>|<span data-ttu-id="b0e34-144">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e34-144">Int32</span></span>|<span data-ttu-id="b0e34-145">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="b0e34-145">Number of error devices</span></span>|
|<span data-ttu-id="b0e34-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="b0e34-146">failedCount</span></span>|<span data-ttu-id="b0e34-147">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e34-147">Int32</span></span>|<span data-ttu-id="b0e34-148">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="b0e34-148">Number of failed devices</span></span>|
|<span data-ttu-id="b0e34-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b0e34-149">lastUpdateDateTime</span></span>|<span data-ttu-id="b0e34-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0e34-150">DateTimeOffset</span></span>|<span data-ttu-id="b0e34-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="b0e34-151">Last update time</span></span>|
|<span data-ttu-id="b0e34-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="b0e34-152">configurationVersion</span></span>|<span data-ttu-id="b0e34-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b0e34-153">Int32</span></span>|<span data-ttu-id="b0e34-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="b0e34-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="b0e34-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0e34-155">Response</span></span>
<span data-ttu-id="b0e34-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0e34-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0e34-157">Пример</span><span class="sxs-lookup"><span data-stu-id="b0e34-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0e34-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0e34-158">Request</span></span>
<span data-ttu-id="b0e34-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0e34-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0e34-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0e34-160">Response</span></span>
<span data-ttu-id="b0e34-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b0e34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



