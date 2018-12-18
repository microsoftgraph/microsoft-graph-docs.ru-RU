---
title: Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
ms.openlocfilehash: 35a75cba4d67c23f5c011bfe7e75e23452d4c954
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330186"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="1b0c2-103">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1b0c2-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="1b0c2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b0c2-105">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1b0c2-105">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b0c2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1b0c2-106">Prerequisites</span></span>
<span data-ttu-id="1b0c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b0c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b0c2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b0c2-109">Permission type</span></span>|<span data-ttu-id="1b0c2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b0c2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b0c2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b0c2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b0c2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b0c2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b0c2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b0c2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b0c2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-114">Not supported.</span></span>|
|<span data-ttu-id="1b0c2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b0c2-115">Application</span></span>|<span data-ttu-id="1b0c2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b0c2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b0c2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="1b0c2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b0c2-118">Request headers</span></span>
|<span data-ttu-id="1b0c2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b0c2-119">Header</span></span>|<span data-ttu-id="1b0c2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1b0c2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b0c2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b0c2-121">Authorization</span></span>|<span data-ttu-id="1b0c2-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1b0c2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b0c2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1b0c2-123">Accept</span></span>|<span data-ttu-id="1b0c2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1b0c2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b0c2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b0c2-125">Request body</span></span>
<span data-ttu-id="1b0c2-126">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="1b0c2-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1b0c2-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="1b0c2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b0c2-128">Property</span></span>|<span data-ttu-id="1b0c2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1b0c2-129">Type</span></span>|<span data-ttu-id="1b0c2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1b0c2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b0c2-131">id</span><span class="sxs-lookup"><span data-stu-id="1b0c2-131">id</span></span>|<span data-ttu-id="1b0c2-132">Строка</span><span class="sxs-lookup"><span data-stu-id="1b0c2-132">String</span></span>|<span data-ttu-id="1b0c2-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-133">Key of the entity.</span></span>|
|<span data-ttu-id="1b0c2-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="1b0c2-134">pendingCount</span></span>|<span data-ttu-id="1b0c2-135">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0c2-135">Int32</span></span>|<span data-ttu-id="1b0c2-136">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-136">Number of pending devices</span></span>|
|<span data-ttu-id="1b0c2-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1b0c2-137">notApplicableCount</span></span>|<span data-ttu-id="1b0c2-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0c2-138">Int32</span></span>|<span data-ttu-id="1b0c2-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="1b0c2-140">successCount</span><span class="sxs-lookup"><span data-stu-id="1b0c2-140">successCount</span></span>|<span data-ttu-id="1b0c2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0c2-141">Int32</span></span>|<span data-ttu-id="1b0c2-142">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="1b0c2-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="1b0c2-143">errorCount</span></span>|<span data-ttu-id="1b0c2-144">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0c2-144">Int32</span></span>|<span data-ttu-id="1b0c2-145">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-145">Number of error devices</span></span>|
|<span data-ttu-id="1b0c2-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="1b0c2-146">failedCount</span></span>|<span data-ttu-id="1b0c2-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0c2-147">Int32</span></span>|<span data-ttu-id="1b0c2-148">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-148">Number of failed devices</span></span>|
|<span data-ttu-id="1b0c2-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0c2-149">lastUpdateDateTime</span></span>|<span data-ttu-id="1b0c2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0c2-150">DateTimeOffset</span></span>|<span data-ttu-id="1b0c2-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-151">Last update time</span></span>|
|<span data-ttu-id="1b0c2-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="1b0c2-152">configurationVersion</span></span>|<span data-ttu-id="1b0c2-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0c2-153">Int32</span></span>|<span data-ttu-id="1b0c2-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="1b0c2-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b0c2-155">Response</span></span>
<span data-ttu-id="1b0c2-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b0c2-157">Пример</span><span class="sxs-lookup"><span data-stu-id="1b0c2-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b0c2-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b0c2-158">Request</span></span>
<span data-ttu-id="1b0c2-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b0c2-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b0c2-160">Response</span></span>
<span data-ttu-id="1b0c2-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b0c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



