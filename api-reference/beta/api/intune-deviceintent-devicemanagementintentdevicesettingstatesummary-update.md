---
title: Обновление Девицеманажементинтентдевицесеттингстатесуммари
description: Обновление свойств объекта Девицеманажементинтентдевицесеттингстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bcf05f6906d15eadbba9b8eba82b21667707222a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471010"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="1117b-103">Обновление Девицеманажементинтентдевицесеттингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="1117b-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="1117b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1117b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1117b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1117b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1117b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1117b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1117b-107">Обновление свойств объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="1117b-107">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1117b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1117b-108">Prerequisites</span></span>
<span data-ttu-id="1117b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1117b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1117b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1117b-111">Permission type</span></span>|<span data-ttu-id="1117b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1117b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1117b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1117b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1117b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1117b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1117b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1117b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1117b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1117b-116">Not supported.</span></span>|
|<span data-ttu-id="1117b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1117b-117">Application</span></span>|<span data-ttu-id="1117b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1117b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1117b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1117b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="1117b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1117b-120">Request headers</span></span>
|<span data-ttu-id="1117b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1117b-121">Header</span></span>|<span data-ttu-id="1117b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1117b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1117b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1117b-123">Authorization</span></span>|<span data-ttu-id="1117b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1117b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1117b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1117b-125">Accept</span></span>|<span data-ttu-id="1117b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1117b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1117b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1117b-127">Request body</span></span>
<span data-ttu-id="1117b-128">В тексте запроса добавьте представление объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1117b-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="1117b-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1117b-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="1117b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1117b-130">Property</span></span>|<span data-ttu-id="1117b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1117b-131">Type</span></span>|<span data-ttu-id="1117b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1117b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1117b-133">id</span><span class="sxs-lookup"><span data-stu-id="1117b-133">id</span></span>|<span data-ttu-id="1117b-134">String</span><span class="sxs-lookup"><span data-stu-id="1117b-134">String</span></span>|<span data-ttu-id="1117b-135">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="1117b-135">The ID</span></span>|
|<span data-ttu-id="1117b-136">settingName</span><span class="sxs-lookup"><span data-stu-id="1117b-136">settingName</span></span>|<span data-ttu-id="1117b-137">String</span><span class="sxs-lookup"><span data-stu-id="1117b-137">String</span></span>|<span data-ttu-id="1117b-138">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="1117b-138">Name of a setting</span></span>|
|<span data-ttu-id="1117b-139">комплианткаунт</span><span class="sxs-lookup"><span data-stu-id="1117b-139">compliantCount</span></span>|<span data-ttu-id="1117b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1117b-140">Int32</span></span>|<span data-ttu-id="1117b-141">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="1117b-141">Number of compliant devices</span></span>|
|<span data-ttu-id="1117b-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="1117b-142">conflictCount</span></span>|<span data-ttu-id="1117b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1117b-143">Int32</span></span>|<span data-ttu-id="1117b-144">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="1117b-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="1117b-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="1117b-145">errorCount</span></span>|<span data-ttu-id="1117b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1117b-146">Int32</span></span>|<span data-ttu-id="1117b-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="1117b-147">Number of error devices</span></span>|
|<span data-ttu-id="1117b-148">нонкомплианткаунт</span><span class="sxs-lookup"><span data-stu-id="1117b-148">nonCompliantCount</span></span>|<span data-ttu-id="1117b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1117b-149">Int32</span></span>|<span data-ttu-id="1117b-150">Количество устройств, не соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="1117b-150">Number of non compliant devices</span></span>|
|<span data-ttu-id="1117b-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1117b-151">notApplicableCount</span></span>|<span data-ttu-id="1117b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1117b-152">Int32</span></span>|<span data-ttu-id="1117b-153">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="1117b-153">Number of not applicable devices</span></span>|
|<span data-ttu-id="1117b-154">ремедиатедкаунт</span><span class="sxs-lookup"><span data-stu-id="1117b-154">remediatedCount</span></span>|<span data-ttu-id="1117b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="1117b-155">Int32</span></span>|<span data-ttu-id="1117b-156">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="1117b-156">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="1117b-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="1117b-157">Response</span></span>
<span data-ttu-id="1117b-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1117b-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1117b-159">Пример</span><span class="sxs-lookup"><span data-stu-id="1117b-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="1117b-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="1117b-160">Request</span></span>
<span data-ttu-id="1117b-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1117b-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1117b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="1117b-162">Response</span></span>
<span data-ttu-id="1117b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1117b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





