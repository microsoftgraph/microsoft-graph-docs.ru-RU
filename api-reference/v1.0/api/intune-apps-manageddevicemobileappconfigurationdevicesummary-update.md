---
title: Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 595a1b0352421b4470324011cafb7e594dad60ce
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759842"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="546cd-103">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="546cd-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

<span data-ttu-id="546cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="546cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="546cd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="546cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="546cd-106">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="546cd-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="546cd-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="546cd-107">Prerequisites</span></span>
<span data-ttu-id="546cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="546cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="546cd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="546cd-110">Permission type</span></span>|<span data-ttu-id="546cd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="546cd-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="546cd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="546cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="546cd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="546cd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="546cd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="546cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="546cd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="546cd-115">Not supported.</span></span>|
|<span data-ttu-id="546cd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="546cd-116">Application</span></span>|<span data-ttu-id="546cd-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="546cd-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="546cd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="546cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="546cd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="546cd-119">Request headers</span></span>
|<span data-ttu-id="546cd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="546cd-120">Header</span></span>|<span data-ttu-id="546cd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="546cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="546cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="546cd-122">Authorization</span></span>|<span data-ttu-id="546cd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="546cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="546cd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="546cd-124">Accept</span></span>|<span data-ttu-id="546cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="546cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="546cd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="546cd-126">Request body</span></span>
<span data-ttu-id="546cd-127">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="546cd-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="546cd-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="546cd-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="546cd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="546cd-129">Property</span></span>|<span data-ttu-id="546cd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="546cd-130">Type</span></span>|<span data-ttu-id="546cd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="546cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="546cd-132">id</span><span class="sxs-lookup"><span data-stu-id="546cd-132">id</span></span>|<span data-ttu-id="546cd-133">String</span><span class="sxs-lookup"><span data-stu-id="546cd-133">String</span></span>|<span data-ttu-id="546cd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="546cd-134">Key of the entity.</span></span>|
|<span data-ttu-id="546cd-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="546cd-135">pendingCount</span></span>|<span data-ttu-id="546cd-136">Int32</span><span class="sxs-lookup"><span data-stu-id="546cd-136">Int32</span></span>|<span data-ttu-id="546cd-137">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="546cd-137">Number of pending devices</span></span>|
|<span data-ttu-id="546cd-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="546cd-138">notApplicableCount</span></span>|<span data-ttu-id="546cd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="546cd-139">Int32</span></span>|<span data-ttu-id="546cd-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="546cd-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="546cd-141">successCount</span><span class="sxs-lookup"><span data-stu-id="546cd-141">successCount</span></span>|<span data-ttu-id="546cd-142">Int32</span><span class="sxs-lookup"><span data-stu-id="546cd-142">Int32</span></span>|<span data-ttu-id="546cd-143">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="546cd-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="546cd-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="546cd-144">errorCount</span></span>|<span data-ttu-id="546cd-145">Int32</span><span class="sxs-lookup"><span data-stu-id="546cd-145">Int32</span></span>|<span data-ttu-id="546cd-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="546cd-146">Number of error devices</span></span>|
|<span data-ttu-id="546cd-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="546cd-147">failedCount</span></span>|<span data-ttu-id="546cd-148">Int32</span><span class="sxs-lookup"><span data-stu-id="546cd-148">Int32</span></span>|<span data-ttu-id="546cd-149">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="546cd-149">Number of failed devices</span></span>|
|<span data-ttu-id="546cd-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="546cd-150">lastUpdateDateTime</span></span>|<span data-ttu-id="546cd-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="546cd-151">DateTimeOffset</span></span>|<span data-ttu-id="546cd-152">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="546cd-152">Last update time</span></span>|
|<span data-ttu-id="546cd-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="546cd-153">configurationVersion</span></span>|<span data-ttu-id="546cd-154">Int32</span><span class="sxs-lookup"><span data-stu-id="546cd-154">Int32</span></span>|<span data-ttu-id="546cd-155">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="546cd-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="546cd-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="546cd-156">Response</span></span>
<span data-ttu-id="546cd-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="546cd-157">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="546cd-158">Пример</span><span class="sxs-lookup"><span data-stu-id="546cd-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="546cd-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="546cd-159">Request</span></span>
<span data-ttu-id="546cd-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="546cd-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 299

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="546cd-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="546cd-161">Response</span></span>
<span data-ttu-id="546cd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="546cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




