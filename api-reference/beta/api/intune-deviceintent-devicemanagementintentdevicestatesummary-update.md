---
title: Обновление deviceManagementIntentDeviceStateSummary
description: Обновление свойств объекта deviceManagementIntentDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0556f44326e76563374d3e84497f1f9ed3dbf1c2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130968"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="7c288-103">Обновление deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7c288-103">Update deviceManagementIntentDeviceStateSummary</span></span>

<span data-ttu-id="7c288-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c288-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c288-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c288-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c288-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c288-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c288-107">Обновление свойств объекта [deviceManagementIntentDeviceStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="7c288-107">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c288-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7c288-108">Prerequisites</span></span>
<span data-ttu-id="7c288-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c288-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c288-111">Permission type</span></span>|<span data-ttu-id="7c288-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c288-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c288-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c288-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c288-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c288-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c288-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c288-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c288-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c288-116">Not supported.</span></span>|
|<span data-ttu-id="7c288-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7c288-117">Application</span></span>|<span data-ttu-id="7c288-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c288-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c288-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c288-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="7c288-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7c288-120">Request headers</span></span>
|<span data-ttu-id="7c288-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c288-121">Header</span></span>|<span data-ttu-id="7c288-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7c288-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c288-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c288-123">Authorization</span></span>|<span data-ttu-id="7c288-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c288-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c288-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c288-125">Accept</span></span>|<span data-ttu-id="7c288-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c288-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c288-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c288-127">Request body</span></span>
<span data-ttu-id="7c288-128">В теле запроса поставляем представление JSON для [объекта deviceManagementIntentDeviceStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="7c288-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

<span data-ttu-id="7c288-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementIntentDeviceStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="7c288-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span></span>

|<span data-ttu-id="7c288-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c288-130">Property</span></span>|<span data-ttu-id="7c288-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7c288-131">Type</span></span>|<span data-ttu-id="7c288-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7c288-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c288-133">id</span><span class="sxs-lookup"><span data-stu-id="7c288-133">id</span></span>|<span data-ttu-id="7c288-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7c288-134">String</span></span>|<span data-ttu-id="7c288-135">The ID</span><span class="sxs-lookup"><span data-stu-id="7c288-135">The ID</span></span>|
|<span data-ttu-id="7c288-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="7c288-136">conflictCount</span></span>|<span data-ttu-id="7c288-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7c288-137">Int32</span></span>|<span data-ttu-id="7c288-138">Количество устройств в конфликте</span><span class="sxs-lookup"><span data-stu-id="7c288-138">Number of devices in conflict</span></span>|
|<span data-ttu-id="7c288-139">errorCount</span><span class="sxs-lookup"><span data-stu-id="7c288-139">errorCount</span></span>|<span data-ttu-id="7c288-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7c288-140">Int32</span></span>|<span data-ttu-id="7c288-141">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="7c288-141">Number of error devices</span></span>|
|<span data-ttu-id="7c288-142">failedCount</span><span class="sxs-lookup"><span data-stu-id="7c288-142">failedCount</span></span>|<span data-ttu-id="7c288-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7c288-143">Int32</span></span>|<span data-ttu-id="7c288-144">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="7c288-144">Number of failed devices</span></span>|
|<span data-ttu-id="7c288-145">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="7c288-145">notApplicableCount</span></span>|<span data-ttu-id="7c288-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7c288-146">Int32</span></span>|<span data-ttu-id="7c288-147">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="7c288-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="7c288-148">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="7c288-148">notApplicablePlatformCount</span></span>|<span data-ttu-id="7c288-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7c288-149">Int32</span></span>|<span data-ttu-id="7c288-150">Количество не применимых устройств из-за несоответствия платформы и политики</span><span class="sxs-lookup"><span data-stu-id="7c288-150">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="7c288-151">successCount</span><span class="sxs-lookup"><span data-stu-id="7c288-151">successCount</span></span>|<span data-ttu-id="7c288-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7c288-152">Int32</span></span>|<span data-ttu-id="7c288-153">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="7c288-153">Number of succeeded devices</span></span>|



## <a name="response"></a><span data-ttu-id="7c288-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c288-154">Response</span></span>
<span data-ttu-id="7c288-155">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7c288-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c288-156">Пример</span><span class="sxs-lookup"><span data-stu-id="7c288-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c288-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c288-157">Request</span></span>
<span data-ttu-id="7c288-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c288-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
Content-type: application/json
Content-length: 237

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```

### <a name="response"></a><span data-ttu-id="7c288-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c288-159">Response</span></span>
<span data-ttu-id="7c288-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c288-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "12230bf9-0bf9-1223-f90b-2312f90b2312",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```




