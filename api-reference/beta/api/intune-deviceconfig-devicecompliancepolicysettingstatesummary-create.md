---
title: Create deviceCompliancePolicySettingStateSummary
description: Создание объекта deviceCompliancePolicySettingStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35ad4dc3762356f89732fb59fb00cfb9dd39c3ae
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949653"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="aceea-103">Create deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="aceea-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="aceea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aceea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aceea-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aceea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aceea-106">Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="aceea-106">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aceea-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="aceea-107">Prerequisites</span></span>
<span data-ttu-id="aceea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aceea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aceea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aceea-110">Permission type</span></span>|<span data-ttu-id="aceea-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aceea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aceea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aceea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aceea-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aceea-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aceea-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aceea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aceea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aceea-115">Not supported.</span></span>|
|<span data-ttu-id="aceea-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aceea-116">Application</span></span>|<span data-ttu-id="aceea-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aceea-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aceea-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aceea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="aceea-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aceea-119">Request headers</span></span>
|<span data-ttu-id="aceea-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aceea-120">Header</span></span>|<span data-ttu-id="aceea-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aceea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aceea-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aceea-122">Authorization</span></span>|<span data-ttu-id="aceea-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aceea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aceea-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aceea-124">Accept</span></span>|<span data-ttu-id="aceea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aceea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aceea-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aceea-126">Request body</span></span>
<span data-ttu-id="aceea-127">В теле запроса добавьте представление объекта deviceCompliancePolicySettingStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aceea-127">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="aceea-128">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="aceea-128">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="aceea-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="aceea-129">Property</span></span>|<span data-ttu-id="aceea-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aceea-130">Type</span></span>|<span data-ttu-id="aceea-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aceea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aceea-132">id</span><span class="sxs-lookup"><span data-stu-id="aceea-132">id</span></span>|<span data-ttu-id="aceea-133">Строка</span><span class="sxs-lookup"><span data-stu-id="aceea-133">String</span></span>|<span data-ttu-id="aceea-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aceea-134">Key of the entity.</span></span>|
|<span data-ttu-id="aceea-135">setting</span><span class="sxs-lookup"><span data-stu-id="aceea-135">setting</span></span>|<span data-ttu-id="aceea-136">Строка</span><span class="sxs-lookup"><span data-stu-id="aceea-136">String</span></span>|<span data-ttu-id="aceea-137">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="aceea-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="aceea-138">settingName</span><span class="sxs-lookup"><span data-stu-id="aceea-138">settingName</span></span>|<span data-ttu-id="aceea-139">String</span><span class="sxs-lookup"><span data-stu-id="aceea-139">String</span></span>|<span data-ttu-id="aceea-140">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="aceea-140">Name of the setting.</span></span>|
|<span data-ttu-id="aceea-141">platformType</span><span class="sxs-lookup"><span data-stu-id="aceea-141">platformType</span></span>|[<span data-ttu-id="aceea-142">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="aceea-142">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="aceea-143">Настройка платформы.</span><span class="sxs-lookup"><span data-stu-id="aceea-143">Setting platform.</span></span> <span data-ttu-id="aceea-144">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="aceea-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="aceea-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aceea-145">unknownDeviceCount</span></span>|<span data-ttu-id="aceea-146">Int32</span><span class="sxs-lookup"><span data-stu-id="aceea-146">Int32</span></span>|<span data-ttu-id="aceea-147">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="aceea-147">Number of unknown devices</span></span>|
|<span data-ttu-id="aceea-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aceea-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="aceea-149">Int32</span><span class="sxs-lookup"><span data-stu-id="aceea-149">Int32</span></span>|<span data-ttu-id="aceea-150">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="aceea-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="aceea-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aceea-151">compliantDeviceCount</span></span>|<span data-ttu-id="aceea-152">Int32</span><span class="sxs-lookup"><span data-stu-id="aceea-152">Int32</span></span>|<span data-ttu-id="aceea-153">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="aceea-153">Number of compliant devices</span></span>|
|<span data-ttu-id="aceea-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aceea-154">remediatedDeviceCount</span></span>|<span data-ttu-id="aceea-155">Int32</span><span class="sxs-lookup"><span data-stu-id="aceea-155">Int32</span></span>|<span data-ttu-id="aceea-156">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="aceea-156">Number of remediated devices</span></span>|
|<span data-ttu-id="aceea-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aceea-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="aceea-158">Int32</span><span class="sxs-lookup"><span data-stu-id="aceea-158">Int32</span></span>|<span data-ttu-id="aceea-159">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="aceea-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="aceea-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aceea-160">errorDeviceCount</span></span>|<span data-ttu-id="aceea-161">Int32</span><span class="sxs-lookup"><span data-stu-id="aceea-161">Int32</span></span>|<span data-ttu-id="aceea-162">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="aceea-162">Number of error devices</span></span>|
|<span data-ttu-id="aceea-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aceea-163">conflictDeviceCount</span></span>|<span data-ttu-id="aceea-164">Int32</span><span class="sxs-lookup"><span data-stu-id="aceea-164">Int32</span></span>|<span data-ttu-id="aceea-165">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="aceea-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="aceea-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="aceea-166">Response</span></span>
<span data-ttu-id="aceea-167">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="aceea-167">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aceea-168">Пример</span><span class="sxs-lookup"><span data-stu-id="aceea-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="aceea-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="aceea-169">Request</span></span>
<span data-ttu-id="aceea-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aceea-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="aceea-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="aceea-171">Response</span></span>
<span data-ttu-id="aceea-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aceea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





