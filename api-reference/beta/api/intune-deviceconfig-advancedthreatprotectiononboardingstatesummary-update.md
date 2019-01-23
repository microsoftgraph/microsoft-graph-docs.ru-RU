---
title: Обновление advancedThreatProtectionOnboardingStateSummary
description: Обновление свойства объекта advancedThreatProtectionOnboardingStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9a94e5b0abee3d369148c2301942a1196ef9010c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409281"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="ca93b-103">Обновление advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="ca93b-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="ca93b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca93b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca93b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca93b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca93b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca93b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca93b-107">Обновление свойства объекта [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ca93b-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca93b-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="ca93b-108">Prerequisites</span></span>
<span data-ttu-id="ca93b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca93b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ca93b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca93b-111">Permission type</span></span>|<span data-ttu-id="ca93b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca93b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca93b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca93b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca93b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca93b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca93b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca93b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca93b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca93b-116">Not supported.</span></span>|
|<span data-ttu-id="ca93b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca93b-117">Application</span></span>|<span data-ttu-id="ca93b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca93b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca93b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca93b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="ca93b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca93b-120">Request headers</span></span>
|<span data-ttu-id="ca93b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca93b-121">Header</span></span>|<span data-ttu-id="ca93b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ca93b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca93b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca93b-123">Authorization</span></span>|<span data-ttu-id="ca93b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ca93b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca93b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca93b-125">Accept</span></span>|<span data-ttu-id="ca93b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca93b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca93b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca93b-127">Request body</span></span>
<span data-ttu-id="ca93b-128">В тексте запроса укажите представление JSON для объекта [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ca93b-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="ca93b-129">В следующей таблице показаны свойства, которые необходимы для создания [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ca93b-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="ca93b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca93b-130">Property</span></span>|<span data-ttu-id="ca93b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ca93b-131">Type</span></span>|<span data-ttu-id="ca93b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ca93b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca93b-133">id</span><span class="sxs-lookup"><span data-stu-id="ca93b-133">id</span></span>|<span data-ttu-id="ca93b-134">String</span><span class="sxs-lookup"><span data-stu-id="ca93b-134">String</span></span>|<span data-ttu-id="ca93b-135">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="ca93b-135">Unique Identifier</span></span>|
|<span data-ttu-id="ca93b-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ca93b-136">unknownDeviceCount</span></span>|<span data-ttu-id="ca93b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ca93b-137">Int32</span></span>|<span data-ttu-id="ca93b-138">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="ca93b-138">Number of unknown devices</span></span>|
|<span data-ttu-id="ca93b-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ca93b-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="ca93b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ca93b-140">Int32</span></span>|<span data-ttu-id="ca93b-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="ca93b-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="ca93b-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ca93b-142">compliantDeviceCount</span></span>|<span data-ttu-id="ca93b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ca93b-143">Int32</span></span>|<span data-ttu-id="ca93b-144">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="ca93b-144">Number of compliant devices</span></span>|
|<span data-ttu-id="ca93b-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ca93b-145">remediatedDeviceCount</span></span>|<span data-ttu-id="ca93b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ca93b-146">Int32</span></span>|<span data-ttu-id="ca93b-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="ca93b-147">Number of remediated devices</span></span>|
|<span data-ttu-id="ca93b-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ca93b-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="ca93b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ca93b-149">Int32</span></span>|<span data-ttu-id="ca93b-150">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="ca93b-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="ca93b-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ca93b-151">errorDeviceCount</span></span>|<span data-ttu-id="ca93b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ca93b-152">Int32</span></span>|<span data-ttu-id="ca93b-153">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="ca93b-153">Number of error devices</span></span>|
|<span data-ttu-id="ca93b-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ca93b-154">conflictDeviceCount</span></span>|<span data-ttu-id="ca93b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="ca93b-155">Int32</span></span>|<span data-ttu-id="ca93b-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="ca93b-156">Number of conflict devices</span></span>|
|<span data-ttu-id="ca93b-157">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ca93b-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="ca93b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ca93b-158">Int32</span></span>|<span data-ttu-id="ca93b-159">Число не назначенный устройств</span><span class="sxs-lookup"><span data-stu-id="ca93b-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="ca93b-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca93b-160">Response</span></span>
<span data-ttu-id="ca93b-161">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ca93b-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca93b-162">Пример</span><span class="sxs-lookup"><span data-stu-id="ca93b-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca93b-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca93b-163">Request</span></span>
<span data-ttu-id="ca93b-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca93b-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca93b-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca93b-165">Response</span></span>
<span data-ttu-id="ca93b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ca93b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




