---
title: Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a29e7f3f3e76e8327073831d4e4deec5fafb8bf2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471715"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="a1fb9-103">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a1fb9-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

<span data-ttu-id="a1fb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1fb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1fb9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1fb9-106">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a1fb9-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1fb9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a1fb9-107">Prerequisites</span></span>
<span data-ttu-id="a1fb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1fb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1fb9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1fb9-110">Permission type</span></span>|<span data-ttu-id="a1fb9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1fb9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1fb9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1fb9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1fb9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1fb9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a1fb9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1fb9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1fb9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-115">Not supported.</span></span>|
|<span data-ttu-id="a1fb9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1fb9-116">Application</span></span>|<span data-ttu-id="a1fb9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1fb9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1fb9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="a1fb9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a1fb9-119">Request headers</span></span>
|<span data-ttu-id="a1fb9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1fb9-120">Header</span></span>|<span data-ttu-id="a1fb9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a1fb9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1fb9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1fb9-122">Authorization</span></span>|<span data-ttu-id="a1fb9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1fb9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a1fb9-124">Accept</span></span>|<span data-ttu-id="a1fb9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1fb9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1fb9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1fb9-126">Request body</span></span>
<span data-ttu-id="a1fb9-127">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="a1fb9-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a1fb9-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="a1fb9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1fb9-129">Property</span></span>|<span data-ttu-id="a1fb9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a1fb9-130">Type</span></span>|<span data-ttu-id="a1fb9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a1fb9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1fb9-132">id</span><span class="sxs-lookup"><span data-stu-id="a1fb9-132">id</span></span>|<span data-ttu-id="a1fb9-133">String</span><span class="sxs-lookup"><span data-stu-id="a1fb9-133">String</span></span>|<span data-ttu-id="a1fb9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-134">Key of the entity.</span></span>|
|<span data-ttu-id="a1fb9-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="a1fb9-135">pendingCount</span></span>|<span data-ttu-id="a1fb9-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a1fb9-136">Int32</span></span>|<span data-ttu-id="a1fb9-137">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-137">Number of pending devices</span></span>|
|<span data-ttu-id="a1fb9-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a1fb9-138">notApplicableCount</span></span>|<span data-ttu-id="a1fb9-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a1fb9-139">Int32</span></span>|<span data-ttu-id="a1fb9-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="a1fb9-141">successCount</span><span class="sxs-lookup"><span data-stu-id="a1fb9-141">successCount</span></span>|<span data-ttu-id="a1fb9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a1fb9-142">Int32</span></span>|<span data-ttu-id="a1fb9-143">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="a1fb9-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="a1fb9-144">errorCount</span></span>|<span data-ttu-id="a1fb9-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a1fb9-145">Int32</span></span>|<span data-ttu-id="a1fb9-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-146">Number of error devices</span></span>|
|<span data-ttu-id="a1fb9-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="a1fb9-147">failedCount</span></span>|<span data-ttu-id="a1fb9-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a1fb9-148">Int32</span></span>|<span data-ttu-id="a1fb9-149">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-149">Number of failed devices</span></span>|
|<span data-ttu-id="a1fb9-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a1fb9-150">lastUpdateDateTime</span></span>|<span data-ttu-id="a1fb9-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1fb9-151">DateTimeOffset</span></span>|<span data-ttu-id="a1fb9-152">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-152">Last update time</span></span>|
|<span data-ttu-id="a1fb9-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="a1fb9-153">configurationVersion</span></span>|<span data-ttu-id="a1fb9-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a1fb9-154">Int32</span></span>|<span data-ttu-id="a1fb9-155">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="a1fb9-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1fb9-156">Response</span></span>
<span data-ttu-id="a1fb9-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-157">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1fb9-158">Пример</span><span class="sxs-lookup"><span data-stu-id="a1fb9-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1fb9-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1fb9-159">Request</span></span>
<span data-ttu-id="a1fb9-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1fb9-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1fb9-161">Response</span></span>
<span data-ttu-id="a1fb9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1fb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






