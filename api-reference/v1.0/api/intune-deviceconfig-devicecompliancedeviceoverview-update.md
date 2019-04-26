---
title: Обновление объекта deviceComplianceDeviceOverview
description: Обновление свойств объекта deviceComplianceDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dafbfe048217320c0b82905b3c32d2cb9e179893
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572544"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="0e055-103">Обновление объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0e055-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="0e055-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e055-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e055-105">Обновление свойств объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="0e055-105">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e055-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0e055-106">Prerequisites</span></span>
<span data-ttu-id="0e055-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e055-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e055-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e055-109">Permission type</span></span>|<span data-ttu-id="0e055-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e055-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e055-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e055-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e055-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e055-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e055-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e055-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e055-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e055-114">Not supported.</span></span>|
|<span data-ttu-id="0e055-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e055-115">Application</span></span>|<span data-ttu-id="0e055-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e055-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e055-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e055-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="0e055-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e055-118">Request headers</span></span>
|<span data-ttu-id="0e055-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e055-119">Header</span></span>|<span data-ttu-id="0e055-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0e055-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e055-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e055-121">Authorization</span></span>|<span data-ttu-id="0e055-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e055-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e055-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0e055-123">Accept</span></span>|<span data-ttu-id="0e055-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0e055-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e055-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e055-125">Request body</span></span>
<span data-ttu-id="0e055-126">В тексте запроса добавьте представление объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e055-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="0e055-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="0e055-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="0e055-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e055-128">Property</span></span>|<span data-ttu-id="0e055-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0e055-129">Type</span></span>|<span data-ttu-id="0e055-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0e055-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e055-131">id</span><span class="sxs-lookup"><span data-stu-id="0e055-131">id</span></span>|<span data-ttu-id="0e055-132">String</span><span class="sxs-lookup"><span data-stu-id="0e055-132">String</span></span>|<span data-ttu-id="0e055-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0e055-133">Key of the entity.</span></span>|
|<span data-ttu-id="0e055-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="0e055-134">pendingCount</span></span>|<span data-ttu-id="0e055-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0e055-135">Int32</span></span>|<span data-ttu-id="0e055-136">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="0e055-136">Number of pending devices</span></span>|
|<span data-ttu-id="0e055-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0e055-137">notApplicableCount</span></span>|<span data-ttu-id="0e055-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0e055-138">Int32</span></span>|<span data-ttu-id="0e055-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="0e055-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="0e055-140">successCount</span><span class="sxs-lookup"><span data-stu-id="0e055-140">successCount</span></span>|<span data-ttu-id="0e055-141">Int32</span><span class="sxs-lookup"><span data-stu-id="0e055-141">Int32</span></span>|<span data-ttu-id="0e055-142">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="0e055-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="0e055-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="0e055-143">errorCount</span></span>|<span data-ttu-id="0e055-144">Int32</span><span class="sxs-lookup"><span data-stu-id="0e055-144">Int32</span></span>|<span data-ttu-id="0e055-145">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="0e055-145">Number of error devices</span></span>|
|<span data-ttu-id="0e055-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="0e055-146">failedCount</span></span>|<span data-ttu-id="0e055-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0e055-147">Int32</span></span>|<span data-ttu-id="0e055-148">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="0e055-148">Number of failed devices</span></span>|
|<span data-ttu-id="0e055-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0e055-149">lastUpdateDateTime</span></span>|<span data-ttu-id="0e055-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e055-150">DateTimeOffset</span></span>|<span data-ttu-id="0e055-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="0e055-151">Last update time</span></span>|
|<span data-ttu-id="0e055-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="0e055-152">configurationVersion</span></span>|<span data-ttu-id="0e055-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0e055-153">Int32</span></span>|<span data-ttu-id="0e055-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="0e055-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="0e055-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e055-155">Response</span></span>
<span data-ttu-id="0e055-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e055-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e055-157">Пример</span><span class="sxs-lookup"><span data-stu-id="0e055-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e055-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e055-158">Request</span></span>
<span data-ttu-id="0e055-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e055-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e055-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e055-160">Response</span></span>
<span data-ttu-id="0e055-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e055-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



