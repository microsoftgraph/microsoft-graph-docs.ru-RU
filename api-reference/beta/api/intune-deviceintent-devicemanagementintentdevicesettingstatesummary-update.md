---
title: Обновление Девицеманажементинтентдевицесеттингстатесуммари
description: Обновление свойств объекта Девицеманажементинтентдевицесеттингстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52051e44f4aad274fd157cd72ba3d8bf93514ad0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960288"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="c64db-103">Обновление Девицеманажементинтентдевицесеттингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="c64db-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="c64db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c64db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c64db-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c64db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c64db-106">Обновление свойств объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c64db-106">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c64db-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c64db-107">Prerequisites</span></span>
<span data-ttu-id="c64db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c64db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c64db-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c64db-110">Permission type</span></span>|<span data-ttu-id="c64db-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c64db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c64db-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c64db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c64db-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c64db-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c64db-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c64db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c64db-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c64db-115">Not supported.</span></span>|
|<span data-ttu-id="c64db-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c64db-116">Application</span></span>|<span data-ttu-id="c64db-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c64db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c64db-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c64db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="c64db-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c64db-119">Request headers</span></span>
|<span data-ttu-id="c64db-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c64db-120">Header</span></span>|<span data-ttu-id="c64db-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c64db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c64db-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c64db-122">Authorization</span></span>|<span data-ttu-id="c64db-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c64db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c64db-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c64db-124">Accept</span></span>|<span data-ttu-id="c64db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c64db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c64db-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c64db-126">Request body</span></span>
<span data-ttu-id="c64db-127">В тексте запроса добавьте представление объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c64db-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="c64db-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c64db-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="c64db-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c64db-129">Property</span></span>|<span data-ttu-id="c64db-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c64db-130">Type</span></span>|<span data-ttu-id="c64db-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c64db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c64db-132">id</span><span class="sxs-lookup"><span data-stu-id="c64db-132">id</span></span>|<span data-ttu-id="c64db-133">String</span><span class="sxs-lookup"><span data-stu-id="c64db-133">String</span></span>|<span data-ttu-id="c64db-134">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="c64db-134">The ID</span></span>|
|<span data-ttu-id="c64db-135">settingName</span><span class="sxs-lookup"><span data-stu-id="c64db-135">settingName</span></span>|<span data-ttu-id="c64db-136">String</span><span class="sxs-lookup"><span data-stu-id="c64db-136">String</span></span>|<span data-ttu-id="c64db-137">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c64db-137">Name of a setting</span></span>|
|<span data-ttu-id="c64db-138">Комплианткаунт</span><span class="sxs-lookup"><span data-stu-id="c64db-138">compliantCount</span></span>|<span data-ttu-id="c64db-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c64db-139">Int32</span></span>|<span data-ttu-id="c64db-140">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="c64db-140">Number of compliant devices</span></span>|
|<span data-ttu-id="c64db-141">conflictCount</span><span class="sxs-lookup"><span data-stu-id="c64db-141">conflictCount</span></span>|<span data-ttu-id="c64db-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c64db-142">Int32</span></span>|<span data-ttu-id="c64db-143">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="c64db-143">Number of devices in conflict</span></span>|
|<span data-ttu-id="c64db-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="c64db-144">errorCount</span></span>|<span data-ttu-id="c64db-145">Int32</span><span class="sxs-lookup"><span data-stu-id="c64db-145">Int32</span></span>|<span data-ttu-id="c64db-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="c64db-146">Number of error devices</span></span>|
|<span data-ttu-id="c64db-147">Нонкомплианткаунт</span><span class="sxs-lookup"><span data-stu-id="c64db-147">nonCompliantCount</span></span>|<span data-ttu-id="c64db-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c64db-148">Int32</span></span>|<span data-ttu-id="c64db-149">Количество устройств, не соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="c64db-149">Number of non compliant devices</span></span>|
|<span data-ttu-id="c64db-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c64db-150">notApplicableCount</span></span>|<span data-ttu-id="c64db-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c64db-151">Int32</span></span>|<span data-ttu-id="c64db-152">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="c64db-152">Number of not applicable devices</span></span>|
|<span data-ttu-id="c64db-153">Ремедиатедкаунт</span><span class="sxs-lookup"><span data-stu-id="c64db-153">remediatedCount</span></span>|<span data-ttu-id="c64db-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c64db-154">Int32</span></span>|<span data-ttu-id="c64db-155">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="c64db-155">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="c64db-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="c64db-156">Response</span></span>
<span data-ttu-id="c64db-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c64db-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c64db-158">Пример</span><span class="sxs-lookup"><span data-stu-id="c64db-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="c64db-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="c64db-159">Request</span></span>
<span data-ttu-id="c64db-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c64db-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c64db-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="c64db-161">Response</span></span>
<span data-ttu-id="c64db-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c64db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





