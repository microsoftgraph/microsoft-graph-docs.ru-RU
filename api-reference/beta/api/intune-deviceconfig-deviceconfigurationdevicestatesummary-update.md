---
title: Обновление объекта deviceConfigurationDeviceStateSummary
description: Обновление свойств объекта deviceConfigurationDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a618ff77525957148d62f7bcfdbd2e154faf028b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49213548"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="d86e4-103">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="d86e4-103">Update deviceConfigurationDeviceStateSummary</span></span>

<span data-ttu-id="d86e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d86e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d86e4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d86e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d86e4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d86e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d86e4-107">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d86e4-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d86e4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d86e4-108">Prerequisites</span></span>
<span data-ttu-id="d86e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d86e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d86e4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d86e4-111">Permission type</span></span>|<span data-ttu-id="d86e4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d86e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d86e4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d86e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d86e4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d86e4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d86e4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d86e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d86e4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d86e4-116">Not supported.</span></span>|
|<span data-ttu-id="d86e4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d86e4-117">Application</span></span>|<span data-ttu-id="d86e4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d86e4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d86e4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d86e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d86e4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d86e4-120">Request headers</span></span>
|<span data-ttu-id="d86e4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d86e4-121">Header</span></span>|<span data-ttu-id="d86e4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d86e4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d86e4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d86e4-123">Authorization</span></span>|<span data-ttu-id="d86e4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d86e4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d86e4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d86e4-125">Accept</span></span>|<span data-ttu-id="d86e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d86e4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d86e4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d86e4-127">Request body</span></span>
<span data-ttu-id="d86e4-128">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d86e4-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="d86e4-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d86e4-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="d86e4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d86e4-130">Property</span></span>|<span data-ttu-id="d86e4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d86e4-131">Type</span></span>|<span data-ttu-id="d86e4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d86e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d86e4-133">id</span><span class="sxs-lookup"><span data-stu-id="d86e4-133">id</span></span>|<span data-ttu-id="d86e4-134">String</span><span class="sxs-lookup"><span data-stu-id="d86e4-134">String</span></span>|<span data-ttu-id="d86e4-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d86e4-135">Key of the entity.</span></span>|
|<span data-ttu-id="d86e4-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d86e4-136">unknownDeviceCount</span></span>|<span data-ttu-id="d86e4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d86e4-137">Int32</span></span>|<span data-ttu-id="d86e4-138">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="d86e4-138">Number of unknown devices</span></span>|
|<span data-ttu-id="d86e4-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d86e4-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="d86e4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d86e4-140">Int32</span></span>|<span data-ttu-id="d86e4-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="d86e4-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="d86e4-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d86e4-142">compliantDeviceCount</span></span>|<span data-ttu-id="d86e4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d86e4-143">Int32</span></span>|<span data-ttu-id="d86e4-144">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="d86e4-144">Number of compliant devices</span></span>|
|<span data-ttu-id="d86e4-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d86e4-145">remediatedDeviceCount</span></span>|<span data-ttu-id="d86e4-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d86e4-146">Int32</span></span>|<span data-ttu-id="d86e4-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="d86e4-147">Number of remediated devices</span></span>|
|<span data-ttu-id="d86e4-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d86e4-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d86e4-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d86e4-149">Int32</span></span>|<span data-ttu-id="d86e4-150">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="d86e4-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="d86e4-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d86e4-151">errorDeviceCount</span></span>|<span data-ttu-id="d86e4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d86e4-152">Int32</span></span>|<span data-ttu-id="d86e4-153">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="d86e4-153">Number of error devices</span></span>|
|<span data-ttu-id="d86e4-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d86e4-154">conflictDeviceCount</span></span>|<span data-ttu-id="d86e4-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d86e4-155">Int32</span></span>|<span data-ttu-id="d86e4-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="d86e4-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="d86e4-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d86e4-157">Response</span></span>
<span data-ttu-id="d86e4-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d86e4-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d86e4-159">Пример</span><span class="sxs-lookup"><span data-stu-id="d86e4-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d86e4-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="d86e4-160">Request</span></span>
<span data-ttu-id="d86e4-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d86e4-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="d86e4-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="d86e4-162">Response</span></span>
<span data-ttu-id="d86e4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d86e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




