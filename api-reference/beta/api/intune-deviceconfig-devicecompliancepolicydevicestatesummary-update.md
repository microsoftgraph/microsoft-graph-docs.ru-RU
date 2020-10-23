---
title: Обновление объекта deviceCompliancePolicyDeviceStateSummary
description: Обновление свойств объекта deviceCompliancePolicyDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d4df79fcc8a532fa4fe026cffee0b21100c3963a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733072"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="96ed5-103">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="96ed5-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

<span data-ttu-id="96ed5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96ed5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96ed5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96ed5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96ed5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96ed5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96ed5-107">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="96ed5-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96ed5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="96ed5-108">Prerequisites</span></span>
<span data-ttu-id="96ed5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96ed5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96ed5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96ed5-111">Permission type</span></span>|<span data-ttu-id="96ed5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96ed5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96ed5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96ed5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96ed5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96ed5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96ed5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96ed5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96ed5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96ed5-116">Not supported.</span></span>|
|<span data-ttu-id="96ed5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96ed5-117">Application</span></span>|<span data-ttu-id="96ed5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96ed5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96ed5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96ed5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="96ed5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="96ed5-120">Request headers</span></span>
|<span data-ttu-id="96ed5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96ed5-121">Header</span></span>|<span data-ttu-id="96ed5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="96ed5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96ed5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96ed5-123">Authorization</span></span>|<span data-ttu-id="96ed5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96ed5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96ed5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96ed5-125">Accept</span></span>|<span data-ttu-id="96ed5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96ed5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96ed5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="96ed5-127">Request body</span></span>
<span data-ttu-id="96ed5-128">В тексте запроса добавьте представление объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96ed5-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="96ed5-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="96ed5-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="96ed5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="96ed5-130">Property</span></span>|<span data-ttu-id="96ed5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="96ed5-131">Type</span></span>|<span data-ttu-id="96ed5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="96ed5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96ed5-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="96ed5-133">inGracePeriodCount</span></span>|<span data-ttu-id="96ed5-134">Int32</span><span class="sxs-lookup"><span data-stu-id="96ed5-134">Int32</span></span>|<span data-ttu-id="96ed5-135">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="96ed5-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="96ed5-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="96ed5-136">configManagerCount</span></span>|<span data-ttu-id="96ed5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="96ed5-137">Int32</span></span>|<span data-ttu-id="96ed5-138">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="96ed5-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="96ed5-139">id</span><span class="sxs-lookup"><span data-stu-id="96ed5-139">id</span></span>|<span data-ttu-id="96ed5-140">Строка</span><span class="sxs-lookup"><span data-stu-id="96ed5-140">String</span></span>|<span data-ttu-id="96ed5-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="96ed5-141">Key of the entity.</span></span>|
|<span data-ttu-id="96ed5-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ed5-142">unknownDeviceCount</span></span>|<span data-ttu-id="96ed5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="96ed5-143">Int32</span></span>|<span data-ttu-id="96ed5-144">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="96ed5-144">Number of unknown devices</span></span>|
|<span data-ttu-id="96ed5-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ed5-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="96ed5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="96ed5-146">Int32</span></span>|<span data-ttu-id="96ed5-147">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="96ed5-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="96ed5-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ed5-148">compliantDeviceCount</span></span>|<span data-ttu-id="96ed5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="96ed5-149">Int32</span></span>|<span data-ttu-id="96ed5-150">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="96ed5-150">Number of compliant devices</span></span>|
|<span data-ttu-id="96ed5-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ed5-151">remediatedDeviceCount</span></span>|<span data-ttu-id="96ed5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="96ed5-152">Int32</span></span>|<span data-ttu-id="96ed5-153">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="96ed5-153">Number of remediated devices</span></span>|
|<span data-ttu-id="96ed5-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ed5-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="96ed5-155">Int32</span><span class="sxs-lookup"><span data-stu-id="96ed5-155">Int32</span></span>|<span data-ttu-id="96ed5-156">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="96ed5-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="96ed5-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ed5-157">errorDeviceCount</span></span>|<span data-ttu-id="96ed5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="96ed5-158">Int32</span></span>|<span data-ttu-id="96ed5-159">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="96ed5-159">Number of error devices</span></span>|
|<span data-ttu-id="96ed5-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96ed5-160">conflictDeviceCount</span></span>|<span data-ttu-id="96ed5-161">Int32</span><span class="sxs-lookup"><span data-stu-id="96ed5-161">Int32</span></span>|<span data-ttu-id="96ed5-162">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="96ed5-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="96ed5-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="96ed5-163">Response</span></span>
<span data-ttu-id="96ed5-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96ed5-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96ed5-165">Пример</span><span class="sxs-lookup"><span data-stu-id="96ed5-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="96ed5-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="96ed5-166">Request</span></span>
<span data-ttu-id="96ed5-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96ed5-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96ed5-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="96ed5-168">Response</span></span>
<span data-ttu-id="96ed5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96ed5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





