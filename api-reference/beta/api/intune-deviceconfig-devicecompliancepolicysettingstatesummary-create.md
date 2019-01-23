---
title: Create deviceCompliancePolicySettingStateSummary
description: Создание объекта deviceCompliancePolicySettingStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 48bbae6e0252e7c0199d84802c71228ccbfebc04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414188"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="bd0f3-103">Create deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="bd0f3-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="bd0f3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd0f3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd0f3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd0f3-107">Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bd0f3-107">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd0f3-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bd0f3-108">Prerequisites</span></span>
<span data-ttu-id="bd0f3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd0f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bd0f3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd0f3-111">Permission type</span></span>|<span data-ttu-id="bd0f3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd0f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd0f3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd0f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd0f3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd0f3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd0f3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd0f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd0f3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-116">Not supported.</span></span>|
|<span data-ttu-id="bd0f3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd0f3-117">Application</span></span>|<span data-ttu-id="bd0f3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd0f3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd0f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="bd0f3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd0f3-120">Request headers</span></span>
|<span data-ttu-id="bd0f3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd0f3-121">Header</span></span>|<span data-ttu-id="bd0f3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bd0f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd0f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd0f3-123">Authorization</span></span>|<span data-ttu-id="bd0f3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bd0f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd0f3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bd0f3-125">Accept</span></span>|<span data-ttu-id="bd0f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd0f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd0f3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bd0f3-127">Request body</span></span>
<span data-ttu-id="bd0f3-128">В теле запроса добавьте представление объекта deviceCompliancePolicySettingStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-128">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="bd0f3-129">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-129">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="bd0f3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd0f3-130">Property</span></span>|<span data-ttu-id="bd0f3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bd0f3-131">Type</span></span>|<span data-ttu-id="bd0f3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bd0f3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd0f3-133">id</span><span class="sxs-lookup"><span data-stu-id="bd0f3-133">id</span></span>|<span data-ttu-id="bd0f3-134">String</span><span class="sxs-lookup"><span data-stu-id="bd0f3-134">String</span></span>|<span data-ttu-id="bd0f3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-135">Key of the entity.</span></span>|
|<span data-ttu-id="bd0f3-136">setting</span><span class="sxs-lookup"><span data-stu-id="bd0f3-136">setting</span></span>|<span data-ttu-id="bd0f3-137">String</span><span class="sxs-lookup"><span data-stu-id="bd0f3-137">String</span></span>|<span data-ttu-id="bd0f3-138">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="bd0f3-139">settingName</span><span class="sxs-lookup"><span data-stu-id="bd0f3-139">settingName</span></span>|<span data-ttu-id="bd0f3-140">String</span><span class="sxs-lookup"><span data-stu-id="bd0f3-140">String</span></span>|<span data-ttu-id="bd0f3-141">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-141">Name of the setting.</span></span>|
|<span data-ttu-id="bd0f3-142">platformType</span><span class="sxs-lookup"><span data-stu-id="bd0f3-142">platformType</span></span>|[<span data-ttu-id="bd0f3-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="bd0f3-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="bd0f3-144">Параметр платформы.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-144">Setting platform.</span></span> <span data-ttu-id="bd0f3-145">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="bd0f3-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd0f3-146">unknownDeviceCount</span></span>|<span data-ttu-id="bd0f3-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bd0f3-147">Int32</span></span>|<span data-ttu-id="bd0f3-148">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-148">Number of unknown devices</span></span>|
|<span data-ttu-id="bd0f3-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd0f3-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="bd0f3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="bd0f3-150">Int32</span></span>|<span data-ttu-id="bd0f3-151">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="bd0f3-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd0f3-152">compliantDeviceCount</span></span>|<span data-ttu-id="bd0f3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="bd0f3-153">Int32</span></span>|<span data-ttu-id="bd0f3-154">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-154">Number of compliant devices</span></span>|
|<span data-ttu-id="bd0f3-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd0f3-155">remediatedDeviceCount</span></span>|<span data-ttu-id="bd0f3-156">Int32</span><span class="sxs-lookup"><span data-stu-id="bd0f3-156">Int32</span></span>|<span data-ttu-id="bd0f3-157">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-157">Number of remediated devices</span></span>|
|<span data-ttu-id="bd0f3-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd0f3-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="bd0f3-159">Int32</span><span class="sxs-lookup"><span data-stu-id="bd0f3-159">Int32</span></span>|<span data-ttu-id="bd0f3-160">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="bd0f3-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd0f3-161">errorDeviceCount</span></span>|<span data-ttu-id="bd0f3-162">Int32</span><span class="sxs-lookup"><span data-stu-id="bd0f3-162">Int32</span></span>|<span data-ttu-id="bd0f3-163">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-163">Number of error devices</span></span>|
|<span data-ttu-id="bd0f3-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bd0f3-164">conflictDeviceCount</span></span>|<span data-ttu-id="bd0f3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bd0f3-165">Int32</span></span>|<span data-ttu-id="bd0f3-166">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="bd0f3-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd0f3-167">Response</span></span>
<span data-ttu-id="bd0f3-168">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-168">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd0f3-169">Пример</span><span class="sxs-lookup"><span data-stu-id="bd0f3-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd0f3-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd0f3-170">Request</span></span>
<span data-ttu-id="bd0f3-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bd0f3-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd0f3-172">Response</span></span>
<span data-ttu-id="bd0f3-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bd0f3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




