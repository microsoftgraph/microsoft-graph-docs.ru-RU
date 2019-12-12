---
title: Обновление Адванцедсреатпротектиононбоардингстатесуммари
description: Обновление свойств объекта Адванцедсреатпротектиононбоардингстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7031ca604c5d0a6391e68f0a4cb6c7972a2d148
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954050"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="8d949-103">Обновление Адванцедсреатпротектиононбоардингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="8d949-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="8d949-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d949-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d949-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d949-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d949-106">Обновление свойств объекта [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="8d949-106">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d949-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d949-107">Prerequisites</span></span>
<span data-ttu-id="8d949-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d949-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d949-110">Permission type</span></span>|<span data-ttu-id="8d949-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d949-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d949-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d949-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d949-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d949-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d949-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d949-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d949-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d949-115">Not supported.</span></span>|
|<span data-ttu-id="8d949-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d949-116">Application</span></span>|<span data-ttu-id="8d949-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d949-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d949-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d949-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="8d949-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8d949-119">Request headers</span></span>
|<span data-ttu-id="8d949-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d949-120">Header</span></span>|<span data-ttu-id="8d949-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8d949-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d949-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d949-122">Authorization</span></span>|<span data-ttu-id="8d949-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d949-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d949-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8d949-124">Accept</span></span>|<span data-ttu-id="8d949-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d949-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d949-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d949-126">Request body</span></span>
<span data-ttu-id="8d949-127">В тексте запроса добавьте представление объекта [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d949-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="8d949-128">В следующей таблице приведены свойства, необходимые при создании [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8d949-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="8d949-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d949-129">Property</span></span>|<span data-ttu-id="8d949-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8d949-130">Type</span></span>|<span data-ttu-id="8d949-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8d949-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d949-132">id</span><span class="sxs-lookup"><span data-stu-id="8d949-132">id</span></span>|<span data-ttu-id="8d949-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8d949-133">String</span></span>|<span data-ttu-id="8d949-134">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="8d949-134">Unique Identifier</span></span>|
|<span data-ttu-id="8d949-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8d949-135">unknownDeviceCount</span></span>|<span data-ttu-id="8d949-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8d949-136">Int32</span></span>|<span data-ttu-id="8d949-137">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="8d949-137">Number of unknown devices</span></span>|
|<span data-ttu-id="8d949-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8d949-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="8d949-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8d949-139">Int32</span></span>|<span data-ttu-id="8d949-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="8d949-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="8d949-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8d949-141">compliantDeviceCount</span></span>|<span data-ttu-id="8d949-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8d949-142">Int32</span></span>|<span data-ttu-id="8d949-143">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="8d949-143">Number of compliant devices</span></span>|
|<span data-ttu-id="8d949-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8d949-144">remediatedDeviceCount</span></span>|<span data-ttu-id="8d949-145">Int32</span><span class="sxs-lookup"><span data-stu-id="8d949-145">Int32</span></span>|<span data-ttu-id="8d949-146">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="8d949-146">Number of remediated devices</span></span>|
|<span data-ttu-id="8d949-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8d949-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8d949-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8d949-148">Int32</span></span>|<span data-ttu-id="8d949-149">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="8d949-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="8d949-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8d949-150">errorDeviceCount</span></span>|<span data-ttu-id="8d949-151">Int32</span><span class="sxs-lookup"><span data-stu-id="8d949-151">Int32</span></span>|<span data-ttu-id="8d949-152">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="8d949-152">Number of error devices</span></span>|
|<span data-ttu-id="8d949-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8d949-153">conflictDeviceCount</span></span>|<span data-ttu-id="8d949-154">Int32</span><span class="sxs-lookup"><span data-stu-id="8d949-154">Int32</span></span>|<span data-ttu-id="8d949-155">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="8d949-155">Number of conflict devices</span></span>|
|<span data-ttu-id="8d949-156">нотассигнеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="8d949-156">notAssignedDeviceCount</span></span>|<span data-ttu-id="8d949-157">Int32</span><span class="sxs-lookup"><span data-stu-id="8d949-157">Int32</span></span>|<span data-ttu-id="8d949-158">Количество неназначенных устройств</span><span class="sxs-lookup"><span data-stu-id="8d949-158">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="8d949-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d949-159">Response</span></span>
<span data-ttu-id="8d949-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d949-160">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d949-161">Пример</span><span class="sxs-lookup"><span data-stu-id="8d949-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d949-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d949-162">Request</span></span>
<span data-ttu-id="8d949-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d949-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8d949-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d949-164">Response</span></span>
<span data-ttu-id="8d949-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d949-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





