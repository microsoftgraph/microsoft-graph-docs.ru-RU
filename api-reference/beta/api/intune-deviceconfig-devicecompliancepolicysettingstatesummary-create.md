---
title: Create deviceCompliancePolicySettingStateSummary
description: Создание объекта deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f9f64cca9ca75ea8d823e7aa0adedad6d3527666
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832692"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="4144d-103">Create deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="4144d-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="4144d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4144d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4144d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4144d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4144d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4144d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4144d-107">Создание объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4144d-107">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4144d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4144d-108">Prerequisites</span></span>
<span data-ttu-id="4144d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4144d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4144d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4144d-111">Permission type</span></span>|<span data-ttu-id="4144d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4144d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4144d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4144d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4144d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4144d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4144d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4144d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4144d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4144d-116">Not supported.</span></span>|
|<span data-ttu-id="4144d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4144d-117">Application</span></span>|<span data-ttu-id="4144d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4144d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4144d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4144d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="4144d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4144d-120">Request headers</span></span>
|<span data-ttu-id="4144d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4144d-121">Header</span></span>|<span data-ttu-id="4144d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4144d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4144d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4144d-123">Authorization</span></span>|<span data-ttu-id="4144d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4144d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4144d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4144d-125">Accept</span></span>|<span data-ttu-id="4144d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4144d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4144d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4144d-127">Request body</span></span>
<span data-ttu-id="4144d-128">В теле запроса добавьте представление объекта deviceCompliancePolicySettingStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4144d-128">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="4144d-129">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicySettingStateSummary.</span><span class="sxs-lookup"><span data-stu-id="4144d-129">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="4144d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4144d-130">Property</span></span>|<span data-ttu-id="4144d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4144d-131">Type</span></span>|<span data-ttu-id="4144d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4144d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4144d-133">id</span><span class="sxs-lookup"><span data-stu-id="4144d-133">id</span></span>|<span data-ttu-id="4144d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4144d-134">String</span></span>|<span data-ttu-id="4144d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4144d-135">Key of the entity.</span></span>|
|<span data-ttu-id="4144d-136">setting</span><span class="sxs-lookup"><span data-stu-id="4144d-136">setting</span></span>|<span data-ttu-id="4144d-137">String</span><span class="sxs-lookup"><span data-stu-id="4144d-137">String</span></span>|<span data-ttu-id="4144d-138">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="4144d-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="4144d-139">settingName</span><span class="sxs-lookup"><span data-stu-id="4144d-139">settingName</span></span>|<span data-ttu-id="4144d-140">String</span><span class="sxs-lookup"><span data-stu-id="4144d-140">String</span></span>|<span data-ttu-id="4144d-141">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="4144d-141">Name of the setting.</span></span>|
|<span data-ttu-id="4144d-142">platformType</span><span class="sxs-lookup"><span data-stu-id="4144d-142">platformType</span></span>|[<span data-ttu-id="4144d-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="4144d-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="4144d-144">Параметр платформы.</span><span class="sxs-lookup"><span data-stu-id="4144d-144">Setting platform.</span></span> <span data-ttu-id="4144d-145">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="4144d-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="4144d-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4144d-146">unknownDeviceCount</span></span>|<span data-ttu-id="4144d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4144d-147">Int32</span></span>|<span data-ttu-id="4144d-148">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="4144d-148">Number of unknown devices</span></span>|
|<span data-ttu-id="4144d-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4144d-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="4144d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4144d-150">Int32</span></span>|<span data-ttu-id="4144d-151">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="4144d-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="4144d-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4144d-152">compliantDeviceCount</span></span>|<span data-ttu-id="4144d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4144d-153">Int32</span></span>|<span data-ttu-id="4144d-154">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="4144d-154">Number of compliant devices</span></span>|
|<span data-ttu-id="4144d-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4144d-155">remediatedDeviceCount</span></span>|<span data-ttu-id="4144d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="4144d-156">Int32</span></span>|<span data-ttu-id="4144d-157">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="4144d-157">Number of remediated devices</span></span>|
|<span data-ttu-id="4144d-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4144d-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="4144d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="4144d-159">Int32</span></span>|<span data-ttu-id="4144d-160">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="4144d-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="4144d-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4144d-161">errorDeviceCount</span></span>|<span data-ttu-id="4144d-162">Int32</span><span class="sxs-lookup"><span data-stu-id="4144d-162">Int32</span></span>|<span data-ttu-id="4144d-163">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="4144d-163">Number of error devices</span></span>|
|<span data-ttu-id="4144d-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4144d-164">conflictDeviceCount</span></span>|<span data-ttu-id="4144d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4144d-165">Int32</span></span>|<span data-ttu-id="4144d-166">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="4144d-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="4144d-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="4144d-167">Response</span></span>
<span data-ttu-id="4144d-168">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4144d-168">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4144d-169">Пример</span><span class="sxs-lookup"><span data-stu-id="4144d-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="4144d-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="4144d-170">Request</span></span>
<span data-ttu-id="4144d-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4144d-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4144d-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="4144d-172">Response</span></span>
<span data-ttu-id="4144d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4144d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





