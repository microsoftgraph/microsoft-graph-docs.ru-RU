---
title: Обновление Девицеманажементинтентдевицесеттингстатесуммари
description: Обновление свойств объекта Девицеманажементинтентдевицесеттингстатесуммари.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bb1f3458a9fd420bd665728a7a186a23af78abb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787059"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="e6f23-103">Обновление Девицеманажементинтентдевицесеттингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="e6f23-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="e6f23-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6f23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6f23-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6f23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6f23-106">Обновление свойств объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e6f23-106">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6f23-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e6f23-107">Prerequisites</span></span>
<span data-ttu-id="e6f23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6f23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6f23-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6f23-110">Permission type</span></span>|<span data-ttu-id="e6f23-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6f23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6f23-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6f23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6f23-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6f23-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6f23-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6f23-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6f23-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6f23-115">Not supported.</span></span>|
|<span data-ttu-id="e6f23-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6f23-116">Application</span></span>|<span data-ttu-id="e6f23-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6f23-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6f23-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6f23-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="e6f23-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6f23-119">Request headers</span></span>
|<span data-ttu-id="e6f23-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6f23-120">Header</span></span>|<span data-ttu-id="e6f23-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e6f23-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6f23-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6f23-122">Authorization</span></span>|<span data-ttu-id="e6f23-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6f23-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6f23-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e6f23-124">Accept</span></span>|<span data-ttu-id="e6f23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6f23-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6f23-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6f23-126">Request body</span></span>
<span data-ttu-id="e6f23-127">В тексте запроса добавьте представление объекта [Девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6f23-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="e6f23-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e6f23-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="e6f23-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6f23-129">Property</span></span>|<span data-ttu-id="e6f23-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e6f23-130">Type</span></span>|<span data-ttu-id="e6f23-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e6f23-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6f23-132">id</span><span class="sxs-lookup"><span data-stu-id="e6f23-132">id</span></span>|<span data-ttu-id="e6f23-133">String</span><span class="sxs-lookup"><span data-stu-id="e6f23-133">String</span></span>|<span data-ttu-id="e6f23-134">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="e6f23-134">The ID</span></span>|
|<span data-ttu-id="e6f23-135">settingName</span><span class="sxs-lookup"><span data-stu-id="e6f23-135">settingName</span></span>|<span data-ttu-id="e6f23-136">String</span><span class="sxs-lookup"><span data-stu-id="e6f23-136">String</span></span>|<span data-ttu-id="e6f23-137">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="e6f23-137">Name of a setting</span></span>|
|<span data-ttu-id="e6f23-138">Комплианткаунт</span><span class="sxs-lookup"><span data-stu-id="e6f23-138">compliantCount</span></span>|<span data-ttu-id="e6f23-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f23-139">Int32</span></span>|<span data-ttu-id="e6f23-140">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="e6f23-140">Number of compliant devices</span></span>|
|<span data-ttu-id="e6f23-141">conflictCount</span><span class="sxs-lookup"><span data-stu-id="e6f23-141">conflictCount</span></span>|<span data-ttu-id="e6f23-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f23-142">Int32</span></span>|<span data-ttu-id="e6f23-143">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="e6f23-143">Number of devices in conflict</span></span>|
|<span data-ttu-id="e6f23-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="e6f23-144">errorCount</span></span>|<span data-ttu-id="e6f23-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f23-145">Int32</span></span>|<span data-ttu-id="e6f23-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e6f23-146">Number of error devices</span></span>|
|<span data-ttu-id="e6f23-147">Нонкомплианткаунт</span><span class="sxs-lookup"><span data-stu-id="e6f23-147">nonCompliantCount</span></span>|<span data-ttu-id="e6f23-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f23-148">Int32</span></span>|<span data-ttu-id="e6f23-149">Количество устройств, не соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="e6f23-149">Number of non compliant devices</span></span>|
|<span data-ttu-id="e6f23-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e6f23-150">notApplicableCount</span></span>|<span data-ttu-id="e6f23-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f23-151">Int32</span></span>|<span data-ttu-id="e6f23-152">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="e6f23-152">Number of not applicable devices</span></span>|
|<span data-ttu-id="e6f23-153">Ремедиатедкаунт</span><span class="sxs-lookup"><span data-stu-id="e6f23-153">remediatedCount</span></span>|<span data-ttu-id="e6f23-154">Int32</span><span class="sxs-lookup"><span data-stu-id="e6f23-154">Int32</span></span>|<span data-ttu-id="e6f23-155">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="e6f23-155">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="e6f23-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6f23-156">Response</span></span>
<span data-ttu-id="e6f23-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6f23-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6f23-158">Пример</span><span class="sxs-lookup"><span data-stu-id="e6f23-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6f23-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6f23-159">Request</span></span>
<span data-ttu-id="e6f23-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6f23-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e6f23-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6f23-161">Response</span></span>
<span data-ttu-id="e6f23-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6f23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





