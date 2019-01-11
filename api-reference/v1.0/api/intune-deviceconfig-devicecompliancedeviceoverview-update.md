---
title: Обновление объекта deviceComplianceDeviceOverview
description: Обновление свойств объекта deviceComplianceDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 884e8dc786196ff865c4f184a2f20a73926d3855
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876519"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="4729e-103">Обновление объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="4729e-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="4729e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4729e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4729e-105">Обновление свойств объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="4729e-105">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4729e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4729e-106">Prerequisites</span></span>
<span data-ttu-id="4729e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4729e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4729e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4729e-109">Permission type</span></span>|<span data-ttu-id="4729e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4729e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4729e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4729e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4729e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4729e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4729e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4729e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4729e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4729e-114">Not supported.</span></span>|
|<span data-ttu-id="4729e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4729e-115">Application</span></span>|<span data-ttu-id="4729e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4729e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4729e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4729e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="4729e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4729e-118">Request headers</span></span>
|<span data-ttu-id="4729e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4729e-119">Header</span></span>|<span data-ttu-id="4729e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4729e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4729e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4729e-121">Authorization</span></span>|<span data-ttu-id="4729e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4729e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4729e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4729e-123">Accept</span></span>|<span data-ttu-id="4729e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4729e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4729e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4729e-125">Request body</span></span>
<span data-ttu-id="4729e-126">В тексте запроса добавьте представление объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4729e-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="4729e-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="4729e-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="4729e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4729e-128">Property</span></span>|<span data-ttu-id="4729e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4729e-129">Type</span></span>|<span data-ttu-id="4729e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4729e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4729e-131">id</span><span class="sxs-lookup"><span data-stu-id="4729e-131">id</span></span>|<span data-ttu-id="4729e-132">Строка</span><span class="sxs-lookup"><span data-stu-id="4729e-132">String</span></span>|<span data-ttu-id="4729e-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4729e-133">Key of the entity.</span></span>|
|<span data-ttu-id="4729e-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="4729e-134">pendingCount</span></span>|<span data-ttu-id="4729e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="4729e-135">Int32</span></span>|<span data-ttu-id="4729e-136">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="4729e-136">Number of pending devices</span></span>|
|<span data-ttu-id="4729e-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4729e-137">notApplicableCount</span></span>|<span data-ttu-id="4729e-138">Int32</span><span class="sxs-lookup"><span data-stu-id="4729e-138">Int32</span></span>|<span data-ttu-id="4729e-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="4729e-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="4729e-140">successCount</span><span class="sxs-lookup"><span data-stu-id="4729e-140">successCount</span></span>|<span data-ttu-id="4729e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="4729e-141">Int32</span></span>|<span data-ttu-id="4729e-142">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="4729e-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="4729e-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="4729e-143">errorCount</span></span>|<span data-ttu-id="4729e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="4729e-144">Int32</span></span>|<span data-ttu-id="4729e-145">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="4729e-145">Number of error devices</span></span>|
|<span data-ttu-id="4729e-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="4729e-146">failedCount</span></span>|<span data-ttu-id="4729e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4729e-147">Int32</span></span>|<span data-ttu-id="4729e-148">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="4729e-148">Number of failed devices</span></span>|
|<span data-ttu-id="4729e-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4729e-149">lastUpdateDateTime</span></span>|<span data-ttu-id="4729e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4729e-150">DateTimeOffset</span></span>|<span data-ttu-id="4729e-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="4729e-151">Last update time</span></span>|
|<span data-ttu-id="4729e-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="4729e-152">configurationVersion</span></span>|<span data-ttu-id="4729e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4729e-153">Int32</span></span>|<span data-ttu-id="4729e-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="4729e-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="4729e-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4729e-155">Response</span></span>
<span data-ttu-id="4729e-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4729e-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4729e-157">Пример</span><span class="sxs-lookup"><span data-stu-id="4729e-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="4729e-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="4729e-158">Request</span></span>
<span data-ttu-id="4729e-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4729e-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4729e-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="4729e-160">Response</span></span>
<span data-ttu-id="4729e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4729e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



