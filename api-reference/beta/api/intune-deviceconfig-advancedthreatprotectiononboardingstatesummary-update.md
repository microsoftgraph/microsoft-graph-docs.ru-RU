---
title: Обновление Адванцедсреатпротектиононбоардингстатесуммари
description: Обновление свойств объекта Адванцедсреатпротектиононбоардингстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e016ad6a390d09466bf4956c585911669437f82b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958471"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="d542e-103">Обновление Адванцедсреатпротектиононбоардингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="d542e-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="d542e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d542e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d542e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d542e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d542e-106">Обновление свойств объекта [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d542e-106">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d542e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d542e-107">Prerequisites</span></span>
<span data-ttu-id="d542e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d542e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d542e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d542e-110">Permission type</span></span>|<span data-ttu-id="d542e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d542e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d542e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d542e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d542e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d542e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d542e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d542e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d542e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d542e-115">Not supported.</span></span>|
|<span data-ttu-id="d542e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d542e-116">Application</span></span>|<span data-ttu-id="d542e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d542e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d542e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d542e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="d542e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d542e-119">Request headers</span></span>
|<span data-ttu-id="d542e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d542e-120">Header</span></span>|<span data-ttu-id="d542e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d542e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d542e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d542e-122">Authorization</span></span>|<span data-ttu-id="d542e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d542e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d542e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d542e-124">Accept</span></span>|<span data-ttu-id="d542e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d542e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d542e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d542e-126">Request body</span></span>
<span data-ttu-id="d542e-127">В тексте запроса добавьте представление объекта [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d542e-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="d542e-128">В следующей таблице приведены свойства, необходимые при создании [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d542e-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="d542e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d542e-129">Property</span></span>|<span data-ttu-id="d542e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d542e-130">Type</span></span>|<span data-ttu-id="d542e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d542e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d542e-132">id</span><span class="sxs-lookup"><span data-stu-id="d542e-132">id</span></span>|<span data-ttu-id="d542e-133">String</span><span class="sxs-lookup"><span data-stu-id="d542e-133">String</span></span>|<span data-ttu-id="d542e-134">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="d542e-134">Unique Identifier</span></span>|
|<span data-ttu-id="d542e-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d542e-135">unknownDeviceCount</span></span>|<span data-ttu-id="d542e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d542e-136">Int32</span></span>|<span data-ttu-id="d542e-137">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="d542e-137">Number of unknown devices</span></span>|
|<span data-ttu-id="d542e-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d542e-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="d542e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d542e-139">Int32</span></span>|<span data-ttu-id="d542e-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="d542e-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="d542e-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d542e-141">compliantDeviceCount</span></span>|<span data-ttu-id="d542e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d542e-142">Int32</span></span>|<span data-ttu-id="d542e-143">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="d542e-143">Number of compliant devices</span></span>|
|<span data-ttu-id="d542e-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d542e-144">remediatedDeviceCount</span></span>|<span data-ttu-id="d542e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d542e-145">Int32</span></span>|<span data-ttu-id="d542e-146">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="d542e-146">Number of remediated devices</span></span>|
|<span data-ttu-id="d542e-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d542e-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d542e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d542e-148">Int32</span></span>|<span data-ttu-id="d542e-149">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="d542e-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="d542e-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d542e-150">errorDeviceCount</span></span>|<span data-ttu-id="d542e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d542e-151">Int32</span></span>|<span data-ttu-id="d542e-152">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="d542e-152">Number of error devices</span></span>|
|<span data-ttu-id="d542e-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d542e-153">conflictDeviceCount</span></span>|<span data-ttu-id="d542e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d542e-154">Int32</span></span>|<span data-ttu-id="d542e-155">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="d542e-155">Number of conflict devices</span></span>|
|<span data-ttu-id="d542e-156">Нотассигнеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="d542e-156">notAssignedDeviceCount</span></span>|<span data-ttu-id="d542e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="d542e-157">Int32</span></span>|<span data-ttu-id="d542e-158">Количество неназначенных устройств</span><span class="sxs-lookup"><span data-stu-id="d542e-158">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="d542e-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="d542e-159">Response</span></span>
<span data-ttu-id="d542e-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [адванцедсреатпротектиононбоардингстатесуммари](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d542e-160">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d542e-161">Пример</span><span class="sxs-lookup"><span data-stu-id="d542e-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="d542e-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="d542e-162">Request</span></span>
<span data-ttu-id="d542e-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d542e-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d542e-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="d542e-164">Response</span></span>
<span data-ttu-id="d542e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d542e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





