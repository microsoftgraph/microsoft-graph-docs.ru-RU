---
title: Обновление объекта deviceCompliancePolicySettingStateSummary
description: Обновление свойств объекта deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 97eec7bba67552c21c208ed087aab40a096d47b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830025"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="e3aa0-103">Обновление объекта deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="e3aa0-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="e3aa0-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3aa0-105">Обновление свойств объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e3aa0-105">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3aa0-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e3aa0-106">Prerequisites</span></span>
<span data-ttu-id="e3aa0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3aa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3aa0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3aa0-109">Permission type</span></span>|<span data-ttu-id="e3aa0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3aa0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3aa0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3aa0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3aa0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3aa0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3aa0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3aa0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3aa0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-114">Not supported.</span></span>|
|<span data-ttu-id="e3aa0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3aa0-115">Application</span></span>|<span data-ttu-id="e3aa0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3aa0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3aa0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="e3aa0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3aa0-118">Request headers</span></span>
|<span data-ttu-id="e3aa0-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3aa0-119">Header</span></span>|<span data-ttu-id="e3aa0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e3aa0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3aa0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3aa0-121">Authorization</span></span>|<span data-ttu-id="e3aa0-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e3aa0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3aa0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e3aa0-123">Accept</span></span>|<span data-ttu-id="e3aa0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3aa0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3aa0-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e3aa0-125">Request body</span></span>
<span data-ttu-id="e3aa0-126">В теле запроса добавьте представление объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-126">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="e3aa0-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e3aa0-127">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="e3aa0-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3aa0-128">Property</span></span>|<span data-ttu-id="e3aa0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e3aa0-129">Type</span></span>|<span data-ttu-id="e3aa0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e3aa0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3aa0-131">id</span><span class="sxs-lookup"><span data-stu-id="e3aa0-131">id</span></span>|<span data-ttu-id="e3aa0-132">Строка</span><span class="sxs-lookup"><span data-stu-id="e3aa0-132">String</span></span>|<span data-ttu-id="e3aa0-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-133">Key of the entity.</span></span>|
|<span data-ttu-id="e3aa0-134">setting</span><span class="sxs-lookup"><span data-stu-id="e3aa0-134">setting</span></span>|<span data-ttu-id="e3aa0-135">String</span><span class="sxs-lookup"><span data-stu-id="e3aa0-135">String</span></span>|<span data-ttu-id="e3aa0-136">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="e3aa0-137">settingName</span><span class="sxs-lookup"><span data-stu-id="e3aa0-137">settingName</span></span>|<span data-ttu-id="e3aa0-138">String</span><span class="sxs-lookup"><span data-stu-id="e3aa0-138">String</span></span>|<span data-ttu-id="e3aa0-139">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-139">Name of the setting.</span></span>|
|<span data-ttu-id="e3aa0-140">platformType</span><span class="sxs-lookup"><span data-stu-id="e3aa0-140">platformType</span></span>|[<span data-ttu-id="e3aa0-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="e3aa0-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="e3aa0-142">Параметр платформы.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-142">Setting platform.</span></span> <span data-ttu-id="e3aa0-143">Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="e3aa0-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3aa0-144">unknownDeviceCount</span></span>|<span data-ttu-id="e3aa0-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e3aa0-145">Int32</span></span>|<span data-ttu-id="e3aa0-146">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-146">Number of unknown devices</span></span>|
|<span data-ttu-id="e3aa0-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3aa0-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="e3aa0-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e3aa0-148">Int32</span></span>|<span data-ttu-id="e3aa0-149">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="e3aa0-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3aa0-150">compliantDeviceCount</span></span>|<span data-ttu-id="e3aa0-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e3aa0-151">Int32</span></span>|<span data-ttu-id="e3aa0-152">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-152">Number of compliant devices</span></span>|
|<span data-ttu-id="e3aa0-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3aa0-153">remediatedDeviceCount</span></span>|<span data-ttu-id="e3aa0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="e3aa0-154">Int32</span></span>|<span data-ttu-id="e3aa0-155">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-155">Number of remediated devices</span></span>|
|<span data-ttu-id="e3aa0-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3aa0-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e3aa0-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e3aa0-157">Int32</span></span>|<span data-ttu-id="e3aa0-158">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e3aa0-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3aa0-159">errorDeviceCount</span></span>|<span data-ttu-id="e3aa0-160">Int32</span><span class="sxs-lookup"><span data-stu-id="e3aa0-160">Int32</span></span>|<span data-ttu-id="e3aa0-161">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-161">Number of error devices</span></span>|
|<span data-ttu-id="e3aa0-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3aa0-162">conflictDeviceCount</span></span>|<span data-ttu-id="e3aa0-163">Int32</span><span class="sxs-lookup"><span data-stu-id="e3aa0-163">Int32</span></span>|<span data-ttu-id="e3aa0-164">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="e3aa0-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3aa0-165">Response</span></span>
<span data-ttu-id="e3aa0-166">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-166">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3aa0-167">Пример</span><span class="sxs-lookup"><span data-stu-id="e3aa0-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3aa0-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3aa0-168">Request</span></span>
<span data-ttu-id="e3aa0-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3aa0-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3aa0-170">Response</span></span>
<span data-ttu-id="e3aa0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e3aa0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



