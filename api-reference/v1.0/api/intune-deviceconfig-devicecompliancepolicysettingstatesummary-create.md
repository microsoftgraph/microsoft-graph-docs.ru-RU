---
title: Create deviceCompliancePolicySettingStateSummary
description: Создание объекта deviceCompliancePolicySettingStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 947d2b5fe63e2056c8d2a5ea9626334119f71507
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515016"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="82408-103">Create deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="82408-103">Create deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="82408-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82408-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82408-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82408-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82408-106">Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="82408-106">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82408-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="82408-107">Prerequisites</span></span>
<span data-ttu-id="82408-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82408-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82408-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82408-110">Permission type</span></span>|<span data-ttu-id="82408-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82408-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82408-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82408-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82408-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82408-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82408-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82408-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82408-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82408-115">Not supported.</span></span>|
|<span data-ttu-id="82408-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82408-116">Application</span></span>|<span data-ttu-id="82408-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82408-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82408-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82408-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="82408-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="82408-119">Request headers</span></span>
|<span data-ttu-id="82408-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82408-120">Header</span></span>|<span data-ttu-id="82408-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82408-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82408-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82408-122">Authorization</span></span>|<span data-ttu-id="82408-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82408-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82408-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82408-124">Accept</span></span>|<span data-ttu-id="82408-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82408-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82408-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82408-126">Request body</span></span>
<span data-ttu-id="82408-127">В теле запроса добавьте представление объекта deviceCompliancePolicySettingStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82408-127">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="82408-128">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="82408-128">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="82408-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="82408-129">Property</span></span>|<span data-ttu-id="82408-130">Тип</span><span class="sxs-lookup"><span data-stu-id="82408-130">Type</span></span>|<span data-ttu-id="82408-131">Описание</span><span class="sxs-lookup"><span data-stu-id="82408-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82408-132">id</span><span class="sxs-lookup"><span data-stu-id="82408-132">id</span></span>|<span data-ttu-id="82408-133">Строка</span><span class="sxs-lookup"><span data-stu-id="82408-133">String</span></span>|<span data-ttu-id="82408-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="82408-134">Key of the entity.</span></span>|
|<span data-ttu-id="82408-135">setting</span><span class="sxs-lookup"><span data-stu-id="82408-135">setting</span></span>|<span data-ttu-id="82408-136">Строка</span><span class="sxs-lookup"><span data-stu-id="82408-136">String</span></span>|<span data-ttu-id="82408-137">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="82408-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="82408-138">settingName</span><span class="sxs-lookup"><span data-stu-id="82408-138">settingName</span></span>|<span data-ttu-id="82408-139">String</span><span class="sxs-lookup"><span data-stu-id="82408-139">String</span></span>|<span data-ttu-id="82408-140">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="82408-140">Name of the setting.</span></span>|
|<span data-ttu-id="82408-141">platformType</span><span class="sxs-lookup"><span data-stu-id="82408-141">platformType</span></span>|[<span data-ttu-id="82408-142">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="82408-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="82408-143">Настройка платформы.</span><span class="sxs-lookup"><span data-stu-id="82408-143">Setting platform.</span></span> <span data-ttu-id="82408-144">Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="82408-144">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="82408-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82408-145">unknownDeviceCount</span></span>|<span data-ttu-id="82408-146">Int32</span><span class="sxs-lookup"><span data-stu-id="82408-146">Int32</span></span>|<span data-ttu-id="82408-147">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="82408-147">Number of unknown devices</span></span>|
|<span data-ttu-id="82408-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82408-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="82408-149">Int32</span><span class="sxs-lookup"><span data-stu-id="82408-149">Int32</span></span>|<span data-ttu-id="82408-150">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="82408-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="82408-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82408-151">compliantDeviceCount</span></span>|<span data-ttu-id="82408-152">Int32</span><span class="sxs-lookup"><span data-stu-id="82408-152">Int32</span></span>|<span data-ttu-id="82408-153">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="82408-153">Number of compliant devices</span></span>|
|<span data-ttu-id="82408-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82408-154">remediatedDeviceCount</span></span>|<span data-ttu-id="82408-155">Int32</span><span class="sxs-lookup"><span data-stu-id="82408-155">Int32</span></span>|<span data-ttu-id="82408-156">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="82408-156">Number of remediated devices</span></span>|
|<span data-ttu-id="82408-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82408-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="82408-158">Int32</span><span class="sxs-lookup"><span data-stu-id="82408-158">Int32</span></span>|<span data-ttu-id="82408-159">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="82408-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="82408-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82408-160">errorDeviceCount</span></span>|<span data-ttu-id="82408-161">Int32</span><span class="sxs-lookup"><span data-stu-id="82408-161">Int32</span></span>|<span data-ttu-id="82408-162">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="82408-162">Number of error devices</span></span>|
|<span data-ttu-id="82408-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82408-163">conflictDeviceCount</span></span>|<span data-ttu-id="82408-164">Int32</span><span class="sxs-lookup"><span data-stu-id="82408-164">Int32</span></span>|<span data-ttu-id="82408-165">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="82408-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="82408-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="82408-166">Response</span></span>
<span data-ttu-id="82408-167">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="82408-167">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82408-168">Пример</span><span class="sxs-lookup"><span data-stu-id="82408-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="82408-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="82408-169">Request</span></span>
<span data-ttu-id="82408-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82408-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82408-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="82408-171">Response</span></span>
<span data-ttu-id="82408-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82408-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




