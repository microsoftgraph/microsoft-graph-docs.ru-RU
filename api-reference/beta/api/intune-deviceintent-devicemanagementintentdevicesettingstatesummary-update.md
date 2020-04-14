---
title: Обновление Девицеманажементинтентдевицесеттингстатесуммари
description: Обновление свойств объекта Девицеманажементинтентдевицесеттингстатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11c98bfa60a1bdcc8fc24a63d3dfe48bfb797b0d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43326559"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="d3847-103">Обновление Девицеманажементинтентдевицесеттингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="d3847-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="d3847-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3847-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3847-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3847-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3847-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3847-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3847-107">Обновление свойств объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d3847-107">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3847-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d3847-108">Prerequisites</span></span>
<span data-ttu-id="d3847-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3847-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3847-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3847-111">Permission type</span></span>|<span data-ttu-id="d3847-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3847-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3847-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3847-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3847-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3847-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3847-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3847-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3847-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3847-116">Not supported.</span></span>|
|<span data-ttu-id="d3847-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3847-117">Application</span></span>|<span data-ttu-id="d3847-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3847-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3847-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3847-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d3847-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d3847-120">Request headers</span></span>
|<span data-ttu-id="d3847-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3847-121">Header</span></span>|<span data-ttu-id="d3847-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d3847-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3847-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3847-123">Authorization</span></span>|<span data-ttu-id="d3847-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3847-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3847-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3847-125">Accept</span></span>|<span data-ttu-id="d3847-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3847-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3847-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3847-127">Request body</span></span>
<span data-ttu-id="d3847-128">В тексте запроса добавьте представление объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3847-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="d3847-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d3847-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="d3847-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3847-130">Property</span></span>|<span data-ttu-id="d3847-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d3847-131">Type</span></span>|<span data-ttu-id="d3847-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d3847-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3847-133">id</span><span class="sxs-lookup"><span data-stu-id="d3847-133">id</span></span>|<span data-ttu-id="d3847-134">String</span><span class="sxs-lookup"><span data-stu-id="d3847-134">String</span></span>|<span data-ttu-id="d3847-135">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="d3847-135">The ID</span></span>|
|<span data-ttu-id="d3847-136">settingName</span><span class="sxs-lookup"><span data-stu-id="d3847-136">settingName</span></span>|<span data-ttu-id="d3847-137">String</span><span class="sxs-lookup"><span data-stu-id="d3847-137">String</span></span>|<span data-ttu-id="d3847-138">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="d3847-138">Name of a setting</span></span>|
|<span data-ttu-id="d3847-139">комплианткаунт</span><span class="sxs-lookup"><span data-stu-id="d3847-139">compliantCount</span></span>|<span data-ttu-id="d3847-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d3847-140">Int32</span></span>|<span data-ttu-id="d3847-141">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="d3847-141">Number of compliant devices</span></span>|
|<span data-ttu-id="d3847-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d3847-142">conflictCount</span></span>|<span data-ttu-id="d3847-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d3847-143">Int32</span></span>|<span data-ttu-id="d3847-144">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="d3847-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="d3847-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="d3847-145">errorCount</span></span>|<span data-ttu-id="d3847-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d3847-146">Int32</span></span>|<span data-ttu-id="d3847-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="d3847-147">Number of error devices</span></span>|
|<span data-ttu-id="d3847-148">нонкомплианткаунт</span><span class="sxs-lookup"><span data-stu-id="d3847-148">nonCompliantCount</span></span>|<span data-ttu-id="d3847-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d3847-149">Int32</span></span>|<span data-ttu-id="d3847-150">Количество устройств, не соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="d3847-150">Number of non compliant devices</span></span>|
|<span data-ttu-id="d3847-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d3847-151">notApplicableCount</span></span>|<span data-ttu-id="d3847-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d3847-152">Int32</span></span>|<span data-ttu-id="d3847-153">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="d3847-153">Number of not applicable devices</span></span>|
|<span data-ttu-id="d3847-154">ремедиатедкаунт</span><span class="sxs-lookup"><span data-stu-id="d3847-154">remediatedCount</span></span>|<span data-ttu-id="d3847-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d3847-155">Int32</span></span>|<span data-ttu-id="d3847-156">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="d3847-156">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="d3847-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3847-157">Response</span></span>
<span data-ttu-id="d3847-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3847-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3847-159">Пример</span><span class="sxs-lookup"><span data-stu-id="d3847-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3847-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3847-160">Request</span></span>
<span data-ttu-id="d3847-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3847-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3847-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3847-162">Response</span></span>
<span data-ttu-id="d3847-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3847-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



