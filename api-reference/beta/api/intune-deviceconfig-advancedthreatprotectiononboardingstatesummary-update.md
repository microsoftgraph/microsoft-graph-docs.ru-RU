---
title: Обновление advancedThreatProtectionOnboardingStateSummary
description: Обновление свойств объекта advancedThreatProtectionOnboardingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e980834c33c7fda9f9ad9f1552516d974c0087d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126838"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="f9405-103">Обновление advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f9405-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

<span data-ttu-id="f9405-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9405-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9405-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9405-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9405-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9405-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9405-107">Обновление свойств объекта [advancedThreatProtectionOnboardingStateSummary.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="f9405-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9405-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f9405-108">Prerequisites</span></span>
<span data-ttu-id="f9405-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9405-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9405-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9405-111">Permission type</span></span>|<span data-ttu-id="f9405-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9405-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9405-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9405-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9405-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9405-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9405-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9405-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9405-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9405-116">Not supported.</span></span>|
|<span data-ttu-id="f9405-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f9405-117">Application</span></span>|<span data-ttu-id="f9405-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9405-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9405-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9405-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="f9405-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f9405-120">Request headers</span></span>
|<span data-ttu-id="f9405-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9405-121">Header</span></span>|<span data-ttu-id="f9405-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f9405-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9405-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9405-123">Authorization</span></span>|<span data-ttu-id="f9405-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9405-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9405-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f9405-125">Accept</span></span>|<span data-ttu-id="f9405-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9405-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9405-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9405-127">Request body</span></span>
<span data-ttu-id="f9405-128">В теле запроса подарйте представление JSON для передового [объектаThreatProtectionOnboardingStateSummary.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="f9405-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="f9405-129">В следующей таблице показаны свойства, необходимые при создании [advancedThreatProtectionOnboardingStateSummary.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="f9405-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="f9405-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9405-130">Property</span></span>|<span data-ttu-id="f9405-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f9405-131">Type</span></span>|<span data-ttu-id="f9405-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f9405-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9405-133">id</span><span class="sxs-lookup"><span data-stu-id="f9405-133">id</span></span>|<span data-ttu-id="f9405-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f9405-134">String</span></span>|<span data-ttu-id="f9405-135">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="f9405-135">Unique Identifier</span></span>|
|<span data-ttu-id="f9405-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9405-136">unknownDeviceCount</span></span>|<span data-ttu-id="f9405-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f9405-137">Int32</span></span>|<span data-ttu-id="f9405-138">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="f9405-138">Number of unknown devices</span></span>|
|<span data-ttu-id="f9405-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9405-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="f9405-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f9405-140">Int32</span></span>|<span data-ttu-id="f9405-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="f9405-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="f9405-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9405-142">compliantDeviceCount</span></span>|<span data-ttu-id="f9405-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f9405-143">Int32</span></span>|<span data-ttu-id="f9405-144">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f9405-144">Number of compliant devices</span></span>|
|<span data-ttu-id="f9405-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9405-145">remediatedDeviceCount</span></span>|<span data-ttu-id="f9405-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f9405-146">Int32</span></span>|<span data-ttu-id="f9405-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="f9405-147">Number of remediated devices</span></span>|
|<span data-ttu-id="f9405-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9405-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f9405-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f9405-149">Int32</span></span>|<span data-ttu-id="f9405-150">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f9405-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f9405-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9405-151">errorDeviceCount</span></span>|<span data-ttu-id="f9405-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f9405-152">Int32</span></span>|<span data-ttu-id="f9405-153">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="f9405-153">Number of error devices</span></span>|
|<span data-ttu-id="f9405-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9405-154">conflictDeviceCount</span></span>|<span data-ttu-id="f9405-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f9405-155">Int32</span></span>|<span data-ttu-id="f9405-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="f9405-156">Number of conflict devices</span></span>|
|<span data-ttu-id="f9405-157">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9405-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="f9405-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f9405-158">Int32</span></span>|<span data-ttu-id="f9405-159">Количество не назначенных устройств</span><span class="sxs-lookup"><span data-stu-id="f9405-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="f9405-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9405-160">Response</span></span>
<span data-ttu-id="f9405-161">В случае успеха этот метод возвращает код ответа и обновленный расширенный `200 OK` [объектThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f9405-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9405-162">Пример</span><span class="sxs-lookup"><span data-stu-id="f9405-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9405-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9405-163">Request</span></span>
<span data-ttu-id="f9405-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9405-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```

### <a name="response"></a><span data-ttu-id="f9405-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9405-165">Response</span></span>
<span data-ttu-id="f9405-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9405-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "74089602-9602-7408-0296-087402960874",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```




