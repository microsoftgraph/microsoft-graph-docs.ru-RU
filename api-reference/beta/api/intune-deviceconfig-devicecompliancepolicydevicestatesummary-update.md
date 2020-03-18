---
title: Обновление объекта deviceCompliancePolicyDeviceStateSummary
description: Обновление свойств объекта deviceCompliancePolicyDeviceStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5da4941a6f37f67e320aca647332cadfdffaa483
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42755688"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="d0576-103">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="d0576-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="d0576-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0576-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0576-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0576-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0576-106">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d0576-106">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0576-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d0576-107">Prerequisites</span></span>
<span data-ttu-id="d0576-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0576-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0576-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0576-110">Permission type</span></span>|<span data-ttu-id="d0576-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0576-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0576-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0576-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0576-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0576-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0576-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0576-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0576-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0576-115">Not supported.</span></span>|
|<span data-ttu-id="d0576-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d0576-116">Application</span></span>|<span data-ttu-id="d0576-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0576-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0576-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0576-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="d0576-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d0576-119">Request headers</span></span>
|<span data-ttu-id="d0576-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0576-120">Header</span></span>|<span data-ttu-id="d0576-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d0576-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0576-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0576-122">Authorization</span></span>|<span data-ttu-id="d0576-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0576-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0576-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d0576-124">Accept</span></span>|<span data-ttu-id="d0576-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0576-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0576-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0576-126">Request body</span></span>
<span data-ttu-id="d0576-127">В тексте запроса добавьте представление объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0576-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="d0576-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d0576-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="d0576-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0576-129">Property</span></span>|<span data-ttu-id="d0576-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d0576-130">Type</span></span>|<span data-ttu-id="d0576-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d0576-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0576-132">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="d0576-132">inGracePeriodCount</span></span>|<span data-ttu-id="d0576-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d0576-133">Int32</span></span>|<span data-ttu-id="d0576-134">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="d0576-134">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="d0576-135">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="d0576-135">configManagerCount</span></span>|<span data-ttu-id="d0576-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d0576-136">Int32</span></span>|<span data-ttu-id="d0576-137">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="d0576-137">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="d0576-138">id</span><span class="sxs-lookup"><span data-stu-id="d0576-138">id</span></span>|<span data-ttu-id="d0576-139">String</span><span class="sxs-lookup"><span data-stu-id="d0576-139">String</span></span>|<span data-ttu-id="d0576-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d0576-140">Key of the entity.</span></span>|
|<span data-ttu-id="d0576-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d0576-141">unknownDeviceCount</span></span>|<span data-ttu-id="d0576-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d0576-142">Int32</span></span>|<span data-ttu-id="d0576-143">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="d0576-143">Number of unknown devices</span></span>|
|<span data-ttu-id="d0576-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d0576-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="d0576-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d0576-145">Int32</span></span>|<span data-ttu-id="d0576-146">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="d0576-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="d0576-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d0576-147">compliantDeviceCount</span></span>|<span data-ttu-id="d0576-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d0576-148">Int32</span></span>|<span data-ttu-id="d0576-149">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="d0576-149">Number of compliant devices</span></span>|
|<span data-ttu-id="d0576-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d0576-150">remediatedDeviceCount</span></span>|<span data-ttu-id="d0576-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d0576-151">Int32</span></span>|<span data-ttu-id="d0576-152">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="d0576-152">Number of remediated devices</span></span>|
|<span data-ttu-id="d0576-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d0576-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d0576-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d0576-154">Int32</span></span>|<span data-ttu-id="d0576-155">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="d0576-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="d0576-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d0576-156">errorDeviceCount</span></span>|<span data-ttu-id="d0576-157">Int32</span><span class="sxs-lookup"><span data-stu-id="d0576-157">Int32</span></span>|<span data-ttu-id="d0576-158">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="d0576-158">Number of error devices</span></span>|
|<span data-ttu-id="d0576-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d0576-159">conflictDeviceCount</span></span>|<span data-ttu-id="d0576-160">Int32</span><span class="sxs-lookup"><span data-stu-id="d0576-160">Int32</span></span>|<span data-ttu-id="d0576-161">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="d0576-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="d0576-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0576-162">Response</span></span>
<span data-ttu-id="d0576-163">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0576-163">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0576-164">Пример</span><span class="sxs-lookup"><span data-stu-id="d0576-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0576-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0576-165">Request</span></span>
<span data-ttu-id="d0576-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0576-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 349

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="d0576-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0576-167">Response</span></span>
<span data-ttu-id="d0576-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0576-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




