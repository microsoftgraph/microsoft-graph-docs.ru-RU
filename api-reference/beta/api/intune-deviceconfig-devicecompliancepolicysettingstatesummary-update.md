---
title: Обновление объекта deviceCompliancePolicySettingStateSummary
description: Обновление свойств объекта deviceCompliancePolicySettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 353bd57cb090994996a536f2f8ed6b74d34c360d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49292102"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="d8ff9-103">Обновление объекта deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="d8ff9-103">Update deviceCompliancePolicySettingStateSummary</span></span>

<span data-ttu-id="d8ff9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8ff9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8ff9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8ff9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8ff9-107">Обновление свойств объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d8ff9-107">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8ff9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d8ff9-108">Prerequisites</span></span>
<span data-ttu-id="d8ff9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8ff9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8ff9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8ff9-111">Permission type</span></span>|<span data-ttu-id="d8ff9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8ff9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8ff9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8ff9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8ff9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ff9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8ff9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8ff9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8ff9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-116">Not supported.</span></span>|
|<span data-ttu-id="d8ff9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8ff9-117">Application</span></span>|<span data-ttu-id="d8ff9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ff9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8ff9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8ff9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d8ff9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d8ff9-120">Request headers</span></span>
|<span data-ttu-id="d8ff9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8ff9-121">Header</span></span>|<span data-ttu-id="d8ff9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d8ff9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8ff9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8ff9-123">Authorization</span></span>|<span data-ttu-id="d8ff9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8ff9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8ff9-125">Accept</span></span>|<span data-ttu-id="d8ff9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8ff9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8ff9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8ff9-127">Request body</span></span>
<span data-ttu-id="d8ff9-128">В теле запроса добавьте представление объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-128">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="d8ff9-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d8ff9-129">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="d8ff9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8ff9-130">Property</span></span>|<span data-ttu-id="d8ff9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d8ff9-131">Type</span></span>|<span data-ttu-id="d8ff9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d8ff9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8ff9-133">id</span><span class="sxs-lookup"><span data-stu-id="d8ff9-133">id</span></span>|<span data-ttu-id="d8ff9-134">String</span><span class="sxs-lookup"><span data-stu-id="d8ff9-134">String</span></span>|<span data-ttu-id="d8ff9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-135">Key of the entity.</span></span>|
|<span data-ttu-id="d8ff9-136">setting</span><span class="sxs-lookup"><span data-stu-id="d8ff9-136">setting</span></span>|<span data-ttu-id="d8ff9-137">String</span><span class="sxs-lookup"><span data-stu-id="d8ff9-137">String</span></span>|<span data-ttu-id="d8ff9-138">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="d8ff9-139">settingName</span><span class="sxs-lookup"><span data-stu-id="d8ff9-139">settingName</span></span>|<span data-ttu-id="d8ff9-140">String</span><span class="sxs-lookup"><span data-stu-id="d8ff9-140">String</span></span>|<span data-ttu-id="d8ff9-141">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-141">Name of the setting.</span></span>|
|<span data-ttu-id="d8ff9-142">platformType</span><span class="sxs-lookup"><span data-stu-id="d8ff9-142">platformType</span></span>|[<span data-ttu-id="d8ff9-143">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="d8ff9-143">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="d8ff9-144">Настройка платформы.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-144">Setting platform.</span></span> <span data-ttu-id="d8ff9-145">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="d8ff9-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8ff9-146">unknownDeviceCount</span></span>|<span data-ttu-id="d8ff9-147">Int32</span><span class="sxs-lookup"><span data-stu-id="d8ff9-147">Int32</span></span>|<span data-ttu-id="d8ff9-148">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-148">Number of unknown devices</span></span>|
|<span data-ttu-id="d8ff9-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8ff9-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="d8ff9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d8ff9-150">Int32</span></span>|<span data-ttu-id="d8ff9-151">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="d8ff9-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8ff9-152">compliantDeviceCount</span></span>|<span data-ttu-id="d8ff9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d8ff9-153">Int32</span></span>|<span data-ttu-id="d8ff9-154">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-154">Number of compliant devices</span></span>|
|<span data-ttu-id="d8ff9-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8ff9-155">remediatedDeviceCount</span></span>|<span data-ttu-id="d8ff9-156">Int32</span><span class="sxs-lookup"><span data-stu-id="d8ff9-156">Int32</span></span>|<span data-ttu-id="d8ff9-157">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-157">Number of remediated devices</span></span>|
|<span data-ttu-id="d8ff9-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8ff9-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d8ff9-159">Int32</span><span class="sxs-lookup"><span data-stu-id="d8ff9-159">Int32</span></span>|<span data-ttu-id="d8ff9-160">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="d8ff9-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8ff9-161">errorDeviceCount</span></span>|<span data-ttu-id="d8ff9-162">Int32</span><span class="sxs-lookup"><span data-stu-id="d8ff9-162">Int32</span></span>|<span data-ttu-id="d8ff9-163">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-163">Number of error devices</span></span>|
|<span data-ttu-id="d8ff9-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8ff9-164">conflictDeviceCount</span></span>|<span data-ttu-id="d8ff9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d8ff9-165">Int32</span></span>|<span data-ttu-id="d8ff9-166">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="d8ff9-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8ff9-167">Response</span></span>
<span data-ttu-id="d8ff9-168">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-168">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8ff9-169">Пример</span><span class="sxs-lookup"><span data-stu-id="d8ff9-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8ff9-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8ff9-170">Request</span></span>
<span data-ttu-id="d8ff9-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d8ff9-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8ff9-172">Response</span></span>
<span data-ttu-id="d8ff9-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8ff9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




