---
title: Обновление объекта deviceCompliancePolicySettingStateSummary
description: Обновление свойств объекта deviceCompliancePolicySettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ceb3cec5557270057cb2137148fcc64e6811977b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723660"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="218c1-103">Обновление объекта deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="218c1-103">Update deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="218c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="218c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="218c1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="218c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="218c1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="218c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="218c1-107">Обновление свойств объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="218c1-107">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="218c1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="218c1-108">Prerequisites</span></span>
<span data-ttu-id="218c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="218c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="218c1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="218c1-111">Permission type</span></span>|<span data-ttu-id="218c1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="218c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="218c1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="218c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="218c1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="218c1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="218c1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="218c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="218c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="218c1-116">Not supported.</span></span>|
|<span data-ttu-id="218c1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="218c1-117">Application</span></span>|<span data-ttu-id="218c1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="218c1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="218c1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="218c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="218c1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="218c1-120">Request headers</span></span>
|<span data-ttu-id="218c1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="218c1-121">Header</span></span>|<span data-ttu-id="218c1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="218c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="218c1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="218c1-123">Authorization</span></span>|<span data-ttu-id="218c1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="218c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="218c1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="218c1-125">Accept</span></span>|<span data-ttu-id="218c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="218c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="218c1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="218c1-127">Request body</span></span>
<span data-ttu-id="218c1-128">В теле запроса добавьте представление объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="218c1-128">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="218c1-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="218c1-129">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="218c1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="218c1-130">Property</span></span>|<span data-ttu-id="218c1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="218c1-131">Type</span></span>|<span data-ttu-id="218c1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="218c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="218c1-133">id</span><span class="sxs-lookup"><span data-stu-id="218c1-133">id</span></span>|<span data-ttu-id="218c1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="218c1-134">String</span></span>|<span data-ttu-id="218c1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="218c1-135">Key of the entity.</span></span>|
|<span data-ttu-id="218c1-136">setting</span><span class="sxs-lookup"><span data-stu-id="218c1-136">setting</span></span>|<span data-ttu-id="218c1-137">String</span><span class="sxs-lookup"><span data-stu-id="218c1-137">String</span></span>|<span data-ttu-id="218c1-138">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="218c1-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="218c1-139">settingName</span><span class="sxs-lookup"><span data-stu-id="218c1-139">settingName</span></span>|<span data-ttu-id="218c1-140">String</span><span class="sxs-lookup"><span data-stu-id="218c1-140">String</span></span>|<span data-ttu-id="218c1-141">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="218c1-141">Name of the setting.</span></span>|
|<span data-ttu-id="218c1-142">platformType</span><span class="sxs-lookup"><span data-stu-id="218c1-142">platformType</span></span>|[<span data-ttu-id="218c1-143">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="218c1-143">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="218c1-144">Настройка платформы.</span><span class="sxs-lookup"><span data-stu-id="218c1-144">Setting platform.</span></span> <span data-ttu-id="218c1-145">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="218c1-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="218c1-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="218c1-146">unknownDeviceCount</span></span>|<span data-ttu-id="218c1-147">Int32</span><span class="sxs-lookup"><span data-stu-id="218c1-147">Int32</span></span>|<span data-ttu-id="218c1-148">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="218c1-148">Number of unknown devices</span></span>|
|<span data-ttu-id="218c1-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="218c1-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="218c1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="218c1-150">Int32</span></span>|<span data-ttu-id="218c1-151">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="218c1-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="218c1-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="218c1-152">compliantDeviceCount</span></span>|<span data-ttu-id="218c1-153">Int32</span><span class="sxs-lookup"><span data-stu-id="218c1-153">Int32</span></span>|<span data-ttu-id="218c1-154">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="218c1-154">Number of compliant devices</span></span>|
|<span data-ttu-id="218c1-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="218c1-155">remediatedDeviceCount</span></span>|<span data-ttu-id="218c1-156">Int32</span><span class="sxs-lookup"><span data-stu-id="218c1-156">Int32</span></span>|<span data-ttu-id="218c1-157">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="218c1-157">Number of remediated devices</span></span>|
|<span data-ttu-id="218c1-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="218c1-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="218c1-159">Int32</span><span class="sxs-lookup"><span data-stu-id="218c1-159">Int32</span></span>|<span data-ttu-id="218c1-160">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="218c1-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="218c1-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="218c1-161">errorDeviceCount</span></span>|<span data-ttu-id="218c1-162">Int32</span><span class="sxs-lookup"><span data-stu-id="218c1-162">Int32</span></span>|<span data-ttu-id="218c1-163">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="218c1-163">Number of error devices</span></span>|
|<span data-ttu-id="218c1-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="218c1-164">conflictDeviceCount</span></span>|<span data-ttu-id="218c1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="218c1-165">Int32</span></span>|<span data-ttu-id="218c1-166">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="218c1-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="218c1-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="218c1-167">Response</span></span>
<span data-ttu-id="218c1-168">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="218c1-168">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="218c1-169">Пример</span><span class="sxs-lookup"><span data-stu-id="218c1-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="218c1-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="218c1-170">Request</span></span>
<span data-ttu-id="218c1-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="218c1-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="218c1-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="218c1-172">Response</span></span>
<span data-ttu-id="218c1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="218c1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





