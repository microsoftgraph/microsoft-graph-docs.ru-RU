---
title: Обновление Адванцедсреатпротектиононбоардингстатесуммари
description: Обновление свойств объекта Адванцедсреатпротектиононбоардингстатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 544c7f27b0f498e86b66ef4d72112f75321c90b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990335"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="4cd23-103">Обновление Адванцедсреатпротектиононбоардингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="4cd23-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

<span data-ttu-id="4cd23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cd23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4cd23-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cd23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cd23-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cd23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cd23-107">Обновление свойств объекта [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="4cd23-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cd23-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4cd23-108">Prerequisites</span></span>
<span data-ttu-id="4cd23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cd23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cd23-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cd23-111">Permission type</span></span>|<span data-ttu-id="4cd23-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cd23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cd23-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cd23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4cd23-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cd23-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4cd23-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cd23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cd23-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cd23-116">Not supported.</span></span>|
|<span data-ttu-id="4cd23-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cd23-117">Application</span></span>|<span data-ttu-id="4cd23-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cd23-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cd23-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cd23-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="4cd23-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4cd23-120">Request headers</span></span>
|<span data-ttu-id="4cd23-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cd23-121">Header</span></span>|<span data-ttu-id="4cd23-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4cd23-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cd23-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cd23-123">Authorization</span></span>|<span data-ttu-id="4cd23-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cd23-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cd23-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4cd23-125">Accept</span></span>|<span data-ttu-id="4cd23-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4cd23-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cd23-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4cd23-127">Request body</span></span>
<span data-ttu-id="4cd23-128">В тексте запроса добавьте представление объекта [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cd23-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="4cd23-129">В следующей таблице приведены свойства, необходимые при создании [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4cd23-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="4cd23-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cd23-130">Property</span></span>|<span data-ttu-id="4cd23-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4cd23-131">Type</span></span>|<span data-ttu-id="4cd23-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4cd23-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cd23-133">id</span><span class="sxs-lookup"><span data-stu-id="4cd23-133">id</span></span>|<span data-ttu-id="4cd23-134">String</span><span class="sxs-lookup"><span data-stu-id="4cd23-134">String</span></span>|<span data-ttu-id="4cd23-135">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="4cd23-135">Unique Identifier</span></span>|
|<span data-ttu-id="4cd23-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cd23-136">unknownDeviceCount</span></span>|<span data-ttu-id="4cd23-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4cd23-137">Int32</span></span>|<span data-ttu-id="4cd23-138">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="4cd23-138">Number of unknown devices</span></span>|
|<span data-ttu-id="4cd23-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cd23-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="4cd23-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4cd23-140">Int32</span></span>|<span data-ttu-id="4cd23-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="4cd23-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="4cd23-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cd23-142">compliantDeviceCount</span></span>|<span data-ttu-id="4cd23-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4cd23-143">Int32</span></span>|<span data-ttu-id="4cd23-144">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="4cd23-144">Number of compliant devices</span></span>|
|<span data-ttu-id="4cd23-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cd23-145">remediatedDeviceCount</span></span>|<span data-ttu-id="4cd23-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4cd23-146">Int32</span></span>|<span data-ttu-id="4cd23-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="4cd23-147">Number of remediated devices</span></span>|
|<span data-ttu-id="4cd23-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cd23-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="4cd23-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4cd23-149">Int32</span></span>|<span data-ttu-id="4cd23-150">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="4cd23-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="4cd23-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cd23-151">errorDeviceCount</span></span>|<span data-ttu-id="4cd23-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4cd23-152">Int32</span></span>|<span data-ttu-id="4cd23-153">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="4cd23-153">Number of error devices</span></span>|
|<span data-ttu-id="4cd23-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cd23-154">conflictDeviceCount</span></span>|<span data-ttu-id="4cd23-155">Int32</span><span class="sxs-lookup"><span data-stu-id="4cd23-155">Int32</span></span>|<span data-ttu-id="4cd23-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="4cd23-156">Number of conflict devices</span></span>|
|<span data-ttu-id="4cd23-157">нотассигнеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="4cd23-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="4cd23-158">Int32</span><span class="sxs-lookup"><span data-stu-id="4cd23-158">Int32</span></span>|<span data-ttu-id="4cd23-159">Количество неназначенных устройств</span><span class="sxs-lookup"><span data-stu-id="4cd23-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="4cd23-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cd23-160">Response</span></span>
<span data-ttu-id="4cd23-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4cd23-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cd23-162">Пример</span><span class="sxs-lookup"><span data-stu-id="4cd23-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cd23-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cd23-163">Request</span></span>
<span data-ttu-id="4cd23-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cd23-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4cd23-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cd23-165">Response</span></span>
<span data-ttu-id="4cd23-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cd23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






