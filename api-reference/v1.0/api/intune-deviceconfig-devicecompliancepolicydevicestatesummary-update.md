---
title: Обновление объекта deviceCompliancePolicyDeviceStateSummary
description: Обновление свойств объекта deviceCompliancePolicyDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd58291b1f9dbec8c18449202aa10f461c645b6f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459677"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="e63d8-103">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e63d8-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="e63d8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e63d8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e63d8-105">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e63d8-105">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e63d8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e63d8-106">Prerequisites</span></span>
<span data-ttu-id="e63d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e63d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e63d8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e63d8-109">Permission type</span></span>|<span data-ttu-id="e63d8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e63d8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e63d8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e63d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e63d8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e63d8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e63d8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e63d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e63d8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e63d8-114">Not supported.</span></span>|
|<span data-ttu-id="e63d8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e63d8-115">Application</span></span>|<span data-ttu-id="e63d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e63d8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e63d8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e63d8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="e63d8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e63d8-118">Request headers</span></span>
|<span data-ttu-id="e63d8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e63d8-119">Header</span></span>|<span data-ttu-id="e63d8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e63d8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e63d8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e63d8-121">Authorization</span></span>|<span data-ttu-id="e63d8-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e63d8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e63d8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e63d8-123">Accept</span></span>|<span data-ttu-id="e63d8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e63d8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e63d8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e63d8-125">Request body</span></span>
<span data-ttu-id="e63d8-126">В тексте запроса добавьте представление объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e63d8-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="e63d8-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e63d8-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="e63d8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e63d8-128">Property</span></span>|<span data-ttu-id="e63d8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e63d8-129">Type</span></span>|<span data-ttu-id="e63d8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e63d8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e63d8-131">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="e63d8-131">inGracePeriodCount</span></span>|<span data-ttu-id="e63d8-132">Int32</span><span class="sxs-lookup"><span data-stu-id="e63d8-132">Int32</span></span>|<span data-ttu-id="e63d8-133">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="e63d8-133">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="e63d8-134">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="e63d8-134">configManagerCount</span></span>|<span data-ttu-id="e63d8-135">Int32</span><span class="sxs-lookup"><span data-stu-id="e63d8-135">Int32</span></span>|<span data-ttu-id="e63d8-136">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="e63d8-136">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="e63d8-137">id</span><span class="sxs-lookup"><span data-stu-id="e63d8-137">id</span></span>|<span data-ttu-id="e63d8-138">String</span><span class="sxs-lookup"><span data-stu-id="e63d8-138">String</span></span>|<span data-ttu-id="e63d8-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e63d8-139">Key of the entity.</span></span>|
|<span data-ttu-id="e63d8-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e63d8-140">unknownDeviceCount</span></span>|<span data-ttu-id="e63d8-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e63d8-141">Int32</span></span>|<span data-ttu-id="e63d8-142">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="e63d8-142">Number of unknown devices</span></span>|
|<span data-ttu-id="e63d8-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e63d8-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="e63d8-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e63d8-144">Int32</span></span>|<span data-ttu-id="e63d8-145">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="e63d8-145">Number of not applicable devices</span></span>|
|<span data-ttu-id="e63d8-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e63d8-146">compliantDeviceCount</span></span>|<span data-ttu-id="e63d8-147">Int32</span><span class="sxs-lookup"><span data-stu-id="e63d8-147">Int32</span></span>|<span data-ttu-id="e63d8-148">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="e63d8-148">Number of compliant devices</span></span>|
|<span data-ttu-id="e63d8-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e63d8-149">remediatedDeviceCount</span></span>|<span data-ttu-id="e63d8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e63d8-150">Int32</span></span>|<span data-ttu-id="e63d8-151">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="e63d8-151">Number of remediated devices</span></span>|
|<span data-ttu-id="e63d8-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e63d8-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e63d8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e63d8-153">Int32</span></span>|<span data-ttu-id="e63d8-154">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="e63d8-154">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e63d8-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e63d8-155">errorDeviceCount</span></span>|<span data-ttu-id="e63d8-156">Int32</span><span class="sxs-lookup"><span data-stu-id="e63d8-156">Int32</span></span>|<span data-ttu-id="e63d8-157">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e63d8-157">Number of error devices</span></span>|
|<span data-ttu-id="e63d8-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e63d8-158">conflictDeviceCount</span></span>|<span data-ttu-id="e63d8-159">Int32</span><span class="sxs-lookup"><span data-stu-id="e63d8-159">Int32</span></span>|<span data-ttu-id="e63d8-160">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="e63d8-160">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="e63d8-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="e63d8-161">Response</span></span>
<span data-ttu-id="e63d8-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e63d8-162">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e63d8-163">Пример</span><span class="sxs-lookup"><span data-stu-id="e63d8-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="e63d8-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="e63d8-164">Request</span></span>
<span data-ttu-id="e63d8-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e63d8-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
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

### <a name="response"></a><span data-ttu-id="e63d8-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="e63d8-166">Response</span></span>
<span data-ttu-id="e63d8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e63d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



