---
title: Обновление объекта deviceCompliancePolicySettingStateSummary
description: Обновление свойств объекта deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 216c5005b9d6a33e10accccd728f9f0d40e9d2ec
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171913"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="3bdc7-103">Обновление объекта deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="3bdc7-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="3bdc7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bdc7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bdc7-106">Обновление свойств объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3bdc7-106">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bdc7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3bdc7-107">Prerequisites</span></span>
<span data-ttu-id="3bdc7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3bdc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3bdc7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bdc7-110">Permission type</span></span>|<span data-ttu-id="3bdc7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bdc7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bdc7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bdc7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3bdc7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bdc7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3bdc7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bdc7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bdc7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-115">Not supported.</span></span>|
|<span data-ttu-id="3bdc7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bdc7-116">Application</span></span>|<span data-ttu-id="3bdc7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bdc7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bdc7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="3bdc7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bdc7-119">Request headers</span></span>
|<span data-ttu-id="3bdc7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3bdc7-120">Header</span></span>|<span data-ttu-id="3bdc7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3bdc7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bdc7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bdc7-122">Authorization</span></span>|<span data-ttu-id="3bdc7-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3bdc7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bdc7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3bdc7-124">Accept</span></span>|<span data-ttu-id="3bdc7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3bdc7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bdc7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3bdc7-126">Request body</span></span>
<span data-ttu-id="3bdc7-127">В теле запроса добавьте представление объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-127">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="3bdc7-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3bdc7-128">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="3bdc7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3bdc7-129">Property</span></span>|<span data-ttu-id="3bdc7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3bdc7-130">Type</span></span>|<span data-ttu-id="3bdc7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3bdc7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bdc7-132">id</span><span class="sxs-lookup"><span data-stu-id="3bdc7-132">id</span></span>|<span data-ttu-id="3bdc7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="3bdc7-133">String</span></span>|<span data-ttu-id="3bdc7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-134">Key of the entity.</span></span>|
|<span data-ttu-id="3bdc7-135">setting</span><span class="sxs-lookup"><span data-stu-id="3bdc7-135">setting</span></span>|<span data-ttu-id="3bdc7-136">String</span><span class="sxs-lookup"><span data-stu-id="3bdc7-136">String</span></span>|<span data-ttu-id="3bdc7-137">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="3bdc7-138">settingName</span><span class="sxs-lookup"><span data-stu-id="3bdc7-138">settingName</span></span>|<span data-ttu-id="3bdc7-139">String</span><span class="sxs-lookup"><span data-stu-id="3bdc7-139">String</span></span>|<span data-ttu-id="3bdc7-140">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-140">Name of the setting.</span></span>|
|<span data-ttu-id="3bdc7-141">platformType</span><span class="sxs-lookup"><span data-stu-id="3bdc7-141">platformType</span></span>|[<span data-ttu-id="3bdc7-142">Полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="3bdc7-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="3bdc7-143">Настройка платформы.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-143">Setting platform.</span></span> <span data-ttu-id="3bdc7-144">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="3bdc7-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3bdc7-145">unknownDeviceCount</span></span>|<span data-ttu-id="3bdc7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3bdc7-146">Int32</span></span>|<span data-ttu-id="3bdc7-147">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-147">Number of unknown devices</span></span>|
|<span data-ttu-id="3bdc7-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3bdc7-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="3bdc7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3bdc7-149">Int32</span></span>|<span data-ttu-id="3bdc7-150">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="3bdc7-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3bdc7-151">compliantDeviceCount</span></span>|<span data-ttu-id="3bdc7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3bdc7-152">Int32</span></span>|<span data-ttu-id="3bdc7-153">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-153">Number of compliant devices</span></span>|
|<span data-ttu-id="3bdc7-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3bdc7-154">remediatedDeviceCount</span></span>|<span data-ttu-id="3bdc7-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3bdc7-155">Int32</span></span>|<span data-ttu-id="3bdc7-156">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-156">Number of remediated devices</span></span>|
|<span data-ttu-id="3bdc7-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3bdc7-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3bdc7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3bdc7-158">Int32</span></span>|<span data-ttu-id="3bdc7-159">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="3bdc7-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3bdc7-160">errorDeviceCount</span></span>|<span data-ttu-id="3bdc7-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3bdc7-161">Int32</span></span>|<span data-ttu-id="3bdc7-162">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-162">Number of error devices</span></span>|
|<span data-ttu-id="3bdc7-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3bdc7-163">conflictDeviceCount</span></span>|<span data-ttu-id="3bdc7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3bdc7-164">Int32</span></span>|<span data-ttu-id="3bdc7-165">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="3bdc7-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bdc7-166">Response</span></span>
<span data-ttu-id="3bdc7-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-167">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bdc7-168">Пример</span><span class="sxs-lookup"><span data-stu-id="3bdc7-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bdc7-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bdc7-169">Request</span></span>
<span data-ttu-id="3bdc7-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="3bdc7-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="3bdc7-171">Response</span></span>
<span data-ttu-id="3bdc7-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3bdc7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




