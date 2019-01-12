---
title: Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 971557babcc93a440361ef511a32b912953baceb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970502"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="b3d2a-103">Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="b3d2a-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="b3d2a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3d2a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3d2a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3d2a-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b3d2a-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3d2a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b3d2a-108">Prerequisites</span></span>
<span data-ttu-id="b3d2a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3d2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3d2a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3d2a-111">Permission type</span></span>|<span data-ttu-id="b3d2a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3d2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3d2a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3d2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3d2a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3d2a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3d2a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3d2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3d2a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-116">Not supported.</span></span>|
|<span data-ttu-id="b3d2a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3d2a-117">Application</span></span>|<span data-ttu-id="b3d2a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3d2a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3d2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="b3d2a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3d2a-120">Request headers</span></span>
|<span data-ttu-id="b3d2a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3d2a-121">Header</span></span>|<span data-ttu-id="b3d2a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b3d2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3d2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3d2a-123">Authorization</span></span>|<span data-ttu-id="b3d2a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b3d2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3d2a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3d2a-125">Accept</span></span>|<span data-ttu-id="b3d2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3d2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3d2a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3d2a-127">Request body</span></span>
<span data-ttu-id="b3d2a-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="b3d2a-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b3d2a-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="b3d2a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3d2a-130">Property</span></span>|<span data-ttu-id="b3d2a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b3d2a-131">Type</span></span>|<span data-ttu-id="b3d2a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b3d2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3d2a-133">id</span><span class="sxs-lookup"><span data-stu-id="b3d2a-133">id</span></span>|<span data-ttu-id="b3d2a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b3d2a-134">String</span></span>|<span data-ttu-id="b3d2a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-135">Key of the entity.</span></span>|
|<span data-ttu-id="b3d2a-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="b3d2a-136">pendingCount</span></span>|<span data-ttu-id="b3d2a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b3d2a-137">Int32</span></span>|<span data-ttu-id="b3d2a-138">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-138">Number of pending devices</span></span>|
|<span data-ttu-id="b3d2a-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b3d2a-139">notApplicableCount</span></span>|<span data-ttu-id="b3d2a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b3d2a-140">Int32</span></span>|<span data-ttu-id="b3d2a-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="b3d2a-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="b3d2a-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="b3d2a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b3d2a-143">Int32</span></span>|<span data-ttu-id="b3d2a-144">Число неприменимо устройств из-за несоответствие платформы и политики</span><span class="sxs-lookup"><span data-stu-id="b3d2a-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="b3d2a-145">successCount</span><span class="sxs-lookup"><span data-stu-id="b3d2a-145">successCount</span></span>|<span data-ttu-id="b3d2a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b3d2a-146">Int32</span></span>|<span data-ttu-id="b3d2a-147">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="b3d2a-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="b3d2a-148">errorCount</span></span>|<span data-ttu-id="b3d2a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b3d2a-149">Int32</span></span>|<span data-ttu-id="b3d2a-150">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-150">Number of error devices</span></span>|
|<span data-ttu-id="b3d2a-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="b3d2a-151">failedCount</span></span>|<span data-ttu-id="b3d2a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b3d2a-152">Int32</span></span>|<span data-ttu-id="b3d2a-153">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-153">Number of failed devices</span></span>|
|<span data-ttu-id="b3d2a-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="b3d2a-154">conflictCount</span></span>|<span data-ttu-id="b3d2a-155">Int32</span><span class="sxs-lookup"><span data-stu-id="b3d2a-155">Int32</span></span>|<span data-ttu-id="b3d2a-156">Количество устройств в конфликта</span><span class="sxs-lookup"><span data-stu-id="b3d2a-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="b3d2a-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b3d2a-157">lastUpdateDateTime</span></span>|<span data-ttu-id="b3d2a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3d2a-158">DateTimeOffset</span></span>|<span data-ttu-id="b3d2a-159">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-159">Last update time</span></span>|
|<span data-ttu-id="b3d2a-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="b3d2a-160">configurationVersion</span></span>|<span data-ttu-id="b3d2a-161">Int32</span><span class="sxs-lookup"><span data-stu-id="b3d2a-161">Int32</span></span>|<span data-ttu-id="b3d2a-162">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="b3d2a-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3d2a-163">Response</span></span>
<span data-ttu-id="b3d2a-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-164">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3d2a-165">Пример</span><span class="sxs-lookup"><span data-stu-id="b3d2a-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3d2a-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3d2a-166">Request</span></span>
<span data-ttu-id="b3d2a-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
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

### <a name="response"></a><span data-ttu-id="b3d2a-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3d2a-168">Response</span></span>
<span data-ttu-id="b3d2a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b3d2a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





