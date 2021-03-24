---
title: Обновление deviceManagementIntentDeviceSettingStateSummary
description: Обновление свойств объекта deviceManagementIntentDeviceSettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be1189953214b68196e10eefd36a9b055f5bb99d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132046"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="e4aeb-103">Обновление deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="e4aeb-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="e4aeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4aeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4aeb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4aeb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4aeb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4aeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4aeb-107">Обновление свойств объекта [deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e4aeb-107">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4aeb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4aeb-108">Prerequisites</span></span>
<span data-ttu-id="e4aeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4aeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4aeb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4aeb-111">Permission type</span></span>|<span data-ttu-id="e4aeb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4aeb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4aeb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4aeb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4aeb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4aeb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4aeb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4aeb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4aeb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4aeb-116">Not supported.</span></span>|
|<span data-ttu-id="e4aeb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e4aeb-117">Application</span></span>|<span data-ttu-id="e4aeb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4aeb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4aeb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4aeb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="e4aeb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e4aeb-120">Request headers</span></span>
|<span data-ttu-id="e4aeb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4aeb-121">Header</span></span>|<span data-ttu-id="e4aeb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e4aeb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4aeb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4aeb-123">Authorization</span></span>|<span data-ttu-id="e4aeb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4aeb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4aeb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4aeb-125">Accept</span></span>|<span data-ttu-id="e4aeb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4aeb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4aeb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4aeb-127">Request body</span></span>
<span data-ttu-id="e4aeb-128">В корпусе запроса поставляем представление JSON для [объекта deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e4aeb-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="e4aeb-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e4aeb-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="e4aeb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4aeb-130">Property</span></span>|<span data-ttu-id="e4aeb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e4aeb-131">Type</span></span>|<span data-ttu-id="e4aeb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e4aeb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4aeb-133">id</span><span class="sxs-lookup"><span data-stu-id="e4aeb-133">id</span></span>|<span data-ttu-id="e4aeb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e4aeb-134">String</span></span>|<span data-ttu-id="e4aeb-135">The ID</span><span class="sxs-lookup"><span data-stu-id="e4aeb-135">The ID</span></span>|
|<span data-ttu-id="e4aeb-136">settingName</span><span class="sxs-lookup"><span data-stu-id="e4aeb-136">settingName</span></span>|<span data-ttu-id="e4aeb-137">String</span><span class="sxs-lookup"><span data-stu-id="e4aeb-137">String</span></span>|<span data-ttu-id="e4aeb-138">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="e4aeb-138">Name of a setting</span></span>|
|<span data-ttu-id="e4aeb-139">compliantCount</span><span class="sxs-lookup"><span data-stu-id="e4aeb-139">compliantCount</span></span>|<span data-ttu-id="e4aeb-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e4aeb-140">Int32</span></span>|<span data-ttu-id="e4aeb-141">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="e4aeb-141">Number of compliant devices</span></span>|
|<span data-ttu-id="e4aeb-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="e4aeb-142">conflictCount</span></span>|<span data-ttu-id="e4aeb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e4aeb-143">Int32</span></span>|<span data-ttu-id="e4aeb-144">Количество устройств в конфликте</span><span class="sxs-lookup"><span data-stu-id="e4aeb-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="e4aeb-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="e4aeb-145">errorCount</span></span>|<span data-ttu-id="e4aeb-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e4aeb-146">Int32</span></span>|<span data-ttu-id="e4aeb-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e4aeb-147">Number of error devices</span></span>|
|<span data-ttu-id="e4aeb-148">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="e4aeb-148">nonCompliantCount</span></span>|<span data-ttu-id="e4aeb-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e4aeb-149">Int32</span></span>|<span data-ttu-id="e4aeb-150">Число устройств, не совместимых с соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="e4aeb-150">Number of non compliant devices</span></span>|
|<span data-ttu-id="e4aeb-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e4aeb-151">notApplicableCount</span></span>|<span data-ttu-id="e4aeb-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e4aeb-152">Int32</span></span>|<span data-ttu-id="e4aeb-153">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="e4aeb-153">Number of not applicable devices</span></span>|
|<span data-ttu-id="e4aeb-154">исправленоКоунт</span><span class="sxs-lookup"><span data-stu-id="e4aeb-154">remediatedCount</span></span>|<span data-ttu-id="e4aeb-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e4aeb-155">Int32</span></span>|<span data-ttu-id="e4aeb-156">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="e4aeb-156">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="e4aeb-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4aeb-157">Response</span></span>
<span data-ttu-id="e4aeb-158">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e4aeb-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4aeb-159">Пример</span><span class="sxs-lookup"><span data-stu-id="e4aeb-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4aeb-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4aeb-160">Request</span></span>
<span data-ttu-id="e4aeb-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4aeb-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
Content-type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```

### <a name="response"></a><span data-ttu-id="e4aeb-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4aeb-162">Response</span></span>
<span data-ttu-id="e4aeb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4aeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "d3d3a75f-a75f-d3d3-5fa7-d3d35fa7d3d3",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```




