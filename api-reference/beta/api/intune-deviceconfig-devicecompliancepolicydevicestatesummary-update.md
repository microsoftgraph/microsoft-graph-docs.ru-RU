---
title: Обновление объекта deviceCompliancePolicyDeviceStateSummary
description: Обновление свойств объекта deviceCompliancePolicyDeviceStateSummary.
ms.openlocfilehash: 045c9ac7aaecac535f3c4d04f587c74cbe84f442
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078469"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="e6a54-103">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e6a54-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="e6a54-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6a54-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6a54-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6a54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6a54-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e6a54-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6a54-107">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e6a54-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6a54-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e6a54-108">Prerequisites</span></span>
<span data-ttu-id="e6a54-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6a54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6a54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6a54-111">Permission type</span></span>|<span data-ttu-id="e6a54-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6a54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6a54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6a54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6a54-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6a54-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6a54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6a54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6a54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6a54-116">Not supported.</span></span>|
|<span data-ttu-id="e6a54-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6a54-117">Application</span></span>|<span data-ttu-id="e6a54-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6a54-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6a54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6a54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="e6a54-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6a54-120">Request headers</span></span>
|<span data-ttu-id="e6a54-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6a54-121">Header</span></span>|<span data-ttu-id="e6a54-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e6a54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6a54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6a54-123">Authorization</span></span>|<span data-ttu-id="e6a54-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e6a54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6a54-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e6a54-125">Accept</span></span>|<span data-ttu-id="e6a54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6a54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6a54-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6a54-127">Request body</span></span>
<span data-ttu-id="e6a54-128">В тексте запроса добавьте представление объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6a54-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="e6a54-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e6a54-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="e6a54-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6a54-130">Property</span></span>|<span data-ttu-id="e6a54-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e6a54-131">Type</span></span>|<span data-ttu-id="e6a54-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e6a54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6a54-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="e6a54-133">inGracePeriodCount</span></span>|<span data-ttu-id="e6a54-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a54-134">Int32</span></span>|<span data-ttu-id="e6a54-135">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="e6a54-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="e6a54-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="e6a54-136">configManagerCount</span></span>|<span data-ttu-id="e6a54-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a54-137">Int32</span></span>|<span data-ttu-id="e6a54-138">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="e6a54-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="e6a54-139">id</span><span class="sxs-lookup"><span data-stu-id="e6a54-139">id</span></span>|<span data-ttu-id="e6a54-140">String</span><span class="sxs-lookup"><span data-stu-id="e6a54-140">String</span></span>|<span data-ttu-id="e6a54-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e6a54-141">Key of the entity.</span></span>|
|<span data-ttu-id="e6a54-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a54-142">unknownDeviceCount</span></span>|<span data-ttu-id="e6a54-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a54-143">Int32</span></span>|<span data-ttu-id="e6a54-144">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="e6a54-144">Number of unknown devices</span></span>|
|<span data-ttu-id="e6a54-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a54-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="e6a54-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a54-146">Int32</span></span>|<span data-ttu-id="e6a54-147">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="e6a54-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="e6a54-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a54-148">compliantDeviceCount</span></span>|<span data-ttu-id="e6a54-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a54-149">Int32</span></span>|<span data-ttu-id="e6a54-150">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="e6a54-150">Number of compliant devices</span></span>|
|<span data-ttu-id="e6a54-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a54-151">remediatedDeviceCount</span></span>|<span data-ttu-id="e6a54-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a54-152">Int32</span></span>|<span data-ttu-id="e6a54-153">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="e6a54-153">Number of remediated devices</span></span>|
|<span data-ttu-id="e6a54-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a54-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e6a54-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a54-155">Int32</span></span>|<span data-ttu-id="e6a54-156">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="e6a54-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e6a54-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a54-157">errorDeviceCount</span></span>|<span data-ttu-id="e6a54-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a54-158">Int32</span></span>|<span data-ttu-id="e6a54-159">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e6a54-159">Number of error devices</span></span>|
|<span data-ttu-id="e6a54-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e6a54-160">conflictDeviceCount</span></span>|<span data-ttu-id="e6a54-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e6a54-161">Int32</span></span>|<span data-ttu-id="e6a54-162">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="e6a54-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="e6a54-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6a54-163">Response</span></span>
<span data-ttu-id="e6a54-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6a54-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6a54-165">Пример</span><span class="sxs-lookup"><span data-stu-id="e6a54-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6a54-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6a54-166">Request</span></span>
<span data-ttu-id="e6a54-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6a54-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 270

{
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="e6a54-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6a54-168">Response</span></span>
<span data-ttu-id="e6a54-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e6a54-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```





