---
title: Create deviceCompliancePolicySettingStateSummary
description: Создание объекта deviceCompliancePolicySettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c63c4a0f31c2db63db0d3ef65d3516f1cea3528
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399936"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="f9c84-103">Create deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f9c84-103">Create deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="f9c84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9c84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9c84-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9c84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9c84-106">Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f9c84-106">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9c84-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f9c84-107">Prerequisites</span></span>
<span data-ttu-id="f9c84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9c84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9c84-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9c84-110">Permission type</span></span>|<span data-ttu-id="f9c84-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9c84-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9c84-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9c84-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9c84-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9c84-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9c84-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9c84-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9c84-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9c84-115">Not supported.</span></span>|
|<span data-ttu-id="f9c84-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9c84-116">Application</span></span>|<span data-ttu-id="f9c84-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9c84-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9c84-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9c84-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="f9c84-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f9c84-119">Request headers</span></span>
|<span data-ttu-id="f9c84-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9c84-120">Header</span></span>|<span data-ttu-id="f9c84-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f9c84-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9c84-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9c84-122">Authorization</span></span>|<span data-ttu-id="f9c84-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9c84-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9c84-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f9c84-124">Accept</span></span>|<span data-ttu-id="f9c84-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9c84-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9c84-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9c84-126">Request body</span></span>
<span data-ttu-id="f9c84-127">В теле запроса добавьте представление объекта deviceCompliancePolicySettingStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9c84-127">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="f9c84-128">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="f9c84-128">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="f9c84-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9c84-129">Property</span></span>|<span data-ttu-id="f9c84-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f9c84-130">Type</span></span>|<span data-ttu-id="f9c84-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f9c84-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9c84-132">id</span><span class="sxs-lookup"><span data-stu-id="f9c84-132">id</span></span>|<span data-ttu-id="f9c84-133">String</span><span class="sxs-lookup"><span data-stu-id="f9c84-133">String</span></span>|<span data-ttu-id="f9c84-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f9c84-134">Key of the entity.</span></span>|
|<span data-ttu-id="f9c84-135">setting</span><span class="sxs-lookup"><span data-stu-id="f9c84-135">setting</span></span>|<span data-ttu-id="f9c84-136">String</span><span class="sxs-lookup"><span data-stu-id="f9c84-136">String</span></span>|<span data-ttu-id="f9c84-137">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="f9c84-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="f9c84-138">settingName</span><span class="sxs-lookup"><span data-stu-id="f9c84-138">settingName</span></span>|<span data-ttu-id="f9c84-139">String</span><span class="sxs-lookup"><span data-stu-id="f9c84-139">String</span></span>|<span data-ttu-id="f9c84-140">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="f9c84-140">Name of the setting.</span></span>|
|<span data-ttu-id="f9c84-141">platformType</span><span class="sxs-lookup"><span data-stu-id="f9c84-141">platformType</span></span>|[<span data-ttu-id="f9c84-142">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="f9c84-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="f9c84-143">Настройка платформы.</span><span class="sxs-lookup"><span data-stu-id="f9c84-143">Setting platform.</span></span> <span data-ttu-id="f9c84-144">Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="f9c84-144">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="f9c84-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9c84-145">unknownDeviceCount</span></span>|<span data-ttu-id="f9c84-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f9c84-146">Int32</span></span>|<span data-ttu-id="f9c84-147">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="f9c84-147">Number of unknown devices</span></span>|
|<span data-ttu-id="f9c84-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9c84-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="f9c84-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f9c84-149">Int32</span></span>|<span data-ttu-id="f9c84-150">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="f9c84-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="f9c84-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9c84-151">compliantDeviceCount</span></span>|<span data-ttu-id="f9c84-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f9c84-152">Int32</span></span>|<span data-ttu-id="f9c84-153">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f9c84-153">Number of compliant devices</span></span>|
|<span data-ttu-id="f9c84-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9c84-154">remediatedDeviceCount</span></span>|<span data-ttu-id="f9c84-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f9c84-155">Int32</span></span>|<span data-ttu-id="f9c84-156">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="f9c84-156">Number of remediated devices</span></span>|
|<span data-ttu-id="f9c84-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9c84-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f9c84-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f9c84-158">Int32</span></span>|<span data-ttu-id="f9c84-159">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f9c84-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f9c84-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9c84-160">errorDeviceCount</span></span>|<span data-ttu-id="f9c84-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f9c84-161">Int32</span></span>|<span data-ttu-id="f9c84-162">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="f9c84-162">Number of error devices</span></span>|
|<span data-ttu-id="f9c84-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9c84-163">conflictDeviceCount</span></span>|<span data-ttu-id="f9c84-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f9c84-164">Int32</span></span>|<span data-ttu-id="f9c84-165">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="f9c84-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="f9c84-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9c84-166">Response</span></span>
<span data-ttu-id="f9c84-167">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f9c84-167">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9c84-168">Пример</span><span class="sxs-lookup"><span data-stu-id="f9c84-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9c84-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9c84-169">Request</span></span>
<span data-ttu-id="f9c84-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9c84-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9c84-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9c84-171">Response</span></span>
<span data-ttu-id="f9c84-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9c84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






