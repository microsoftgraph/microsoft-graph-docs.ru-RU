---
title: Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5672fa78f041967064425520a1df5cb52c6ff15c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412669"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="815b2-103">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="815b2-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="815b2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="815b2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="815b2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="815b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="815b2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="815b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="815b2-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="815b2-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="815b2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="815b2-108">Prerequisites</span></span>
<span data-ttu-id="815b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="815b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="815b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="815b2-111">Permission type</span></span>|<span data-ttu-id="815b2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="815b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="815b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="815b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="815b2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="815b2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="815b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="815b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="815b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="815b2-116">Not supported.</span></span>|
|<span data-ttu-id="815b2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="815b2-117">Application</span></span>|<span data-ttu-id="815b2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="815b2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="815b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="815b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="815b2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="815b2-120">Request headers</span></span>
|<span data-ttu-id="815b2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="815b2-121">Header</span></span>|<span data-ttu-id="815b2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="815b2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="815b2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="815b2-123">Authorization</span></span>|<span data-ttu-id="815b2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="815b2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="815b2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="815b2-125">Accept</span></span>|<span data-ttu-id="815b2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="815b2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="815b2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="815b2-127">Request body</span></span>
<span data-ttu-id="815b2-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="815b2-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="815b2-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="815b2-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="815b2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="815b2-130">Property</span></span>|<span data-ttu-id="815b2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="815b2-131">Type</span></span>|<span data-ttu-id="815b2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="815b2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="815b2-133">id</span><span class="sxs-lookup"><span data-stu-id="815b2-133">id</span></span>|<span data-ttu-id="815b2-134">String</span><span class="sxs-lookup"><span data-stu-id="815b2-134">String</span></span>|<span data-ttu-id="815b2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="815b2-135">Key of the entity.</span></span>|
|<span data-ttu-id="815b2-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="815b2-136">pendingCount</span></span>|<span data-ttu-id="815b2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="815b2-137">Int32</span></span>|<span data-ttu-id="815b2-138">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="815b2-138">Number of pending devices</span></span>|
|<span data-ttu-id="815b2-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="815b2-139">notApplicableCount</span></span>|<span data-ttu-id="815b2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="815b2-140">Int32</span></span>|<span data-ttu-id="815b2-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="815b2-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="815b2-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="815b2-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="815b2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="815b2-143">Int32</span></span>|<span data-ttu-id="815b2-144">Число неприменимо устройств из-за несоответствие платформы и политики</span><span class="sxs-lookup"><span data-stu-id="815b2-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="815b2-145">successCount</span><span class="sxs-lookup"><span data-stu-id="815b2-145">successCount</span></span>|<span data-ttu-id="815b2-146">Int32</span><span class="sxs-lookup"><span data-stu-id="815b2-146">Int32</span></span>|<span data-ttu-id="815b2-147">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="815b2-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="815b2-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="815b2-148">errorCount</span></span>|<span data-ttu-id="815b2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="815b2-149">Int32</span></span>|<span data-ttu-id="815b2-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="815b2-150">Number of error devices</span></span>|
|<span data-ttu-id="815b2-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="815b2-151">failedCount</span></span>|<span data-ttu-id="815b2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="815b2-152">Int32</span></span>|<span data-ttu-id="815b2-153">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="815b2-153">Number of failed devices</span></span>|
|<span data-ttu-id="815b2-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="815b2-154">conflictCount</span></span>|<span data-ttu-id="815b2-155">Int32</span><span class="sxs-lookup"><span data-stu-id="815b2-155">Int32</span></span>|<span data-ttu-id="815b2-156">Количество устройств в конфликта</span><span class="sxs-lookup"><span data-stu-id="815b2-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="815b2-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="815b2-157">lastUpdateDateTime</span></span>|<span data-ttu-id="815b2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="815b2-158">DateTimeOffset</span></span>|<span data-ttu-id="815b2-159">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="815b2-159">Last update time</span></span>|
|<span data-ttu-id="815b2-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="815b2-160">configurationVersion</span></span>|<span data-ttu-id="815b2-161">Int32</span><span class="sxs-lookup"><span data-stu-id="815b2-161">Int32</span></span>|<span data-ttu-id="815b2-162">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="815b2-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="815b2-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="815b2-163">Response</span></span>
<span data-ttu-id="815b2-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="815b2-164">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="815b2-165">Пример</span><span class="sxs-lookup"><span data-stu-id="815b2-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="815b2-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="815b2-166">Request</span></span>
<span data-ttu-id="815b2-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="815b2-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
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

### <a name="response"></a><span data-ttu-id="815b2-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="815b2-168">Response</span></span>
<span data-ttu-id="815b2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="815b2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
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




