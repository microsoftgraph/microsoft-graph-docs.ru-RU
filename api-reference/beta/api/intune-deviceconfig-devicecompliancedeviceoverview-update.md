---
title: Обновление объекта deviceComplianceDeviceOverview
description: Обновление свойств объекта deviceComplianceDeviceOverview.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e0a52b7d9456340b8eed48eda2d39d435a33d225
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402680"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="299fc-103">Обновление объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="299fc-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="299fc-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="299fc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="299fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="299fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="299fc-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="299fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="299fc-107">Обновление свойств объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="299fc-107">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="299fc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="299fc-108">Prerequisites</span></span>
<span data-ttu-id="299fc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="299fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="299fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="299fc-111">Permission type</span></span>|<span data-ttu-id="299fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="299fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="299fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="299fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="299fc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="299fc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="299fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="299fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="299fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="299fc-116">Not supported.</span></span>|
|<span data-ttu-id="299fc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="299fc-117">Application</span></span>|<span data-ttu-id="299fc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="299fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="299fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="299fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="299fc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="299fc-120">Request headers</span></span>
|<span data-ttu-id="299fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="299fc-121">Header</span></span>|<span data-ttu-id="299fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="299fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="299fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="299fc-123">Authorization</span></span>|<span data-ttu-id="299fc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="299fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="299fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="299fc-125">Accept</span></span>|<span data-ttu-id="299fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="299fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="299fc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="299fc-127">Request body</span></span>
<span data-ttu-id="299fc-128">В тексте запроса добавьте представление объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="299fc-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="299fc-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="299fc-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="299fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="299fc-130">Property</span></span>|<span data-ttu-id="299fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="299fc-131">Type</span></span>|<span data-ttu-id="299fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="299fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="299fc-133">id</span><span class="sxs-lookup"><span data-stu-id="299fc-133">id</span></span>|<span data-ttu-id="299fc-134">String</span><span class="sxs-lookup"><span data-stu-id="299fc-134">String</span></span>|<span data-ttu-id="299fc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="299fc-135">Key of the entity.</span></span>|
|<span data-ttu-id="299fc-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="299fc-136">pendingCount</span></span>|<span data-ttu-id="299fc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="299fc-137">Int32</span></span>|<span data-ttu-id="299fc-138">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="299fc-138">Number of pending devices</span></span>|
|<span data-ttu-id="299fc-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="299fc-139">notApplicableCount</span></span>|<span data-ttu-id="299fc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="299fc-140">Int32</span></span>|<span data-ttu-id="299fc-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="299fc-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="299fc-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="299fc-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="299fc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="299fc-143">Int32</span></span>|<span data-ttu-id="299fc-144">Число неприменимо устройств из-за несоответствие платформы и политики</span><span class="sxs-lookup"><span data-stu-id="299fc-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="299fc-145">successCount</span><span class="sxs-lookup"><span data-stu-id="299fc-145">successCount</span></span>|<span data-ttu-id="299fc-146">Int32</span><span class="sxs-lookup"><span data-stu-id="299fc-146">Int32</span></span>|<span data-ttu-id="299fc-147">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="299fc-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="299fc-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="299fc-148">errorCount</span></span>|<span data-ttu-id="299fc-149">Int32</span><span class="sxs-lookup"><span data-stu-id="299fc-149">Int32</span></span>|<span data-ttu-id="299fc-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="299fc-150">Number of error devices</span></span>|
|<span data-ttu-id="299fc-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="299fc-151">failedCount</span></span>|<span data-ttu-id="299fc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="299fc-152">Int32</span></span>|<span data-ttu-id="299fc-153">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="299fc-153">Number of failed devices</span></span>|
|<span data-ttu-id="299fc-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="299fc-154">conflictCount</span></span>|<span data-ttu-id="299fc-155">Int32</span><span class="sxs-lookup"><span data-stu-id="299fc-155">Int32</span></span>|<span data-ttu-id="299fc-156">Количество устройств в конфликта</span><span class="sxs-lookup"><span data-stu-id="299fc-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="299fc-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="299fc-157">lastUpdateDateTime</span></span>|<span data-ttu-id="299fc-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="299fc-158">DateTimeOffset</span></span>|<span data-ttu-id="299fc-159">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="299fc-159">Last update time</span></span>|
|<span data-ttu-id="299fc-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="299fc-160">configurationVersion</span></span>|<span data-ttu-id="299fc-161">Int32</span><span class="sxs-lookup"><span data-stu-id="299fc-161">Int32</span></span>|<span data-ttu-id="299fc-162">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="299fc-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="299fc-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="299fc-163">Response</span></span>
<span data-ttu-id="299fc-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="299fc-164">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="299fc-165">Пример</span><span class="sxs-lookup"><span data-stu-id="299fc-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="299fc-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="299fc-166">Request</span></span>
<span data-ttu-id="299fc-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="299fc-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="299fc-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="299fc-168">Response</span></span>
<span data-ttu-id="299fc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="299fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




