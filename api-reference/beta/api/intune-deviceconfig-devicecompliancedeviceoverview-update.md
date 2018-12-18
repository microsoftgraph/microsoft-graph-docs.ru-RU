---
title: Обновление объекта deviceComplianceDeviceOverview
description: Обновление свойств объекта deviceComplianceDeviceOverview.
author: tfitzmac
ms.openlocfilehash: 57237ed27f766c6cf8eab797cfa56735fde64aea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333217"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="34495-103">Обновление объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="34495-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="34495-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34495-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34495-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34495-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34495-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="34495-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34495-107">Обновление свойств объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="34495-107">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34495-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="34495-108">Prerequisites</span></span>
<span data-ttu-id="34495-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34495-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34495-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34495-111">Permission type</span></span>|<span data-ttu-id="34495-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34495-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34495-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34495-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34495-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34495-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34495-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34495-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34495-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34495-116">Not supported.</span></span>|
|<span data-ttu-id="34495-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34495-117">Application</span></span>|<span data-ttu-id="34495-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34495-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34495-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34495-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="34495-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34495-120">Request headers</span></span>
|<span data-ttu-id="34495-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34495-121">Header</span></span>|<span data-ttu-id="34495-122">Значение</span><span class="sxs-lookup"><span data-stu-id="34495-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34495-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34495-123">Authorization</span></span>|<span data-ttu-id="34495-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="34495-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34495-125">Accept</span><span class="sxs-lookup"><span data-stu-id="34495-125">Accept</span></span>|<span data-ttu-id="34495-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34495-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34495-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34495-127">Request body</span></span>
<span data-ttu-id="34495-128">В тексте запроса добавьте представление объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34495-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="34495-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="34495-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="34495-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="34495-130">Property</span></span>|<span data-ttu-id="34495-131">Тип</span><span class="sxs-lookup"><span data-stu-id="34495-131">Type</span></span>|<span data-ttu-id="34495-132">Описание</span><span class="sxs-lookup"><span data-stu-id="34495-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34495-133">id</span><span class="sxs-lookup"><span data-stu-id="34495-133">id</span></span>|<span data-ttu-id="34495-134">Строка</span><span class="sxs-lookup"><span data-stu-id="34495-134">String</span></span>|<span data-ttu-id="34495-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="34495-135">Key of the entity.</span></span>|
|<span data-ttu-id="34495-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="34495-136">pendingCount</span></span>|<span data-ttu-id="34495-137">Int32</span><span class="sxs-lookup"><span data-stu-id="34495-137">Int32</span></span>|<span data-ttu-id="34495-138">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="34495-138">Number of pending devices</span></span>|
|<span data-ttu-id="34495-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="34495-139">notApplicableCount</span></span>|<span data-ttu-id="34495-140">Int32</span><span class="sxs-lookup"><span data-stu-id="34495-140">Int32</span></span>|<span data-ttu-id="34495-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="34495-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="34495-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="34495-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="34495-143">Int32</span><span class="sxs-lookup"><span data-stu-id="34495-143">Int32</span></span>|<span data-ttu-id="34495-144">Число неприменимо устройств из-за несоответствие платформы и политики</span><span class="sxs-lookup"><span data-stu-id="34495-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="34495-145">successCount</span><span class="sxs-lookup"><span data-stu-id="34495-145">successCount</span></span>|<span data-ttu-id="34495-146">Int32</span><span class="sxs-lookup"><span data-stu-id="34495-146">Int32</span></span>|<span data-ttu-id="34495-147">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="34495-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="34495-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="34495-148">errorCount</span></span>|<span data-ttu-id="34495-149">Int32</span><span class="sxs-lookup"><span data-stu-id="34495-149">Int32</span></span>|<span data-ttu-id="34495-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="34495-150">Number of error devices</span></span>|
|<span data-ttu-id="34495-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="34495-151">failedCount</span></span>|<span data-ttu-id="34495-152">Int32</span><span class="sxs-lookup"><span data-stu-id="34495-152">Int32</span></span>|<span data-ttu-id="34495-153">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="34495-153">Number of failed devices</span></span>|
|<span data-ttu-id="34495-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="34495-154">conflictCount</span></span>|<span data-ttu-id="34495-155">Int32</span><span class="sxs-lookup"><span data-stu-id="34495-155">Int32</span></span>|<span data-ttu-id="34495-156">Количество устройств в конфликта</span><span class="sxs-lookup"><span data-stu-id="34495-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="34495-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="34495-157">lastUpdateDateTime</span></span>|<span data-ttu-id="34495-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34495-158">DateTimeOffset</span></span>|<span data-ttu-id="34495-159">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="34495-159">Last update time</span></span>|
|<span data-ttu-id="34495-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="34495-160">configurationVersion</span></span>|<span data-ttu-id="34495-161">Int32</span><span class="sxs-lookup"><span data-stu-id="34495-161">Int32</span></span>|<span data-ttu-id="34495-162">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="34495-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="34495-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="34495-163">Response</span></span>
<span data-ttu-id="34495-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34495-164">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34495-165">Пример</span><span class="sxs-lookup"><span data-stu-id="34495-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="34495-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="34495-166">Request</span></span>
<span data-ttu-id="34495-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34495-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 273

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="34495-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="34495-168">Response</span></span>
<span data-ttu-id="34495-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="34495-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





