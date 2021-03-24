---
title: Обновление объекта deviceConfigurationDeviceStateSummary
description: Обновление свойств объекта deviceConfigurationDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 64182b6155346b509ed16ce0a2029d08e8597c1d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131661"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="a71e5-103">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="a71e5-103">Update deviceConfigurationDeviceStateSummary</span></span>

<span data-ttu-id="a71e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a71e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a71e5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a71e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a71e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a71e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a71e5-107">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a71e5-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a71e5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a71e5-108">Prerequisites</span></span>
<span data-ttu-id="a71e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a71e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a71e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a71e5-111">Permission type</span></span>|<span data-ttu-id="a71e5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a71e5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a71e5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a71e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a71e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a71e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a71e5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a71e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a71e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a71e5-116">Not supported.</span></span>|
|<span data-ttu-id="a71e5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a71e5-117">Application</span></span>|<span data-ttu-id="a71e5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a71e5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a71e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a71e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a71e5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a71e5-120">Request headers</span></span>
|<span data-ttu-id="a71e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a71e5-121">Header</span></span>|<span data-ttu-id="a71e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a71e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a71e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a71e5-123">Authorization</span></span>|<span data-ttu-id="a71e5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a71e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a71e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a71e5-125">Accept</span></span>|<span data-ttu-id="a71e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a71e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a71e5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a71e5-127">Request body</span></span>
<span data-ttu-id="a71e5-128">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a71e5-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="a71e5-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a71e5-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="a71e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a71e5-130">Property</span></span>|<span data-ttu-id="a71e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a71e5-131">Type</span></span>|<span data-ttu-id="a71e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a71e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a71e5-133">id</span><span class="sxs-lookup"><span data-stu-id="a71e5-133">id</span></span>|<span data-ttu-id="a71e5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a71e5-134">String</span></span>|<span data-ttu-id="a71e5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a71e5-135">Key of the entity.</span></span>|
|<span data-ttu-id="a71e5-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a71e5-136">unknownDeviceCount</span></span>|<span data-ttu-id="a71e5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a71e5-137">Int32</span></span>|<span data-ttu-id="a71e5-138">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="a71e5-138">Number of unknown devices</span></span>|
|<span data-ttu-id="a71e5-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a71e5-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="a71e5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a71e5-140">Int32</span></span>|<span data-ttu-id="a71e5-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="a71e5-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="a71e5-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a71e5-142">compliantDeviceCount</span></span>|<span data-ttu-id="a71e5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a71e5-143">Int32</span></span>|<span data-ttu-id="a71e5-144">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="a71e5-144">Number of compliant devices</span></span>|
|<span data-ttu-id="a71e5-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a71e5-145">remediatedDeviceCount</span></span>|<span data-ttu-id="a71e5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a71e5-146">Int32</span></span>|<span data-ttu-id="a71e5-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="a71e5-147">Number of remediated devices</span></span>|
|<span data-ttu-id="a71e5-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a71e5-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a71e5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a71e5-149">Int32</span></span>|<span data-ttu-id="a71e5-150">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="a71e5-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="a71e5-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a71e5-151">errorDeviceCount</span></span>|<span data-ttu-id="a71e5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a71e5-152">Int32</span></span>|<span data-ttu-id="a71e5-153">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="a71e5-153">Number of error devices</span></span>|
|<span data-ttu-id="a71e5-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a71e5-154">conflictDeviceCount</span></span>|<span data-ttu-id="a71e5-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a71e5-155">Int32</span></span>|<span data-ttu-id="a71e5-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="a71e5-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="a71e5-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a71e5-157">Response</span></span>
<span data-ttu-id="a71e5-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a71e5-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a71e5-159">Пример</span><span class="sxs-lookup"><span data-stu-id="a71e5-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="a71e5-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="a71e5-160">Request</span></span>
<span data-ttu-id="a71e5-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a71e5-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a71e5-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="a71e5-162">Response</span></span>
<span data-ttu-id="a71e5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a71e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




