---
title: Create deviceCompliancePolicySettingStateSummary
description: Создание объекта deviceCompliancePolicySettingStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0858801c8ff049419043bbfc2fc2aa8d75e2da3
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37369011"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="7ec1a-103">Create deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="7ec1a-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="7ec1a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ec1a-105">Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7ec1a-105">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ec1a-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7ec1a-106">Prerequisites</span></span>
<span data-ttu-id="7ec1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ec1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ec1a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ec1a-109">Permission type</span></span>|<span data-ttu-id="7ec1a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ec1a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ec1a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ec1a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7ec1a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ec1a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ec1a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ec1a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ec1a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-114">Not supported.</span></span>|
|<span data-ttu-id="7ec1a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ec1a-115">Application</span></span>|<span data-ttu-id="7ec1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ec1a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ec1a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="7ec1a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ec1a-118">Request headers</span></span>
|<span data-ttu-id="7ec1a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ec1a-119">Header</span></span>|<span data-ttu-id="7ec1a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7ec1a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ec1a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ec1a-121">Authorization</span></span>|<span data-ttu-id="7ec1a-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ec1a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7ec1a-123">Accept</span></span>|<span data-ttu-id="7ec1a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7ec1a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ec1a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ec1a-125">Request body</span></span>
<span data-ttu-id="7ec1a-126">В теле запроса добавьте представление объекта deviceCompliancePolicySettingStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-126">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="7ec1a-127">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-127">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="7ec1a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ec1a-128">Property</span></span>|<span data-ttu-id="7ec1a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7ec1a-129">Type</span></span>|<span data-ttu-id="7ec1a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7ec1a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ec1a-131">id</span><span class="sxs-lookup"><span data-stu-id="7ec1a-131">id</span></span>|<span data-ttu-id="7ec1a-132">String</span><span class="sxs-lookup"><span data-stu-id="7ec1a-132">String</span></span>|<span data-ttu-id="7ec1a-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-133">Key of the entity.</span></span>|
|<span data-ttu-id="7ec1a-134">setting</span><span class="sxs-lookup"><span data-stu-id="7ec1a-134">setting</span></span>|<span data-ttu-id="7ec1a-135">String</span><span class="sxs-lookup"><span data-stu-id="7ec1a-135">String</span></span>|<span data-ttu-id="7ec1a-136">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="7ec1a-137">settingName</span><span class="sxs-lookup"><span data-stu-id="7ec1a-137">settingName</span></span>|<span data-ttu-id="7ec1a-138">String</span><span class="sxs-lookup"><span data-stu-id="7ec1a-138">String</span></span>|<span data-ttu-id="7ec1a-139">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-139">Name of the setting.</span></span>|
|<span data-ttu-id="7ec1a-140">platformType</span><span class="sxs-lookup"><span data-stu-id="7ec1a-140">platformType</span></span>|[<span data-ttu-id="7ec1a-141">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="7ec1a-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="7ec1a-142">Настройка платформы.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-142">Setting platform.</span></span> <span data-ttu-id="7ec1a-143">Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="7ec1a-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec1a-144">unknownDeviceCount</span></span>|<span data-ttu-id="7ec1a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec1a-145">Int32</span></span>|<span data-ttu-id="7ec1a-146">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-146">Number of unknown devices</span></span>|
|<span data-ttu-id="7ec1a-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec1a-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="7ec1a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec1a-148">Int32</span></span>|<span data-ttu-id="7ec1a-149">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="7ec1a-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec1a-150">compliantDeviceCount</span></span>|<span data-ttu-id="7ec1a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec1a-151">Int32</span></span>|<span data-ttu-id="7ec1a-152">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-152">Number of compliant devices</span></span>|
|<span data-ttu-id="7ec1a-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec1a-153">remediatedDeviceCount</span></span>|<span data-ttu-id="7ec1a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec1a-154">Int32</span></span>|<span data-ttu-id="7ec1a-155">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-155">Number of remediated devices</span></span>|
|<span data-ttu-id="7ec1a-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec1a-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7ec1a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec1a-157">Int32</span></span>|<span data-ttu-id="7ec1a-158">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="7ec1a-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec1a-159">errorDeviceCount</span></span>|<span data-ttu-id="7ec1a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec1a-160">Int32</span></span>|<span data-ttu-id="7ec1a-161">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-161">Number of error devices</span></span>|
|<span data-ttu-id="7ec1a-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7ec1a-162">conflictDeviceCount</span></span>|<span data-ttu-id="7ec1a-163">Int32</span><span class="sxs-lookup"><span data-stu-id="7ec1a-163">Int32</span></span>|<span data-ttu-id="7ec1a-164">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="7ec1a-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ec1a-165">Response</span></span>
<span data-ttu-id="7ec1a-166">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-166">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ec1a-167">Пример</span><span class="sxs-lookup"><span data-stu-id="7ec1a-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ec1a-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ec1a-168">Request</span></span>
<span data-ttu-id="7ec1a-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ec1a-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ec1a-170">Response</span></span>
<span data-ttu-id="7ec1a-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ec1a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




