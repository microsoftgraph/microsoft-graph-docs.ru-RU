---
title: Обновление Адванцедсреатпротектиононбоардингстатесуммари
description: Обновление свойств объекта Адванцедсреатпротектиононбоардингстатесуммари.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b5a9641d107048b5cd93cb13239d05339f330f4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759999"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="3344b-103">Обновление Адванцедсреатпротектиононбоардингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="3344b-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="3344b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3344b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3344b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3344b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3344b-106">Обновление свойств объекта [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3344b-106">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3344b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3344b-107">Prerequisites</span></span>
<span data-ttu-id="3344b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3344b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3344b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3344b-110">Permission type</span></span>|<span data-ttu-id="3344b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3344b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3344b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3344b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3344b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3344b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3344b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3344b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3344b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3344b-115">Not supported.</span></span>|
|<span data-ttu-id="3344b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3344b-116">Application</span></span>|<span data-ttu-id="3344b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3344b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3344b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3344b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="3344b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3344b-119">Request headers</span></span>
|<span data-ttu-id="3344b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3344b-120">Header</span></span>|<span data-ttu-id="3344b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3344b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3344b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3344b-122">Authorization</span></span>|<span data-ttu-id="3344b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3344b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3344b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3344b-124">Accept</span></span>|<span data-ttu-id="3344b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3344b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3344b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3344b-126">Request body</span></span>
<span data-ttu-id="3344b-127">В тексте запроса добавьте представление объекта [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3344b-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="3344b-128">В следующей таблице приведены свойства, необходимые при создании [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3344b-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="3344b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3344b-129">Property</span></span>|<span data-ttu-id="3344b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3344b-130">Type</span></span>|<span data-ttu-id="3344b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3344b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3344b-132">id</span><span class="sxs-lookup"><span data-stu-id="3344b-132">id</span></span>|<span data-ttu-id="3344b-133">String</span><span class="sxs-lookup"><span data-stu-id="3344b-133">String</span></span>|<span data-ttu-id="3344b-134">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="3344b-134">Unique Identifier</span></span>|
|<span data-ttu-id="3344b-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3344b-135">unknownDeviceCount</span></span>|<span data-ttu-id="3344b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3344b-136">Int32</span></span>|<span data-ttu-id="3344b-137">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="3344b-137">Number of unknown devices</span></span>|
|<span data-ttu-id="3344b-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3344b-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="3344b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3344b-139">Int32</span></span>|<span data-ttu-id="3344b-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="3344b-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="3344b-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3344b-141">compliantDeviceCount</span></span>|<span data-ttu-id="3344b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3344b-142">Int32</span></span>|<span data-ttu-id="3344b-143">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3344b-143">Number of compliant devices</span></span>|
|<span data-ttu-id="3344b-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3344b-144">remediatedDeviceCount</span></span>|<span data-ttu-id="3344b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3344b-145">Int32</span></span>|<span data-ttu-id="3344b-146">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="3344b-146">Number of remediated devices</span></span>|
|<span data-ttu-id="3344b-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3344b-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3344b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3344b-148">Int32</span></span>|<span data-ttu-id="3344b-149">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3344b-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="3344b-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3344b-150">errorDeviceCount</span></span>|<span data-ttu-id="3344b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="3344b-151">Int32</span></span>|<span data-ttu-id="3344b-152">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="3344b-152">Number of error devices</span></span>|
|<span data-ttu-id="3344b-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3344b-153">conflictDeviceCount</span></span>|<span data-ttu-id="3344b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="3344b-154">Int32</span></span>|<span data-ttu-id="3344b-155">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="3344b-155">Number of conflict devices</span></span>|
|<span data-ttu-id="3344b-156">нотассигнеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="3344b-156">notAssignedDeviceCount</span></span>|<span data-ttu-id="3344b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="3344b-157">Int32</span></span>|<span data-ttu-id="3344b-158">Количество неназначенных устройств</span><span class="sxs-lookup"><span data-stu-id="3344b-158">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="3344b-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="3344b-159">Response</span></span>
<span data-ttu-id="3344b-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3344b-160">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3344b-161">Пример</span><span class="sxs-lookup"><span data-stu-id="3344b-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="3344b-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="3344b-162">Request</span></span>
<span data-ttu-id="3344b-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3344b-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```

### <a name="response"></a><span data-ttu-id="3344b-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="3344b-164">Response</span></span>
<span data-ttu-id="3344b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3344b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "74089602-9602-7408-0296-087402960874",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```




