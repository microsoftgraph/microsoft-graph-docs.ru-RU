---
title: Обновление объекта deviceCompliancePolicySettingStateSummary
description: Обновление свойств объекта deviceCompliancePolicySettingStateSummary.
author: tfitzmac
ms.openlocfilehash: d85aa50045c3378a2a4da7826dcaa3fb968664ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345075"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="1cba5-103">Обновление объекта deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="1cba5-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="1cba5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1cba5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cba5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cba5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cba5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1cba5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cba5-107">Обновление свойств объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1cba5-107">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1cba5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1cba5-108">Prerequisites</span></span>
<span data-ttu-id="1cba5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cba5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cba5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cba5-111">Permission type</span></span>|<span data-ttu-id="1cba5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cba5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cba5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cba5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1cba5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cba5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1cba5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cba5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cba5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cba5-116">Not supported.</span></span>|
|<span data-ttu-id="1cba5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cba5-117">Application</span></span>|<span data-ttu-id="1cba5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cba5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cba5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cba5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="1cba5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cba5-120">Request headers</span></span>
|<span data-ttu-id="1cba5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cba5-121">Header</span></span>|<span data-ttu-id="1cba5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1cba5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cba5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1cba5-123">Authorization</span></span>|<span data-ttu-id="1cba5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1cba5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cba5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1cba5-125">Accept</span></span>|<span data-ttu-id="1cba5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1cba5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cba5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1cba5-127">Request body</span></span>
<span data-ttu-id="1cba5-128">В теле запроса добавьте представление объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cba5-128">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="1cba5-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1cba5-129">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="1cba5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cba5-130">Property</span></span>|<span data-ttu-id="1cba5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1cba5-131">Type</span></span>|<span data-ttu-id="1cba5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1cba5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cba5-133">id</span><span class="sxs-lookup"><span data-stu-id="1cba5-133">id</span></span>|<span data-ttu-id="1cba5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1cba5-134">String</span></span>|<span data-ttu-id="1cba5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1cba5-135">Key of the entity.</span></span>|
|<span data-ttu-id="1cba5-136">setting</span><span class="sxs-lookup"><span data-stu-id="1cba5-136">setting</span></span>|<span data-ttu-id="1cba5-137">String</span><span class="sxs-lookup"><span data-stu-id="1cba5-137">String</span></span>|<span data-ttu-id="1cba5-138">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="1cba5-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="1cba5-139">settingName</span><span class="sxs-lookup"><span data-stu-id="1cba5-139">settingName</span></span>|<span data-ttu-id="1cba5-140">String</span><span class="sxs-lookup"><span data-stu-id="1cba5-140">String</span></span>|<span data-ttu-id="1cba5-141">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="1cba5-141">Name of the setting.</span></span>|
|<span data-ttu-id="1cba5-142">platformType</span><span class="sxs-lookup"><span data-stu-id="1cba5-142">platformType</span></span>|[<span data-ttu-id="1cba5-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="1cba5-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="1cba5-144">Параметр платформы.</span><span class="sxs-lookup"><span data-stu-id="1cba5-144">Setting platform.</span></span> <span data-ttu-id="1cba5-145">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="1cba5-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="1cba5-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1cba5-146">unknownDeviceCount</span></span>|<span data-ttu-id="1cba5-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1cba5-147">Int32</span></span>|<span data-ttu-id="1cba5-148">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="1cba5-148">Number of unknown devices</span></span>|
|<span data-ttu-id="1cba5-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1cba5-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="1cba5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1cba5-150">Int32</span></span>|<span data-ttu-id="1cba5-151">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="1cba5-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="1cba5-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1cba5-152">compliantDeviceCount</span></span>|<span data-ttu-id="1cba5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1cba5-153">Int32</span></span>|<span data-ttu-id="1cba5-154">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="1cba5-154">Number of compliant devices</span></span>|
|<span data-ttu-id="1cba5-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1cba5-155">remediatedDeviceCount</span></span>|<span data-ttu-id="1cba5-156">Int32</span><span class="sxs-lookup"><span data-stu-id="1cba5-156">Int32</span></span>|<span data-ttu-id="1cba5-157">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="1cba5-157">Number of remediated devices</span></span>|
|<span data-ttu-id="1cba5-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1cba5-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="1cba5-159">Int32</span><span class="sxs-lookup"><span data-stu-id="1cba5-159">Int32</span></span>|<span data-ttu-id="1cba5-160">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="1cba5-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="1cba5-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1cba5-161">errorDeviceCount</span></span>|<span data-ttu-id="1cba5-162">Int32</span><span class="sxs-lookup"><span data-stu-id="1cba5-162">Int32</span></span>|<span data-ttu-id="1cba5-163">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="1cba5-163">Number of error devices</span></span>|
|<span data-ttu-id="1cba5-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1cba5-164">conflictDeviceCount</span></span>|<span data-ttu-id="1cba5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1cba5-165">Int32</span></span>|<span data-ttu-id="1cba5-166">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="1cba5-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="1cba5-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cba5-167">Response</span></span>
<span data-ttu-id="1cba5-168">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1cba5-168">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cba5-169">Пример</span><span class="sxs-lookup"><span data-stu-id="1cba5-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="1cba5-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cba5-170">Request</span></span>
<span data-ttu-id="1cba5-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cba5-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 322

{
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

### <a name="response"></a><span data-ttu-id="1cba5-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cba5-172">Response</span></span>
<span data-ttu-id="1cba5-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1cba5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





