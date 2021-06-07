---
title: Обновление объекта deviceComplianceDeviceOverview
description: Обновление свойств объекта deviceComplianceDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a24964891779a1b376bc4d0e92e013a1e1ca9728
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756647"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="5d5bf-103">Обновление объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5d5bf-103">Update deviceComplianceDeviceOverview</span></span>

<span data-ttu-id="5d5bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d5bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d5bf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d5bf-106">Обновление свойств объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="5d5bf-106">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d5bf-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5d5bf-107">Prerequisites</span></span>
<span data-ttu-id="5d5bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d5bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d5bf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d5bf-110">Permission type</span></span>|<span data-ttu-id="5d5bf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d5bf-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d5bf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d5bf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5d5bf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d5bf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5d5bf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d5bf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d5bf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-115">Not supported.</span></span>|
|<span data-ttu-id="5d5bf-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5d5bf-116">Application</span></span>|<span data-ttu-id="5d5bf-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d5bf-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d5bf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d5bf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="5d5bf-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5d5bf-119">Request headers</span></span>
|<span data-ttu-id="5d5bf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d5bf-120">Header</span></span>|<span data-ttu-id="5d5bf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5d5bf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d5bf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d5bf-122">Authorization</span></span>|<span data-ttu-id="5d5bf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d5bf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5d5bf-124">Accept</span></span>|<span data-ttu-id="5d5bf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5d5bf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d5bf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d5bf-126">Request body</span></span>
<span data-ttu-id="5d5bf-127">В тексте запроса добавьте представление объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="5d5bf-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="5d5bf-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="5d5bf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d5bf-129">Property</span></span>|<span data-ttu-id="5d5bf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5d5bf-130">Type</span></span>|<span data-ttu-id="5d5bf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5d5bf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d5bf-132">id</span><span class="sxs-lookup"><span data-stu-id="5d5bf-132">id</span></span>|<span data-ttu-id="5d5bf-133">String</span><span class="sxs-lookup"><span data-stu-id="5d5bf-133">String</span></span>|<span data-ttu-id="5d5bf-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-134">Key of the entity.</span></span>|
|<span data-ttu-id="5d5bf-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="5d5bf-135">pendingCount</span></span>|<span data-ttu-id="5d5bf-136">Int32</span><span class="sxs-lookup"><span data-stu-id="5d5bf-136">Int32</span></span>|<span data-ttu-id="5d5bf-137">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-137">Number of pending devices</span></span>|
|<span data-ttu-id="5d5bf-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="5d5bf-138">notApplicableCount</span></span>|<span data-ttu-id="5d5bf-139">Int32</span><span class="sxs-lookup"><span data-stu-id="5d5bf-139">Int32</span></span>|<span data-ttu-id="5d5bf-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="5d5bf-141">successCount</span><span class="sxs-lookup"><span data-stu-id="5d5bf-141">successCount</span></span>|<span data-ttu-id="5d5bf-142">Int32</span><span class="sxs-lookup"><span data-stu-id="5d5bf-142">Int32</span></span>|<span data-ttu-id="5d5bf-143">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="5d5bf-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="5d5bf-144">errorCount</span></span>|<span data-ttu-id="5d5bf-145">Int32</span><span class="sxs-lookup"><span data-stu-id="5d5bf-145">Int32</span></span>|<span data-ttu-id="5d5bf-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-146">Number of error devices</span></span>|
|<span data-ttu-id="5d5bf-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="5d5bf-147">failedCount</span></span>|<span data-ttu-id="5d5bf-148">Int32</span><span class="sxs-lookup"><span data-stu-id="5d5bf-148">Int32</span></span>|<span data-ttu-id="5d5bf-149">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-149">Number of failed devices</span></span>|
|<span data-ttu-id="5d5bf-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="5d5bf-150">lastUpdateDateTime</span></span>|<span data-ttu-id="5d5bf-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d5bf-151">DateTimeOffset</span></span>|<span data-ttu-id="5d5bf-152">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-152">Last update time</span></span>|
|<span data-ttu-id="5d5bf-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="5d5bf-153">configurationVersion</span></span>|<span data-ttu-id="5d5bf-154">Int32</span><span class="sxs-lookup"><span data-stu-id="5d5bf-154">Int32</span></span>|<span data-ttu-id="5d5bf-155">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="5d5bf-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d5bf-156">Response</span></span>
<span data-ttu-id="5d5bf-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d5bf-158">Пример</span><span class="sxs-lookup"><span data-stu-id="5d5bf-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d5bf-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d5bf-159">Request</span></span>
<span data-ttu-id="5d5bf-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="5d5bf-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d5bf-161">Response</span></span>
<span data-ttu-id="5d5bf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d5bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




