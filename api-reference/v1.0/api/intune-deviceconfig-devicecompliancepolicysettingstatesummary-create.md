---
title: Create deviceCompliancePolicySettingStateSummary
description: Создание объекта deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bae242af036d4aa6c0613b4ee60be9c21b24becd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818454"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="8e2ee-103">Create deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="8e2ee-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="8e2ee-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e2ee-105">Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8e2ee-105">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e2ee-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8e2ee-106">Prerequisites</span></span>
<span data-ttu-id="8e2ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e2ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e2ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e2ee-109">Permission type</span></span>|<span data-ttu-id="8e2ee-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e2ee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e2ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e2ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e2ee-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e2ee-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e2ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e2ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e2ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-114">Not supported.</span></span>|
|<span data-ttu-id="8e2ee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e2ee-115">Application</span></span>|<span data-ttu-id="8e2ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e2ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e2ee-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="8e2ee-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e2ee-118">Request headers</span></span>
|<span data-ttu-id="8e2ee-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e2ee-119">Header</span></span>|<span data-ttu-id="8e2ee-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8e2ee-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e2ee-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e2ee-121">Authorization</span></span>|<span data-ttu-id="8e2ee-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8e2ee-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e2ee-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8e2ee-123">Accept</span></span>|<span data-ttu-id="8e2ee-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8e2ee-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e2ee-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e2ee-125">Request body</span></span>
<span data-ttu-id="8e2ee-126">В теле запроса добавьте представление объекта deviceCompliancePolicySettingStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-126">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="8e2ee-127">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-127">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="8e2ee-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e2ee-128">Property</span></span>|<span data-ttu-id="8e2ee-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8e2ee-129">Type</span></span>|<span data-ttu-id="8e2ee-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8e2ee-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e2ee-131">id</span><span class="sxs-lookup"><span data-stu-id="8e2ee-131">id</span></span>|<span data-ttu-id="8e2ee-132">Строка</span><span class="sxs-lookup"><span data-stu-id="8e2ee-132">String</span></span>|<span data-ttu-id="8e2ee-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-133">Key of the entity.</span></span>|
|<span data-ttu-id="8e2ee-134">setting</span><span class="sxs-lookup"><span data-stu-id="8e2ee-134">setting</span></span>|<span data-ttu-id="8e2ee-135">String</span><span class="sxs-lookup"><span data-stu-id="8e2ee-135">String</span></span>|<span data-ttu-id="8e2ee-136">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="8e2ee-137">settingName</span><span class="sxs-lookup"><span data-stu-id="8e2ee-137">settingName</span></span>|<span data-ttu-id="8e2ee-138">String</span><span class="sxs-lookup"><span data-stu-id="8e2ee-138">String</span></span>|<span data-ttu-id="8e2ee-139">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-139">Name of the setting.</span></span>|
|<span data-ttu-id="8e2ee-140">platformType</span><span class="sxs-lookup"><span data-stu-id="8e2ee-140">platformType</span></span>|[<span data-ttu-id="8e2ee-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="8e2ee-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="8e2ee-142">Параметр платформы.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-142">Setting platform.</span></span> <span data-ttu-id="8e2ee-143">Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="8e2ee-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e2ee-144">unknownDeviceCount</span></span>|<span data-ttu-id="8e2ee-145">Int32</span><span class="sxs-lookup"><span data-stu-id="8e2ee-145">Int32</span></span>|<span data-ttu-id="8e2ee-146">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-146">Number of unknown devices</span></span>|
|<span data-ttu-id="8e2ee-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e2ee-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="8e2ee-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8e2ee-148">Int32</span></span>|<span data-ttu-id="8e2ee-149">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="8e2ee-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e2ee-150">compliantDeviceCount</span></span>|<span data-ttu-id="8e2ee-151">Int32</span><span class="sxs-lookup"><span data-stu-id="8e2ee-151">Int32</span></span>|<span data-ttu-id="8e2ee-152">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-152">Number of compliant devices</span></span>|
|<span data-ttu-id="8e2ee-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e2ee-153">remediatedDeviceCount</span></span>|<span data-ttu-id="8e2ee-154">Int32</span><span class="sxs-lookup"><span data-stu-id="8e2ee-154">Int32</span></span>|<span data-ttu-id="8e2ee-155">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-155">Number of remediated devices</span></span>|
|<span data-ttu-id="8e2ee-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e2ee-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8e2ee-157">Int32</span><span class="sxs-lookup"><span data-stu-id="8e2ee-157">Int32</span></span>|<span data-ttu-id="8e2ee-158">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="8e2ee-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e2ee-159">errorDeviceCount</span></span>|<span data-ttu-id="8e2ee-160">Int32</span><span class="sxs-lookup"><span data-stu-id="8e2ee-160">Int32</span></span>|<span data-ttu-id="8e2ee-161">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-161">Number of error devices</span></span>|
|<span data-ttu-id="8e2ee-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e2ee-162">conflictDeviceCount</span></span>|<span data-ttu-id="8e2ee-163">Int32</span><span class="sxs-lookup"><span data-stu-id="8e2ee-163">Int32</span></span>|<span data-ttu-id="8e2ee-164">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="8e2ee-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e2ee-165">Response</span></span>
<span data-ttu-id="8e2ee-166">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-166">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e2ee-167">Пример</span><span class="sxs-lookup"><span data-stu-id="8e2ee-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e2ee-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e2ee-168">Request</span></span>
<span data-ttu-id="8e2ee-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e2ee-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e2ee-170">Response</span></span>
<span data-ttu-id="8e2ee-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8e2ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



