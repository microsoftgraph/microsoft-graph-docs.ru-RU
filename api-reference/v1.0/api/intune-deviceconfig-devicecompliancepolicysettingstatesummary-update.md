---
title: Обновление объекта deviceCompliancePolicySettingStateSummary
description: Обновление свойств объекта deviceCompliancePolicySettingStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca7efcd58256ad56061773355d5c353220f478f8
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368983"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="5a90f-103">Обновление объекта deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="5a90f-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="5a90f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a90f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a90f-105">Обновление свойств объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5a90f-105">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a90f-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5a90f-106">Prerequisites</span></span>
<span data-ttu-id="5a90f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a90f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a90f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a90f-109">Permission type</span></span>|<span data-ttu-id="5a90f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a90f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a90f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a90f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a90f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a90f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a90f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a90f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a90f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a90f-114">Not supported.</span></span>|
|<span data-ttu-id="5a90f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a90f-115">Application</span></span>|<span data-ttu-id="5a90f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a90f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a90f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a90f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="5a90f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a90f-118">Request headers</span></span>
|<span data-ttu-id="5a90f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a90f-119">Header</span></span>|<span data-ttu-id="5a90f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5a90f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a90f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a90f-121">Authorization</span></span>|<span data-ttu-id="5a90f-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a90f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a90f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5a90f-123">Accept</span></span>|<span data-ttu-id="5a90f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5a90f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a90f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a90f-125">Request body</span></span>
<span data-ttu-id="5a90f-126">В теле запроса добавьте представление объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a90f-126">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="5a90f-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5a90f-127">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="5a90f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a90f-128">Property</span></span>|<span data-ttu-id="5a90f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5a90f-129">Type</span></span>|<span data-ttu-id="5a90f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5a90f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a90f-131">id</span><span class="sxs-lookup"><span data-stu-id="5a90f-131">id</span></span>|<span data-ttu-id="5a90f-132">String</span><span class="sxs-lookup"><span data-stu-id="5a90f-132">String</span></span>|<span data-ttu-id="5a90f-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5a90f-133">Key of the entity.</span></span>|
|<span data-ttu-id="5a90f-134">setting</span><span class="sxs-lookup"><span data-stu-id="5a90f-134">setting</span></span>|<span data-ttu-id="5a90f-135">String</span><span class="sxs-lookup"><span data-stu-id="5a90f-135">String</span></span>|<span data-ttu-id="5a90f-136">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="5a90f-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="5a90f-137">settingName</span><span class="sxs-lookup"><span data-stu-id="5a90f-137">settingName</span></span>|<span data-ttu-id="5a90f-138">String</span><span class="sxs-lookup"><span data-stu-id="5a90f-138">String</span></span>|<span data-ttu-id="5a90f-139">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="5a90f-139">Name of the setting.</span></span>|
|<span data-ttu-id="5a90f-140">platformType</span><span class="sxs-lookup"><span data-stu-id="5a90f-140">platformType</span></span>|[<span data-ttu-id="5a90f-141">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="5a90f-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="5a90f-142">Настройка платформы.</span><span class="sxs-lookup"><span data-stu-id="5a90f-142">Setting platform.</span></span> <span data-ttu-id="5a90f-143">Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="5a90f-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="5a90f-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a90f-144">unknownDeviceCount</span></span>|<span data-ttu-id="5a90f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="5a90f-145">Int32</span></span>|<span data-ttu-id="5a90f-146">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="5a90f-146">Number of unknown devices</span></span>|
|<span data-ttu-id="5a90f-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a90f-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="5a90f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="5a90f-148">Int32</span></span>|<span data-ttu-id="5a90f-149">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="5a90f-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="5a90f-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a90f-150">compliantDeviceCount</span></span>|<span data-ttu-id="5a90f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="5a90f-151">Int32</span></span>|<span data-ttu-id="5a90f-152">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="5a90f-152">Number of compliant devices</span></span>|
|<span data-ttu-id="5a90f-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a90f-153">remediatedDeviceCount</span></span>|<span data-ttu-id="5a90f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="5a90f-154">Int32</span></span>|<span data-ttu-id="5a90f-155">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="5a90f-155">Number of remediated devices</span></span>|
|<span data-ttu-id="5a90f-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a90f-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="5a90f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5a90f-157">Int32</span></span>|<span data-ttu-id="5a90f-158">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="5a90f-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="5a90f-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a90f-159">errorDeviceCount</span></span>|<span data-ttu-id="5a90f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="5a90f-160">Int32</span></span>|<span data-ttu-id="5a90f-161">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="5a90f-161">Number of error devices</span></span>|
|<span data-ttu-id="5a90f-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a90f-162">conflictDeviceCount</span></span>|<span data-ttu-id="5a90f-163">Int32</span><span class="sxs-lookup"><span data-stu-id="5a90f-163">Int32</span></span>|<span data-ttu-id="5a90f-164">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="5a90f-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="5a90f-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a90f-165">Response</span></span>
<span data-ttu-id="5a90f-166">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5a90f-166">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a90f-167">Пример</span><span class="sxs-lookup"><span data-stu-id="5a90f-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a90f-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a90f-168">Request</span></span>
<span data-ttu-id="5a90f-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a90f-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="5a90f-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a90f-170">Response</span></span>
<span data-ttu-id="5a90f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a90f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




