---
title: Обновление объекта deviceCompliancePolicySettingStateSummary
description: Обновление свойств объекта deviceCompliancePolicySettingStateSummary.
author: tfitzmac
ms.openlocfilehash: 87fb75ea6e0a059a83f17a06697131e6efa77a97
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351046"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="aaad8-103">Обновление объекта deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="aaad8-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="aaad8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aaad8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aaad8-105">Обновление свойств объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="aaad8-105">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aaad8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aaad8-106">Prerequisites</span></span>
<span data-ttu-id="aaad8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaad8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaad8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaad8-109">Permission type</span></span>|<span data-ttu-id="aaad8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaad8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaad8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaad8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aaad8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaad8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aaad8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaad8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaad8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaad8-114">Not supported.</span></span>|
|<span data-ttu-id="aaad8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaad8-115">Application</span></span>|<span data-ttu-id="aaad8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaad8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaad8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaad8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="aaad8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaad8-118">Request headers</span></span>
|<span data-ttu-id="aaad8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aaad8-119">Header</span></span>|<span data-ttu-id="aaad8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="aaad8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaad8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aaad8-121">Authorization</span></span>|<span data-ttu-id="aaad8-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="aaad8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaad8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="aaad8-123">Accept</span></span>|<span data-ttu-id="aaad8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aaad8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaad8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aaad8-125">Request body</span></span>
<span data-ttu-id="aaad8-126">В теле запроса добавьте представление объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aaad8-126">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="aaad8-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="aaad8-127">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="aaad8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="aaad8-128">Property</span></span>|<span data-ttu-id="aaad8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="aaad8-129">Type</span></span>|<span data-ttu-id="aaad8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="aaad8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaad8-131">id</span><span class="sxs-lookup"><span data-stu-id="aaad8-131">id</span></span>|<span data-ttu-id="aaad8-132">Строка</span><span class="sxs-lookup"><span data-stu-id="aaad8-132">String</span></span>|<span data-ttu-id="aaad8-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aaad8-133">Key of the entity.</span></span>|
|<span data-ttu-id="aaad8-134">setting</span><span class="sxs-lookup"><span data-stu-id="aaad8-134">setting</span></span>|<span data-ttu-id="aaad8-135">String</span><span class="sxs-lookup"><span data-stu-id="aaad8-135">String</span></span>|<span data-ttu-id="aaad8-136">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="aaad8-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="aaad8-137">settingName</span><span class="sxs-lookup"><span data-stu-id="aaad8-137">settingName</span></span>|<span data-ttu-id="aaad8-138">String</span><span class="sxs-lookup"><span data-stu-id="aaad8-138">String</span></span>|<span data-ttu-id="aaad8-139">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="aaad8-139">Name of the setting.</span></span>|
|<span data-ttu-id="aaad8-140">platformType</span><span class="sxs-lookup"><span data-stu-id="aaad8-140">platformType</span></span>|[<span data-ttu-id="aaad8-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="aaad8-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="aaad8-142">Параметр платформы.</span><span class="sxs-lookup"><span data-stu-id="aaad8-142">Setting platform.</span></span> <span data-ttu-id="aaad8-143">Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="aaad8-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="aaad8-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaad8-144">unknownDeviceCount</span></span>|<span data-ttu-id="aaad8-145">Int32</span><span class="sxs-lookup"><span data-stu-id="aaad8-145">Int32</span></span>|<span data-ttu-id="aaad8-146">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="aaad8-146">Number of unknown devices</span></span>|
|<span data-ttu-id="aaad8-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaad8-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="aaad8-148">Int32</span><span class="sxs-lookup"><span data-stu-id="aaad8-148">Int32</span></span>|<span data-ttu-id="aaad8-149">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="aaad8-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="aaad8-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaad8-150">compliantDeviceCount</span></span>|<span data-ttu-id="aaad8-151">Int32</span><span class="sxs-lookup"><span data-stu-id="aaad8-151">Int32</span></span>|<span data-ttu-id="aaad8-152">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="aaad8-152">Number of compliant devices</span></span>|
|<span data-ttu-id="aaad8-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaad8-153">remediatedDeviceCount</span></span>|<span data-ttu-id="aaad8-154">Int32</span><span class="sxs-lookup"><span data-stu-id="aaad8-154">Int32</span></span>|<span data-ttu-id="aaad8-155">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="aaad8-155">Number of remediated devices</span></span>|
|<span data-ttu-id="aaad8-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaad8-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="aaad8-157">Int32</span><span class="sxs-lookup"><span data-stu-id="aaad8-157">Int32</span></span>|<span data-ttu-id="aaad8-158">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="aaad8-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="aaad8-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaad8-159">errorDeviceCount</span></span>|<span data-ttu-id="aaad8-160">Int32</span><span class="sxs-lookup"><span data-stu-id="aaad8-160">Int32</span></span>|<span data-ttu-id="aaad8-161">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="aaad8-161">Number of error devices</span></span>|
|<span data-ttu-id="aaad8-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aaad8-162">conflictDeviceCount</span></span>|<span data-ttu-id="aaad8-163">Int32</span><span class="sxs-lookup"><span data-stu-id="aaad8-163">Int32</span></span>|<span data-ttu-id="aaad8-164">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="aaad8-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="aaad8-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaad8-165">Response</span></span>
<span data-ttu-id="aaad8-166">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aaad8-166">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaad8-167">Пример</span><span class="sxs-lookup"><span data-stu-id="aaad8-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="aaad8-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaad8-168">Request</span></span>
<span data-ttu-id="aaad8-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aaad8-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aaad8-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="aaad8-170">Response</span></span>
<span data-ttu-id="aaad8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="aaad8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



