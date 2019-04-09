---
title: Обновление Девицеманажементинтентдевицестатесуммари
description: Обновление свойств объекта Девицеманажементинтентдевицестатесуммари.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 96c86f9c29eb0f2f200b35ab0346f652b13f970c
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523646"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="b4482-103">Обновление Девицеманажементинтентдевицестатесуммари</span><span class="sxs-lookup"><span data-stu-id="b4482-103">Update deviceManagementIntentDeviceStateSummary</span></span>

> <span data-ttu-id="b4482-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4482-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4482-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4482-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4482-106">Обновление свойств объекта [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b4482-106">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4482-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b4482-107">Prerequisites</span></span>
<span data-ttu-id="b4482-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4482-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4482-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4482-110">Permission type</span></span>|<span data-ttu-id="b4482-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4482-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4482-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4482-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4482-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4482-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4482-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4482-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4482-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4482-115">Not supported.</span></span>|
|<span data-ttu-id="b4482-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4482-116">Application</span></span>|<span data-ttu-id="b4482-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4482-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4482-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4482-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="b4482-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4482-119">Request headers</span></span>
|<span data-ttu-id="b4482-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4482-120">Header</span></span>|<span data-ttu-id="b4482-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b4482-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4482-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4482-122">Authorization</span></span>|<span data-ttu-id="b4482-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4482-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4482-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b4482-124">Accept</span></span>|<span data-ttu-id="b4482-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4482-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4482-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4482-126">Request body</span></span>
<span data-ttu-id="b4482-127">В тексте запроса добавьте представление объекта [Девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4482-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

<span data-ttu-id="b4482-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b4482-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span></span>

|<span data-ttu-id="b4482-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4482-129">Property</span></span>|<span data-ttu-id="b4482-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b4482-130">Type</span></span>|<span data-ttu-id="b4482-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b4482-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4482-132">id</span><span class="sxs-lookup"><span data-stu-id="b4482-132">id</span></span>|<span data-ttu-id="b4482-133">String</span><span class="sxs-lookup"><span data-stu-id="b4482-133">String</span></span>|<span data-ttu-id="b4482-134">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="b4482-134">The ID</span></span>|
|<span data-ttu-id="b4482-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="b4482-135">conflictCount</span></span>|<span data-ttu-id="b4482-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b4482-136">Int32</span></span>|<span data-ttu-id="b4482-137">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="b4482-137">Number of devices in conflict</span></span>|
|<span data-ttu-id="b4482-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="b4482-138">errorCount</span></span>|<span data-ttu-id="b4482-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b4482-139">Int32</span></span>|<span data-ttu-id="b4482-140">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="b4482-140">Number of error devices</span></span>|
|<span data-ttu-id="b4482-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="b4482-141">failedCount</span></span>|<span data-ttu-id="b4482-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b4482-142">Int32</span></span>|<span data-ttu-id="b4482-143">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="b4482-143">Number of failed devices</span></span>|
|<span data-ttu-id="b4482-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b4482-144">notApplicableCount</span></span>|<span data-ttu-id="b4482-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b4482-145">Int32</span></span>|<span data-ttu-id="b4482-146">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="b4482-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="b4482-147">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="b4482-147">notApplicablePlatformCount</span></span>|<span data-ttu-id="b4482-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b4482-148">Int32</span></span>|<span data-ttu-id="b4482-149">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="b4482-149">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="b4482-150">successCount</span><span class="sxs-lookup"><span data-stu-id="b4482-150">successCount</span></span>|<span data-ttu-id="b4482-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b4482-151">Int32</span></span>|<span data-ttu-id="b4482-152">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="b4482-152">Number of succeeded devices</span></span>|



## <a name="response"></a><span data-ttu-id="b4482-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4482-153">Response</span></span>
<span data-ttu-id="b4482-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4482-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4482-155">Пример</span><span class="sxs-lookup"><span data-stu-id="b4482-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4482-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4482-156">Request</span></span>
<span data-ttu-id="b4482-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4482-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4482-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4482-158">Response</span></span>
<span data-ttu-id="b4482-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4482-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







