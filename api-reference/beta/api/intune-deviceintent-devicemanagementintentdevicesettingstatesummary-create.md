---
title: Создание Девицеманажементинтентдевицесеттингстатесуммари
description: Создание нового объекта Девицеманажементинтентдевицесеттингстатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 187f194080922288d36f9cb5c4a91713e61bc5d2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43326929"
---
# <a name="create-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="03320-103">Создание Девицеманажементинтентдевицесеттингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="03320-103">Create deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="03320-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03320-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03320-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03320-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03320-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03320-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03320-107">Создание нового объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="03320-107">Create a new [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03320-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03320-108">Prerequisites</span></span>
<span data-ttu-id="03320-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03320-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03320-111">Permission type</span></span>|<span data-ttu-id="03320-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03320-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03320-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03320-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03320-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03320-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03320-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03320-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03320-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03320-116">Not supported.</span></span>|
|<span data-ttu-id="03320-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03320-117">Application</span></span>|<span data-ttu-id="03320-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03320-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03320-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03320-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="03320-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03320-120">Request headers</span></span>
|<span data-ttu-id="03320-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03320-121">Header</span></span>|<span data-ttu-id="03320-122">Значение</span><span class="sxs-lookup"><span data-stu-id="03320-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03320-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03320-123">Authorization</span></span>|<span data-ttu-id="03320-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03320-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03320-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03320-125">Accept</span></span>|<span data-ttu-id="03320-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03320-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03320-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03320-127">Request body</span></span>
<span data-ttu-id="03320-128">В тексте запроса добавьте представление объекта Девицеманажементинтентдевицесеттингстатесуммари в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03320-128">In the request body, supply a JSON representation for the deviceManagementIntentDeviceSettingStateSummary object.</span></span>

<span data-ttu-id="03320-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентдевицесеттингстатесуммари.</span><span class="sxs-lookup"><span data-stu-id="03320-129">The following table shows the properties that are required when you create the deviceManagementIntentDeviceSettingStateSummary.</span></span>

|<span data-ttu-id="03320-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="03320-130">Property</span></span>|<span data-ttu-id="03320-131">Тип</span><span class="sxs-lookup"><span data-stu-id="03320-131">Type</span></span>|<span data-ttu-id="03320-132">Описание</span><span class="sxs-lookup"><span data-stu-id="03320-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03320-133">id</span><span class="sxs-lookup"><span data-stu-id="03320-133">id</span></span>|<span data-ttu-id="03320-134">String</span><span class="sxs-lookup"><span data-stu-id="03320-134">String</span></span>|<span data-ttu-id="03320-135">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="03320-135">The ID</span></span>|
|<span data-ttu-id="03320-136">settingName</span><span class="sxs-lookup"><span data-stu-id="03320-136">settingName</span></span>|<span data-ttu-id="03320-137">String</span><span class="sxs-lookup"><span data-stu-id="03320-137">String</span></span>|<span data-ttu-id="03320-138">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="03320-138">Name of a setting</span></span>|
|<span data-ttu-id="03320-139">комплианткаунт</span><span class="sxs-lookup"><span data-stu-id="03320-139">compliantCount</span></span>|<span data-ttu-id="03320-140">Int32</span><span class="sxs-lookup"><span data-stu-id="03320-140">Int32</span></span>|<span data-ttu-id="03320-141">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="03320-141">Number of compliant devices</span></span>|
|<span data-ttu-id="03320-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="03320-142">conflictCount</span></span>|<span data-ttu-id="03320-143">Int32</span><span class="sxs-lookup"><span data-stu-id="03320-143">Int32</span></span>|<span data-ttu-id="03320-144">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="03320-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="03320-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="03320-145">errorCount</span></span>|<span data-ttu-id="03320-146">Int32</span><span class="sxs-lookup"><span data-stu-id="03320-146">Int32</span></span>|<span data-ttu-id="03320-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="03320-147">Number of error devices</span></span>|
|<span data-ttu-id="03320-148">нонкомплианткаунт</span><span class="sxs-lookup"><span data-stu-id="03320-148">nonCompliantCount</span></span>|<span data-ttu-id="03320-149">Int32</span><span class="sxs-lookup"><span data-stu-id="03320-149">Int32</span></span>|<span data-ttu-id="03320-150">Количество устройств, не соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="03320-150">Number of non compliant devices</span></span>|
|<span data-ttu-id="03320-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="03320-151">notApplicableCount</span></span>|<span data-ttu-id="03320-152">Int32</span><span class="sxs-lookup"><span data-stu-id="03320-152">Int32</span></span>|<span data-ttu-id="03320-153">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="03320-153">Number of not applicable devices</span></span>|
|<span data-ttu-id="03320-154">ремедиатедкаунт</span><span class="sxs-lookup"><span data-stu-id="03320-154">remediatedCount</span></span>|<span data-ttu-id="03320-155">Int32</span><span class="sxs-lookup"><span data-stu-id="03320-155">Int32</span></span>|<span data-ttu-id="03320-156">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="03320-156">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="03320-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="03320-157">Response</span></span>
<span data-ttu-id="03320-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03320-158">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03320-159">Пример</span><span class="sxs-lookup"><span data-stu-id="03320-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="03320-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="03320-160">Request</span></span>
<span data-ttu-id="03320-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03320-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="03320-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="03320-162">Response</span></span>
<span data-ttu-id="03320-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03320-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



