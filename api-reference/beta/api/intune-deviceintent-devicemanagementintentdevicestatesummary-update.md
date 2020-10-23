---
title: Обновление Девицеманажементинтентдевицестатесуммари
description: Обновление свойств объекта Девицеманажементинтентдевицестатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3729dd0bbc7ac16fd81e305b442a06f704a459c1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707376"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="6071d-103">Обновление Девицеманажементинтентдевицестатесуммари</span><span class="sxs-lookup"><span data-stu-id="6071d-103">Update deviceManagementIntentDeviceStateSummary</span></span>

<span data-ttu-id="6071d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6071d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6071d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6071d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6071d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6071d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6071d-107">Обновление свойств объекта [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="6071d-107">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6071d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6071d-108">Prerequisites</span></span>
<span data-ttu-id="6071d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6071d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6071d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6071d-111">Permission type</span></span>|<span data-ttu-id="6071d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6071d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6071d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6071d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6071d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6071d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6071d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6071d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6071d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6071d-116">Not supported.</span></span>|
|<span data-ttu-id="6071d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6071d-117">Application</span></span>|<span data-ttu-id="6071d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6071d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6071d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6071d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="6071d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6071d-120">Request headers</span></span>
|<span data-ttu-id="6071d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6071d-121">Header</span></span>|<span data-ttu-id="6071d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6071d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6071d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6071d-123">Authorization</span></span>|<span data-ttu-id="6071d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6071d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6071d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6071d-125">Accept</span></span>|<span data-ttu-id="6071d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6071d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6071d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6071d-127">Request body</span></span>
<span data-ttu-id="6071d-128">В тексте запроса добавьте представление объекта [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6071d-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

<span data-ttu-id="6071d-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6071d-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span></span>

|<span data-ttu-id="6071d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6071d-130">Property</span></span>|<span data-ttu-id="6071d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6071d-131">Type</span></span>|<span data-ttu-id="6071d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6071d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6071d-133">id</span><span class="sxs-lookup"><span data-stu-id="6071d-133">id</span></span>|<span data-ttu-id="6071d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6071d-134">String</span></span>|<span data-ttu-id="6071d-135">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="6071d-135">The ID</span></span>|
|<span data-ttu-id="6071d-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="6071d-136">conflictCount</span></span>|<span data-ttu-id="6071d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6071d-137">Int32</span></span>|<span data-ttu-id="6071d-138">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="6071d-138">Number of devices in conflict</span></span>|
|<span data-ttu-id="6071d-139">errorCount</span><span class="sxs-lookup"><span data-stu-id="6071d-139">errorCount</span></span>|<span data-ttu-id="6071d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6071d-140">Int32</span></span>|<span data-ttu-id="6071d-141">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="6071d-141">Number of error devices</span></span>|
|<span data-ttu-id="6071d-142">failedCount</span><span class="sxs-lookup"><span data-stu-id="6071d-142">failedCount</span></span>|<span data-ttu-id="6071d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6071d-143">Int32</span></span>|<span data-ttu-id="6071d-144">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="6071d-144">Number of failed devices</span></span>|
|<span data-ttu-id="6071d-145">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6071d-145">notApplicableCount</span></span>|<span data-ttu-id="6071d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6071d-146">Int32</span></span>|<span data-ttu-id="6071d-147">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="6071d-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="6071d-148">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="6071d-148">notApplicablePlatformCount</span></span>|<span data-ttu-id="6071d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6071d-149">Int32</span></span>|<span data-ttu-id="6071d-150">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="6071d-150">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="6071d-151">successCount</span><span class="sxs-lookup"><span data-stu-id="6071d-151">successCount</span></span>|<span data-ttu-id="6071d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6071d-152">Int32</span></span>|<span data-ttu-id="6071d-153">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="6071d-153">Number of succeeded devices</span></span>|



## <a name="response"></a><span data-ttu-id="6071d-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="6071d-154">Response</span></span>
<span data-ttu-id="6071d-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6071d-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6071d-156">Пример</span><span class="sxs-lookup"><span data-stu-id="6071d-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="6071d-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="6071d-157">Request</span></span>
<span data-ttu-id="6071d-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6071d-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6071d-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="6071d-159">Response</span></span>
<span data-ttu-id="6071d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6071d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





