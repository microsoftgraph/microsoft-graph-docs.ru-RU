---
title: Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: acdbe717ae96e179432ee49c9eb5fba2f5fde596
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934389"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="58f25-103">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="58f25-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="58f25-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="58f25-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58f25-105">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="58f25-105">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58f25-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="58f25-106">Prerequisites</span></span>
<span data-ttu-id="58f25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58f25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58f25-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58f25-109">Permission type</span></span>|<span data-ttu-id="58f25-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58f25-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58f25-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58f25-111">Delegated (work or school account)</span></span>|<span data-ttu-id="58f25-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58f25-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="58f25-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58f25-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58f25-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58f25-114">Not supported.</span></span>|
|<span data-ttu-id="58f25-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58f25-115">Application</span></span>|<span data-ttu-id="58f25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58f25-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58f25-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58f25-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="58f25-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58f25-118">Request headers</span></span>
|<span data-ttu-id="58f25-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58f25-119">Header</span></span>|<span data-ttu-id="58f25-120">Значение</span><span class="sxs-lookup"><span data-stu-id="58f25-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58f25-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58f25-121">Authorization</span></span>|<span data-ttu-id="58f25-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="58f25-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58f25-123">Accept</span><span class="sxs-lookup"><span data-stu-id="58f25-123">Accept</span></span>|<span data-ttu-id="58f25-124">application/json</span><span class="sxs-lookup"><span data-stu-id="58f25-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58f25-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58f25-125">Request body</span></span>
<span data-ttu-id="58f25-126">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58f25-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="58f25-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="58f25-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="58f25-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="58f25-128">Property</span></span>|<span data-ttu-id="58f25-129">Тип</span><span class="sxs-lookup"><span data-stu-id="58f25-129">Type</span></span>|<span data-ttu-id="58f25-130">Описание</span><span class="sxs-lookup"><span data-stu-id="58f25-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58f25-131">id</span><span class="sxs-lookup"><span data-stu-id="58f25-131">id</span></span>|<span data-ttu-id="58f25-132">Строка</span><span class="sxs-lookup"><span data-stu-id="58f25-132">String</span></span>|<span data-ttu-id="58f25-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="58f25-133">Key of the entity.</span></span>|
|<span data-ttu-id="58f25-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="58f25-134">pendingCount</span></span>|<span data-ttu-id="58f25-135">Int32</span><span class="sxs-lookup"><span data-stu-id="58f25-135">Int32</span></span>|<span data-ttu-id="58f25-136">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="58f25-136">Number of pending devices</span></span>|
|<span data-ttu-id="58f25-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="58f25-137">notApplicableCount</span></span>|<span data-ttu-id="58f25-138">Int32</span><span class="sxs-lookup"><span data-stu-id="58f25-138">Int32</span></span>|<span data-ttu-id="58f25-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="58f25-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="58f25-140">successCount</span><span class="sxs-lookup"><span data-stu-id="58f25-140">successCount</span></span>|<span data-ttu-id="58f25-141">Int32</span><span class="sxs-lookup"><span data-stu-id="58f25-141">Int32</span></span>|<span data-ttu-id="58f25-142">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="58f25-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="58f25-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="58f25-143">errorCount</span></span>|<span data-ttu-id="58f25-144">Int32</span><span class="sxs-lookup"><span data-stu-id="58f25-144">Int32</span></span>|<span data-ttu-id="58f25-145">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="58f25-145">Number of error devices</span></span>|
|<span data-ttu-id="58f25-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="58f25-146">failedCount</span></span>|<span data-ttu-id="58f25-147">Int32</span><span class="sxs-lookup"><span data-stu-id="58f25-147">Int32</span></span>|<span data-ttu-id="58f25-148">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="58f25-148">Number of failed devices</span></span>|
|<span data-ttu-id="58f25-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="58f25-149">lastUpdateDateTime</span></span>|<span data-ttu-id="58f25-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58f25-150">DateTimeOffset</span></span>|<span data-ttu-id="58f25-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="58f25-151">Last update time</span></span>|
|<span data-ttu-id="58f25-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="58f25-152">configurationVersion</span></span>|<span data-ttu-id="58f25-153">Int32</span><span class="sxs-lookup"><span data-stu-id="58f25-153">Int32</span></span>|<span data-ttu-id="58f25-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="58f25-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="58f25-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="58f25-155">Response</span></span>
<span data-ttu-id="58f25-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58f25-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58f25-157">Пример</span><span class="sxs-lookup"><span data-stu-id="58f25-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="58f25-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="58f25-158">Request</span></span>
<span data-ttu-id="58f25-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58f25-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58f25-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="58f25-160">Response</span></span>
<span data-ttu-id="58f25-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="58f25-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



