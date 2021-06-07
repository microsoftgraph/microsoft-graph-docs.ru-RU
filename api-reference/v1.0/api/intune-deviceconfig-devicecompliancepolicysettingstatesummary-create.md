---
title: Create deviceCompliancePolicySettingStateSummary
description: Создание объекта deviceCompliancePolicySettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cadf4008d8e2c99917192c2bd124a271fe2f4e9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748406"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="4cfe7-103">Create deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="4cfe7-103">Create deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="4cfe7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cfe7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4cfe7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cfe7-106">Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4cfe7-106">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cfe7-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4cfe7-107">Prerequisites</span></span>
<span data-ttu-id="4cfe7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cfe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cfe7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cfe7-110">Permission type</span></span>|<span data-ttu-id="4cfe7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cfe7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cfe7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cfe7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4cfe7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cfe7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4cfe7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cfe7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cfe7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-115">Not supported.</span></span>|
|<span data-ttu-id="4cfe7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4cfe7-116">Application</span></span>|<span data-ttu-id="4cfe7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cfe7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cfe7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cfe7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="4cfe7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4cfe7-119">Request headers</span></span>
|<span data-ttu-id="4cfe7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cfe7-120">Header</span></span>|<span data-ttu-id="4cfe7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4cfe7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cfe7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cfe7-122">Authorization</span></span>|<span data-ttu-id="4cfe7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cfe7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4cfe7-124">Accept</span></span>|<span data-ttu-id="4cfe7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4cfe7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cfe7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4cfe7-126">Request body</span></span>
<span data-ttu-id="4cfe7-127">В теле запроса добавьте представление объекта deviceCompliancePolicySettingStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-127">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="4cfe7-128">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-128">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="4cfe7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cfe7-129">Property</span></span>|<span data-ttu-id="4cfe7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4cfe7-130">Type</span></span>|<span data-ttu-id="4cfe7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4cfe7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cfe7-132">id</span><span class="sxs-lookup"><span data-stu-id="4cfe7-132">id</span></span>|<span data-ttu-id="4cfe7-133">String</span><span class="sxs-lookup"><span data-stu-id="4cfe7-133">String</span></span>|<span data-ttu-id="4cfe7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-134">Key of the entity.</span></span>|
|<span data-ttu-id="4cfe7-135">setting</span><span class="sxs-lookup"><span data-stu-id="4cfe7-135">setting</span></span>|<span data-ttu-id="4cfe7-136">String</span><span class="sxs-lookup"><span data-stu-id="4cfe7-136">String</span></span>|<span data-ttu-id="4cfe7-137">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="4cfe7-138">settingName</span><span class="sxs-lookup"><span data-stu-id="4cfe7-138">settingName</span></span>|<span data-ttu-id="4cfe7-139">String</span><span class="sxs-lookup"><span data-stu-id="4cfe7-139">String</span></span>|<span data-ttu-id="4cfe7-140">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-140">Name of the setting.</span></span>|
|<span data-ttu-id="4cfe7-141">platformType</span><span class="sxs-lookup"><span data-stu-id="4cfe7-141">platformType</span></span>|[<span data-ttu-id="4cfe7-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="4cfe7-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="4cfe7-143">Настройка платформы.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-143">Setting platform.</span></span> <span data-ttu-id="4cfe7-144">Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-144">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="4cfe7-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cfe7-145">unknownDeviceCount</span></span>|<span data-ttu-id="4cfe7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4cfe7-146">Int32</span></span>|<span data-ttu-id="4cfe7-147">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-147">Number of unknown devices</span></span>|
|<span data-ttu-id="4cfe7-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cfe7-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="4cfe7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4cfe7-149">Int32</span></span>|<span data-ttu-id="4cfe7-150">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="4cfe7-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cfe7-151">compliantDeviceCount</span></span>|<span data-ttu-id="4cfe7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4cfe7-152">Int32</span></span>|<span data-ttu-id="4cfe7-153">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-153">Number of compliant devices</span></span>|
|<span data-ttu-id="4cfe7-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cfe7-154">remediatedDeviceCount</span></span>|<span data-ttu-id="4cfe7-155">Int32</span><span class="sxs-lookup"><span data-stu-id="4cfe7-155">Int32</span></span>|<span data-ttu-id="4cfe7-156">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-156">Number of remediated devices</span></span>|
|<span data-ttu-id="4cfe7-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cfe7-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="4cfe7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="4cfe7-158">Int32</span></span>|<span data-ttu-id="4cfe7-159">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="4cfe7-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cfe7-160">errorDeviceCount</span></span>|<span data-ttu-id="4cfe7-161">Int32</span><span class="sxs-lookup"><span data-stu-id="4cfe7-161">Int32</span></span>|<span data-ttu-id="4cfe7-162">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-162">Number of error devices</span></span>|
|<span data-ttu-id="4cfe7-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4cfe7-163">conflictDeviceCount</span></span>|<span data-ttu-id="4cfe7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4cfe7-164">Int32</span></span>|<span data-ttu-id="4cfe7-165">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="4cfe7-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cfe7-166">Response</span></span>
<span data-ttu-id="4cfe7-167">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-167">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cfe7-168">Пример</span><span class="sxs-lookup"><span data-stu-id="4cfe7-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cfe7-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cfe7-169">Request</span></span>
<span data-ttu-id="4cfe7-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="4cfe7-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cfe7-171">Response</span></span>
<span data-ttu-id="4cfe7-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cfe7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




