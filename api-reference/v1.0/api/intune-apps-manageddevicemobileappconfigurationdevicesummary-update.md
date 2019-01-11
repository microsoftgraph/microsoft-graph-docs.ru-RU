---
title: Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ad4845445e59105c1f304e8e90d67d97f153ed5e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818244"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="f0f4f-103">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f0f4f-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="f0f4f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0f4f-105">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f0f4f-105">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0f4f-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0f4f-106">Prerequisites</span></span>
<span data-ttu-id="f0f4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0f4f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0f4f-109">Permission type</span></span>|<span data-ttu-id="f0f4f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0f4f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0f4f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0f4f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0f4f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f4f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f0f4f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0f4f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0f4f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-114">Not supported.</span></span>|
|<span data-ttu-id="f0f4f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0f4f-115">Application</span></span>|<span data-ttu-id="f0f4f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0f4f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0f4f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="f0f4f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0f4f-118">Request headers</span></span>
|<span data-ttu-id="f0f4f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0f4f-119">Header</span></span>|<span data-ttu-id="f0f4f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f0f4f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0f4f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0f4f-121">Authorization</span></span>|<span data-ttu-id="f0f4f-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f0f4f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0f4f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f0f4f-123">Accept</span></span>|<span data-ttu-id="f0f4f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f0f4f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0f4f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0f4f-125">Request body</span></span>
<span data-ttu-id="f0f4f-126">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="f0f4f-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f0f4f-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="f0f4f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0f4f-128">Property</span></span>|<span data-ttu-id="f0f4f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f0f4f-129">Type</span></span>|<span data-ttu-id="f0f4f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f0f4f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0f4f-131">id</span><span class="sxs-lookup"><span data-stu-id="f0f4f-131">id</span></span>|<span data-ttu-id="f0f4f-132">Строка</span><span class="sxs-lookup"><span data-stu-id="f0f4f-132">String</span></span>|<span data-ttu-id="f0f4f-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-133">Key of the entity.</span></span>|
|<span data-ttu-id="f0f4f-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f0f4f-134">pendingCount</span></span>|<span data-ttu-id="f0f4f-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f4f-135">Int32</span></span>|<span data-ttu-id="f0f4f-136">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-136">Number of pending devices</span></span>|
|<span data-ttu-id="f0f4f-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f0f4f-137">notApplicableCount</span></span>|<span data-ttu-id="f0f4f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f4f-138">Int32</span></span>|<span data-ttu-id="f0f4f-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="f0f4f-140">successCount</span><span class="sxs-lookup"><span data-stu-id="f0f4f-140">successCount</span></span>|<span data-ttu-id="f0f4f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f4f-141">Int32</span></span>|<span data-ttu-id="f0f4f-142">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="f0f4f-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="f0f4f-143">errorCount</span></span>|<span data-ttu-id="f0f4f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f4f-144">Int32</span></span>|<span data-ttu-id="f0f4f-145">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-145">Number of error devices</span></span>|
|<span data-ttu-id="f0f4f-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="f0f4f-146">failedCount</span></span>|<span data-ttu-id="f0f4f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f4f-147">Int32</span></span>|<span data-ttu-id="f0f4f-148">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-148">Number of failed devices</span></span>|
|<span data-ttu-id="f0f4f-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f0f4f-149">lastUpdateDateTime</span></span>|<span data-ttu-id="f0f4f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0f4f-150">DateTimeOffset</span></span>|<span data-ttu-id="f0f4f-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-151">Last update time</span></span>|
|<span data-ttu-id="f0f4f-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f0f4f-152">configurationVersion</span></span>|<span data-ttu-id="f0f4f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f4f-153">Int32</span></span>|<span data-ttu-id="f0f4f-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="f0f4f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0f4f-155">Response</span></span>
<span data-ttu-id="f0f4f-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0f4f-157">Пример</span><span class="sxs-lookup"><span data-stu-id="f0f4f-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0f4f-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0f4f-158">Request</span></span>
<span data-ttu-id="f0f4f-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 299

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="f0f4f-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0f4f-160">Response</span></span>
<span data-ttu-id="f0f4f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f0f4f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



