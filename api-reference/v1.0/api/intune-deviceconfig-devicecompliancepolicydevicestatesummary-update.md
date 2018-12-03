---
title: Обновление объекта deviceCompliancePolicyDeviceStateSummary
description: Обновление свойств объекта deviceCompliancePolicyDeviceStateSummary.
ms.openlocfilehash: 0cf0fe68f87bfe92536a5e13684818dabad1b2bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026161"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="2d7cf-103">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="2d7cf-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="2d7cf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d7cf-105">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="2d7cf-105">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d7cf-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2d7cf-106">Prerequisites</span></span>
<span data-ttu-id="2d7cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d7cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d7cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d7cf-109">Permission type</span></span>|<span data-ttu-id="2d7cf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d7cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d7cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d7cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2d7cf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d7cf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d7cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d7cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d7cf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-114">Not supported.</span></span>|
|<span data-ttu-id="2d7cf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d7cf-115">Application</span></span>|<span data-ttu-id="2d7cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d7cf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d7cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="2d7cf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d7cf-118">Request headers</span></span>
|<span data-ttu-id="2d7cf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d7cf-119">Header</span></span>|<span data-ttu-id="2d7cf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2d7cf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d7cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d7cf-121">Authorization</span></span>|<span data-ttu-id="2d7cf-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2d7cf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d7cf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2d7cf-123">Accept</span></span>|<span data-ttu-id="2d7cf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2d7cf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d7cf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d7cf-125">Request body</span></span>
<span data-ttu-id="2d7cf-126">В тексте запроса добавьте представление объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="2d7cf-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="2d7cf-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="2d7cf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d7cf-128">Property</span></span>|<span data-ttu-id="2d7cf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2d7cf-129">Type</span></span>|<span data-ttu-id="2d7cf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2d7cf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d7cf-131">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="2d7cf-131">inGracePeriodCount</span></span>|<span data-ttu-id="2d7cf-132">Int32</span><span class="sxs-lookup"><span data-stu-id="2d7cf-132">Int32</span></span>|<span data-ttu-id="2d7cf-133">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-133">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="2d7cf-134">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="2d7cf-134">configManagerCount</span></span>|<span data-ttu-id="2d7cf-135">Int32</span><span class="sxs-lookup"><span data-stu-id="2d7cf-135">Int32</span></span>|<span data-ttu-id="2d7cf-136">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-136">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="2d7cf-137">id</span><span class="sxs-lookup"><span data-stu-id="2d7cf-137">id</span></span>|<span data-ttu-id="2d7cf-138">String</span><span class="sxs-lookup"><span data-stu-id="2d7cf-138">String</span></span>|<span data-ttu-id="2d7cf-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-139">Key of the entity.</span></span>|
|<span data-ttu-id="2d7cf-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d7cf-140">unknownDeviceCount</span></span>|<span data-ttu-id="2d7cf-141">Int32</span><span class="sxs-lookup"><span data-stu-id="2d7cf-141">Int32</span></span>|<span data-ttu-id="2d7cf-142">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-142">Number of unknown devices</span></span>|
|<span data-ttu-id="2d7cf-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d7cf-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="2d7cf-144">Int32</span><span class="sxs-lookup"><span data-stu-id="2d7cf-144">Int32</span></span>|<span data-ttu-id="2d7cf-145">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-145">Number of not applicable devices</span></span>|
|<span data-ttu-id="2d7cf-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d7cf-146">compliantDeviceCount</span></span>|<span data-ttu-id="2d7cf-147">Int32</span><span class="sxs-lookup"><span data-stu-id="2d7cf-147">Int32</span></span>|<span data-ttu-id="2d7cf-148">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-148">Number of compliant devices</span></span>|
|<span data-ttu-id="2d7cf-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d7cf-149">remediatedDeviceCount</span></span>|<span data-ttu-id="2d7cf-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2d7cf-150">Int32</span></span>|<span data-ttu-id="2d7cf-151">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-151">Number of remediated devices</span></span>|
|<span data-ttu-id="2d7cf-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d7cf-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="2d7cf-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2d7cf-153">Int32</span></span>|<span data-ttu-id="2d7cf-154">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-154">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="2d7cf-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d7cf-155">errorDeviceCount</span></span>|<span data-ttu-id="2d7cf-156">Int32</span><span class="sxs-lookup"><span data-stu-id="2d7cf-156">Int32</span></span>|<span data-ttu-id="2d7cf-157">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-157">Number of error devices</span></span>|
|<span data-ttu-id="2d7cf-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2d7cf-158">conflictDeviceCount</span></span>|<span data-ttu-id="2d7cf-159">Int32</span><span class="sxs-lookup"><span data-stu-id="2d7cf-159">Int32</span></span>|<span data-ttu-id="2d7cf-160">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-160">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="2d7cf-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d7cf-161">Response</span></span>
<span data-ttu-id="2d7cf-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-162">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d7cf-163">Пример</span><span class="sxs-lookup"><span data-stu-id="2d7cf-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="2d7cf-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d7cf-164">Request</span></span>
<span data-ttu-id="2d7cf-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d7cf-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2d7cf-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d7cf-166">Response</span></span>
<span data-ttu-id="2d7cf-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2d7cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



