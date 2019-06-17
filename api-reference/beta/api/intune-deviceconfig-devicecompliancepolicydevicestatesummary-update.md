---
title: Обновление объекта deviceCompliancePolicyDeviceStateSummary
description: Обновление свойств объекта deviceCompliancePolicyDeviceStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11af97a7245845f9982ac31c5e24109d0a1812d9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968324"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="47501-103">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="47501-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="47501-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47501-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47501-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47501-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47501-106">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="47501-106">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47501-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="47501-107">Prerequisites</span></span>
<span data-ttu-id="47501-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47501-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47501-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47501-110">Permission type</span></span>|<span data-ttu-id="47501-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47501-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47501-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47501-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47501-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47501-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47501-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47501-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47501-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47501-115">Not supported.</span></span>|
|<span data-ttu-id="47501-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47501-116">Application</span></span>|<span data-ttu-id="47501-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47501-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47501-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47501-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="47501-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47501-119">Request headers</span></span>
|<span data-ttu-id="47501-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47501-120">Header</span></span>|<span data-ttu-id="47501-121">Значение</span><span class="sxs-lookup"><span data-stu-id="47501-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47501-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47501-122">Authorization</span></span>|<span data-ttu-id="47501-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47501-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47501-124">Accept</span><span class="sxs-lookup"><span data-stu-id="47501-124">Accept</span></span>|<span data-ttu-id="47501-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47501-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47501-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47501-126">Request body</span></span>
<span data-ttu-id="47501-127">В тексте запроса добавьте представление объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47501-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="47501-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="47501-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="47501-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="47501-129">Property</span></span>|<span data-ttu-id="47501-130">Тип</span><span class="sxs-lookup"><span data-stu-id="47501-130">Type</span></span>|<span data-ttu-id="47501-131">Описание</span><span class="sxs-lookup"><span data-stu-id="47501-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47501-132">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="47501-132">inGracePeriodCount</span></span>|<span data-ttu-id="47501-133">Int32</span><span class="sxs-lookup"><span data-stu-id="47501-133">Int32</span></span>|<span data-ttu-id="47501-134">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="47501-134">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="47501-135">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="47501-135">configManagerCount</span></span>|<span data-ttu-id="47501-136">Int32</span><span class="sxs-lookup"><span data-stu-id="47501-136">Int32</span></span>|<span data-ttu-id="47501-137">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="47501-137">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="47501-138">id</span><span class="sxs-lookup"><span data-stu-id="47501-138">id</span></span>|<span data-ttu-id="47501-139">String</span><span class="sxs-lookup"><span data-stu-id="47501-139">String</span></span>|<span data-ttu-id="47501-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47501-140">Key of the entity.</span></span>|
|<span data-ttu-id="47501-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47501-141">unknownDeviceCount</span></span>|<span data-ttu-id="47501-142">Int32</span><span class="sxs-lookup"><span data-stu-id="47501-142">Int32</span></span>|<span data-ttu-id="47501-143">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="47501-143">Number of unknown devices</span></span>|
|<span data-ttu-id="47501-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47501-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="47501-145">Int32</span><span class="sxs-lookup"><span data-stu-id="47501-145">Int32</span></span>|<span data-ttu-id="47501-146">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="47501-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="47501-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47501-147">compliantDeviceCount</span></span>|<span data-ttu-id="47501-148">Int32</span><span class="sxs-lookup"><span data-stu-id="47501-148">Int32</span></span>|<span data-ttu-id="47501-149">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="47501-149">Number of compliant devices</span></span>|
|<span data-ttu-id="47501-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47501-150">remediatedDeviceCount</span></span>|<span data-ttu-id="47501-151">Int32</span><span class="sxs-lookup"><span data-stu-id="47501-151">Int32</span></span>|<span data-ttu-id="47501-152">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="47501-152">Number of remediated devices</span></span>|
|<span data-ttu-id="47501-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47501-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="47501-154">Int32</span><span class="sxs-lookup"><span data-stu-id="47501-154">Int32</span></span>|<span data-ttu-id="47501-155">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="47501-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="47501-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47501-156">errorDeviceCount</span></span>|<span data-ttu-id="47501-157">Int32</span><span class="sxs-lookup"><span data-stu-id="47501-157">Int32</span></span>|<span data-ttu-id="47501-158">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="47501-158">Number of error devices</span></span>|
|<span data-ttu-id="47501-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47501-159">conflictDeviceCount</span></span>|<span data-ttu-id="47501-160">Int32</span><span class="sxs-lookup"><span data-stu-id="47501-160">Int32</span></span>|<span data-ttu-id="47501-161">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="47501-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="47501-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="47501-162">Response</span></span>
<span data-ttu-id="47501-163">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47501-163">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47501-164">Пример</span><span class="sxs-lookup"><span data-stu-id="47501-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="47501-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="47501-165">Request</span></span>
<span data-ttu-id="47501-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47501-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47501-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="47501-167">Response</span></span>
<span data-ttu-id="47501-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47501-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





