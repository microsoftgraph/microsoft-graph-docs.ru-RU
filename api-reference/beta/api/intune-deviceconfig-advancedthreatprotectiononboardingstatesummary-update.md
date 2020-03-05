---
title: Обновление Адванцедсреатпротектиононбоардингстатесуммари
description: Обновление свойств объекта Адванцедсреатпротектиононбоардингстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 002ba03a5ea0681b1c88598f9e6f20885ad8b762
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450148"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="bb0a4-103">Обновление Адванцедсреатпротектиононбоардингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="bb0a4-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

<span data-ttu-id="bb0a4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bb0a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb0a4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb0a4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb0a4-107">Обновление свойств объекта [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="bb0a4-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb0a4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bb0a4-108">Prerequisites</span></span>
<span data-ttu-id="bb0a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb0a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb0a4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb0a4-111">Permission type</span></span>|<span data-ttu-id="bb0a4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb0a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb0a4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb0a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb0a4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb0a4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb0a4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb0a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb0a4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-116">Not supported.</span></span>|
|<span data-ttu-id="bb0a4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb0a4-117">Application</span></span>|<span data-ttu-id="bb0a4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb0a4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb0a4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb0a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="bb0a4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb0a4-120">Request headers</span></span>
|<span data-ttu-id="bb0a4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb0a4-121">Header</span></span>|<span data-ttu-id="bb0a4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bb0a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb0a4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb0a4-123">Authorization</span></span>|<span data-ttu-id="bb0a4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb0a4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bb0a4-125">Accept</span></span>|<span data-ttu-id="bb0a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb0a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb0a4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb0a4-127">Request body</span></span>
<span data-ttu-id="bb0a4-128">В тексте запроса добавьте представление объекта [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="bb0a4-129">В следующей таблице приведены свойства, необходимые при создании [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bb0a4-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="bb0a4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb0a4-130">Property</span></span>|<span data-ttu-id="bb0a4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bb0a4-131">Type</span></span>|<span data-ttu-id="bb0a4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bb0a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb0a4-133">id</span><span class="sxs-lookup"><span data-stu-id="bb0a4-133">id</span></span>|<span data-ttu-id="bb0a4-134">String</span><span class="sxs-lookup"><span data-stu-id="bb0a4-134">String</span></span>|<span data-ttu-id="bb0a4-135">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-135">Unique Identifier</span></span>|
|<span data-ttu-id="bb0a4-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb0a4-136">unknownDeviceCount</span></span>|<span data-ttu-id="bb0a4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="bb0a4-137">Int32</span></span>|<span data-ttu-id="bb0a4-138">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-138">Number of unknown devices</span></span>|
|<span data-ttu-id="bb0a4-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb0a4-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="bb0a4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="bb0a4-140">Int32</span></span>|<span data-ttu-id="bb0a4-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="bb0a4-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb0a4-142">compliantDeviceCount</span></span>|<span data-ttu-id="bb0a4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="bb0a4-143">Int32</span></span>|<span data-ttu-id="bb0a4-144">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-144">Number of compliant devices</span></span>|
|<span data-ttu-id="bb0a4-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb0a4-145">remediatedDeviceCount</span></span>|<span data-ttu-id="bb0a4-146">Int32</span><span class="sxs-lookup"><span data-stu-id="bb0a4-146">Int32</span></span>|<span data-ttu-id="bb0a4-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-147">Number of remediated devices</span></span>|
|<span data-ttu-id="bb0a4-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb0a4-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="bb0a4-149">Int32</span><span class="sxs-lookup"><span data-stu-id="bb0a4-149">Int32</span></span>|<span data-ttu-id="bb0a4-150">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="bb0a4-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb0a4-151">errorDeviceCount</span></span>|<span data-ttu-id="bb0a4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bb0a4-152">Int32</span></span>|<span data-ttu-id="bb0a4-153">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-153">Number of error devices</span></span>|
|<span data-ttu-id="bb0a4-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb0a4-154">conflictDeviceCount</span></span>|<span data-ttu-id="bb0a4-155">Int32</span><span class="sxs-lookup"><span data-stu-id="bb0a4-155">Int32</span></span>|<span data-ttu-id="bb0a4-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-156">Number of conflict devices</span></span>|
|<span data-ttu-id="bb0a4-157">нотассигнеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="bb0a4-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="bb0a4-158">Int32</span><span class="sxs-lookup"><span data-stu-id="bb0a4-158">Int32</span></span>|<span data-ttu-id="bb0a4-159">Количество неназначенных устройств</span><span class="sxs-lookup"><span data-stu-id="bb0a4-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="bb0a4-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb0a4-160">Response</span></span>
<span data-ttu-id="bb0a4-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb0a4-162">Пример</span><span class="sxs-lookup"><span data-stu-id="bb0a4-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb0a4-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb0a4-163">Request</span></span>
<span data-ttu-id="bb0a4-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb0a4-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb0a4-165">Response</span></span>
<span data-ttu-id="bb0a4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb0a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





