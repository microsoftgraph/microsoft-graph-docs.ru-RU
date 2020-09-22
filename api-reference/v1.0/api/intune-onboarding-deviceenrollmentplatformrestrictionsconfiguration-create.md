---
title: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9bbac90b39141d201792f78dcc9883bc1eb23d2b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033190"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="dc9ab-103">Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="dc9ab-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="dc9ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc9ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc9ab-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc9ab-106">Создание объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dc9ab-106">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc9ab-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dc9ab-107">Prerequisites</span></span>
<span data-ttu-id="dc9ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc9ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc9ab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc9ab-110">Permission type</span></span>|<span data-ttu-id="dc9ab-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc9ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc9ab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc9ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc9ab-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc9ab-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dc9ab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc9ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc9ab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-115">Not supported.</span></span>|
|<span data-ttu-id="dc9ab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc9ab-116">Application</span></span>|<span data-ttu-id="dc9ab-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc9ab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc9ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dc9ab-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dc9ab-119">Request headers</span></span>
|<span data-ttu-id="dc9ab-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc9ab-120">Header</span></span>|<span data-ttu-id="dc9ab-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dc9ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc9ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc9ab-122">Authorization</span></span>|<span data-ttu-id="dc9ab-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc9ab-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dc9ab-124">Accept</span></span>|<span data-ttu-id="dc9ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc9ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc9ab-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dc9ab-126">Request body</span></span>
<span data-ttu-id="dc9ab-127">В теле запроса добавьте представление объекта deviceEnrollmentPlatformRestrictionsConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-127">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="dc9ab-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-128">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="dc9ab-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc9ab-129">Property</span></span>|<span data-ttu-id="dc9ab-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dc9ab-130">Type</span></span>|<span data-ttu-id="dc9ab-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dc9ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc9ab-132">id</span><span class="sxs-lookup"><span data-stu-id="dc9ab-132">id</span></span>|<span data-ttu-id="dc9ab-133">String</span><span class="sxs-lookup"><span data-stu-id="dc9ab-133">String</span></span>|<span data-ttu-id="dc9ab-134">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc9ab-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dc9ab-135">displayName</span><span class="sxs-lookup"><span data-stu-id="dc9ab-135">displayName</span></span>|<span data-ttu-id="dc9ab-136">String</span><span class="sxs-lookup"><span data-stu-id="dc9ab-136">String</span></span>|<span data-ttu-id="dc9ab-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc9ab-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dc9ab-138">description</span><span class="sxs-lookup"><span data-stu-id="dc9ab-138">description</span></span>|<span data-ttu-id="dc9ab-139">String</span><span class="sxs-lookup"><span data-stu-id="dc9ab-139">String</span></span>|<span data-ttu-id="dc9ab-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc9ab-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dc9ab-141">priority</span><span class="sxs-lookup"><span data-stu-id="dc9ab-141">priority</span></span>|<span data-ttu-id="dc9ab-142">Int32</span><span class="sxs-lookup"><span data-stu-id="dc9ab-142">Int32</span></span>|<span data-ttu-id="dc9ab-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc9ab-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dc9ab-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc9ab-144">createdDateTime</span></span>|<span data-ttu-id="dc9ab-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc9ab-145">DateTimeOffset</span></span>|<span data-ttu-id="dc9ab-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc9ab-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dc9ab-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc9ab-147">lastModifiedDateTime</span></span>|<span data-ttu-id="dc9ab-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc9ab-148">DateTimeOffset</span></span>|<span data-ttu-id="dc9ab-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc9ab-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dc9ab-150">version</span><span class="sxs-lookup"><span data-stu-id="dc9ab-150">version</span></span>|<span data-ttu-id="dc9ab-151">Int32</span><span class="sxs-lookup"><span data-stu-id="dc9ab-151">Int32</span></span>|<span data-ttu-id="dc9ab-152">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dc9ab-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="dc9ab-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="dc9ab-153">iosRestriction</span></span>|[<span data-ttu-id="dc9ab-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="dc9ab-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="dc9ab-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-155">Not yet documented</span></span>|
|<span data-ttu-id="dc9ab-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="dc9ab-156">windowsRestriction</span></span>|[<span data-ttu-id="dc9ab-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="dc9ab-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="dc9ab-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-158">Not yet documented</span></span>|
|<span data-ttu-id="dc9ab-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="dc9ab-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="dc9ab-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="dc9ab-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="dc9ab-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-161">Not yet documented</span></span>|
|<span data-ttu-id="dc9ab-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="dc9ab-162">androidRestriction</span></span>|[<span data-ttu-id="dc9ab-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="dc9ab-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="dc9ab-164">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-164">Not yet documented</span></span>|
|<span data-ttu-id="dc9ab-165">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="dc9ab-165">macOSRestriction</span></span>|[<span data-ttu-id="dc9ab-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="dc9ab-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="dc9ab-167">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dc9ab-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc9ab-168">Response</span></span>
<span data-ttu-id="dc9ab-169">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-169">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc9ab-170">Пример</span><span class="sxs-lookup"><span data-stu-id="dc9ab-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc9ab-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc9ab-171">Request</span></span>
<span data-ttu-id="dc9ab-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 1650

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="dc9ab-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc9ab-173">Response</span></span>
<span data-ttu-id="dc9ab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc9ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1822

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```









