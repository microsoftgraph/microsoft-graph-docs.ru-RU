---
title: Обновление Девицеманажементинтентдевицесеттингстатесуммари
description: Обновление свойств объекта Девицеманажементинтентдевицесеттингстатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f4fb26c4e4a60cde2aade117155402f7181232c0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690996"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="6004b-103">Обновление Девицеманажементинтентдевицесеттингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="6004b-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="6004b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6004b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6004b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6004b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6004b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6004b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6004b-107">Обновление свойств объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="6004b-107">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6004b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6004b-108">Prerequisites</span></span>
<span data-ttu-id="6004b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6004b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6004b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6004b-111">Permission type</span></span>|<span data-ttu-id="6004b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6004b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6004b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6004b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6004b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6004b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6004b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6004b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6004b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6004b-116">Not supported.</span></span>|
|<span data-ttu-id="6004b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6004b-117">Application</span></span>|<span data-ttu-id="6004b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6004b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6004b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6004b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="6004b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6004b-120">Request headers</span></span>
|<span data-ttu-id="6004b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6004b-121">Header</span></span>|<span data-ttu-id="6004b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6004b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6004b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6004b-123">Authorization</span></span>|<span data-ttu-id="6004b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6004b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6004b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6004b-125">Accept</span></span>|<span data-ttu-id="6004b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6004b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6004b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6004b-127">Request body</span></span>
<span data-ttu-id="6004b-128">В тексте запроса добавьте представление объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6004b-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="6004b-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6004b-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="6004b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6004b-130">Property</span></span>|<span data-ttu-id="6004b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6004b-131">Type</span></span>|<span data-ttu-id="6004b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6004b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6004b-133">id</span><span class="sxs-lookup"><span data-stu-id="6004b-133">id</span></span>|<span data-ttu-id="6004b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6004b-134">String</span></span>|<span data-ttu-id="6004b-135">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="6004b-135">The ID</span></span>|
|<span data-ttu-id="6004b-136">settingName</span><span class="sxs-lookup"><span data-stu-id="6004b-136">settingName</span></span>|<span data-ttu-id="6004b-137">String</span><span class="sxs-lookup"><span data-stu-id="6004b-137">String</span></span>|<span data-ttu-id="6004b-138">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="6004b-138">Name of a setting</span></span>|
|<span data-ttu-id="6004b-139">комплианткаунт</span><span class="sxs-lookup"><span data-stu-id="6004b-139">compliantCount</span></span>|<span data-ttu-id="6004b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6004b-140">Int32</span></span>|<span data-ttu-id="6004b-141">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="6004b-141">Number of compliant devices</span></span>|
|<span data-ttu-id="6004b-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="6004b-142">conflictCount</span></span>|<span data-ttu-id="6004b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6004b-143">Int32</span></span>|<span data-ttu-id="6004b-144">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="6004b-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="6004b-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="6004b-145">errorCount</span></span>|<span data-ttu-id="6004b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6004b-146">Int32</span></span>|<span data-ttu-id="6004b-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="6004b-147">Number of error devices</span></span>|
|<span data-ttu-id="6004b-148">нонкомплианткаунт</span><span class="sxs-lookup"><span data-stu-id="6004b-148">nonCompliantCount</span></span>|<span data-ttu-id="6004b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6004b-149">Int32</span></span>|<span data-ttu-id="6004b-150">Количество устройств, не соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="6004b-150">Number of non compliant devices</span></span>|
|<span data-ttu-id="6004b-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6004b-151">notApplicableCount</span></span>|<span data-ttu-id="6004b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6004b-152">Int32</span></span>|<span data-ttu-id="6004b-153">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="6004b-153">Number of not applicable devices</span></span>|
|<span data-ttu-id="6004b-154">ремедиатедкаунт</span><span class="sxs-lookup"><span data-stu-id="6004b-154">remediatedCount</span></span>|<span data-ttu-id="6004b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6004b-155">Int32</span></span>|<span data-ttu-id="6004b-156">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="6004b-156">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="6004b-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="6004b-157">Response</span></span>
<span data-ttu-id="6004b-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6004b-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6004b-159">Пример</span><span class="sxs-lookup"><span data-stu-id="6004b-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="6004b-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="6004b-160">Request</span></span>
<span data-ttu-id="6004b-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6004b-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6004b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="6004b-162">Response</span></span>
<span data-ttu-id="6004b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6004b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





