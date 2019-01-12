---
title: Обновление advancedThreatProtectionOnboardingStateSummary
description: Обновление свойства объекта advancedThreatProtectionOnboardingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 423e1c9862d0e42e7d85efacd17cdd5f1733e0e9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929496"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="3b8ac-103">Обновление advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="3b8ac-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="3b8ac-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b8ac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b8ac-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b8ac-107">Обновление свойства объекта [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3b8ac-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b8ac-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3b8ac-108">Prerequisites</span></span>
<span data-ttu-id="3b8ac-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b8ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b8ac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b8ac-111">Permission type</span></span>|<span data-ttu-id="3b8ac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b8ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b8ac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b8ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b8ac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b8ac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b8ac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b8ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b8ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-116">Not supported.</span></span>|
|<span data-ttu-id="3b8ac-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b8ac-117">Application</span></span>|<span data-ttu-id="3b8ac-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b8ac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b8ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="3b8ac-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b8ac-120">Request headers</span></span>
|<span data-ttu-id="3b8ac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b8ac-121">Header</span></span>|<span data-ttu-id="3b8ac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3b8ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b8ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b8ac-123">Authorization</span></span>|<span data-ttu-id="3b8ac-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3b8ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b8ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b8ac-125">Accept</span></span>|<span data-ttu-id="3b8ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b8ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b8ac-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b8ac-127">Request body</span></span>
<span data-ttu-id="3b8ac-128">В тексте запроса укажите представление JSON для объекта [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="3b8ac-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="3b8ac-129">В следующей таблице показаны свойства, которые необходимы для создания [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3b8ac-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="3b8ac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b8ac-130">Property</span></span>|<span data-ttu-id="3b8ac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b8ac-131">Type</span></span>|<span data-ttu-id="3b8ac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b8ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b8ac-133">id</span><span class="sxs-lookup"><span data-stu-id="3b8ac-133">id</span></span>|<span data-ttu-id="3b8ac-134">String</span><span class="sxs-lookup"><span data-stu-id="3b8ac-134">String</span></span>|<span data-ttu-id="3b8ac-135">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-135">Unique Identifier</span></span>|
|<span data-ttu-id="3b8ac-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b8ac-136">unknownDeviceCount</span></span>|<span data-ttu-id="3b8ac-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3b8ac-137">Int32</span></span>|<span data-ttu-id="3b8ac-138">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-138">Number of unknown devices</span></span>|
|<span data-ttu-id="3b8ac-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b8ac-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="3b8ac-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3b8ac-140">Int32</span></span>|<span data-ttu-id="3b8ac-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="3b8ac-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b8ac-142">compliantDeviceCount</span></span>|<span data-ttu-id="3b8ac-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3b8ac-143">Int32</span></span>|<span data-ttu-id="3b8ac-144">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-144">Number of compliant devices</span></span>|
|<span data-ttu-id="3b8ac-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b8ac-145">remediatedDeviceCount</span></span>|<span data-ttu-id="3b8ac-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3b8ac-146">Int32</span></span>|<span data-ttu-id="3b8ac-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-147">Number of remediated devices</span></span>|
|<span data-ttu-id="3b8ac-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b8ac-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3b8ac-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3b8ac-149">Int32</span></span>|<span data-ttu-id="3b8ac-150">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="3b8ac-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b8ac-151">errorDeviceCount</span></span>|<span data-ttu-id="3b8ac-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3b8ac-152">Int32</span></span>|<span data-ttu-id="3b8ac-153">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-153">Number of error devices</span></span>|
|<span data-ttu-id="3b8ac-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b8ac-154">conflictDeviceCount</span></span>|<span data-ttu-id="3b8ac-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3b8ac-155">Int32</span></span>|<span data-ttu-id="3b8ac-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-156">Number of conflict devices</span></span>|
|<span data-ttu-id="3b8ac-157">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b8ac-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="3b8ac-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3b8ac-158">Int32</span></span>|<span data-ttu-id="3b8ac-159">Число не назначенный устройств</span><span class="sxs-lookup"><span data-stu-id="3b8ac-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="3b8ac-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b8ac-160">Response</span></span>
<span data-ttu-id="3b8ac-161">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b8ac-162">Пример</span><span class="sxs-lookup"><span data-stu-id="3b8ac-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b8ac-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b8ac-163">Request</span></span>
<span data-ttu-id="3b8ac-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 246

{
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

### <a name="response"></a><span data-ttu-id="3b8ac-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b8ac-165">Response</span></span>
<span data-ttu-id="3b8ac-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3b8ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





