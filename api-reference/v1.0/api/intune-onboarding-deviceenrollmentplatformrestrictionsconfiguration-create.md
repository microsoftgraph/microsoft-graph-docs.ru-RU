---
title: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10ceea611e932769b69fee4a5c915de570eb1836
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465990"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="a5149-103">Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a5149-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="a5149-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5149-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5149-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5149-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5149-106">Создание объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5149-106">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5149-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a5149-107">Prerequisites</span></span>
<span data-ttu-id="a5149-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5149-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5149-110">Permission type</span></span>|<span data-ttu-id="a5149-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5149-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5149-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5149-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5149-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5149-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a5149-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5149-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5149-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5149-115">Not supported.</span></span>|
|<span data-ttu-id="a5149-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5149-116">Application</span></span>|<span data-ttu-id="a5149-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5149-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5149-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5149-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a5149-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a5149-119">Request headers</span></span>
|<span data-ttu-id="a5149-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5149-120">Header</span></span>|<span data-ttu-id="a5149-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a5149-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5149-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5149-122">Authorization</span></span>|<span data-ttu-id="a5149-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5149-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5149-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a5149-124">Accept</span></span>|<span data-ttu-id="a5149-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5149-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5149-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5149-126">Request body</span></span>
<span data-ttu-id="a5149-127">В теле запроса добавьте представление объекта deviceEnrollmentPlatformRestrictionsConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5149-127">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="a5149-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a5149-128">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="a5149-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5149-129">Property</span></span>|<span data-ttu-id="a5149-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a5149-130">Type</span></span>|<span data-ttu-id="a5149-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a5149-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5149-132">id</span><span class="sxs-lookup"><span data-stu-id="a5149-132">id</span></span>|<span data-ttu-id="a5149-133">String</span><span class="sxs-lookup"><span data-stu-id="a5149-133">String</span></span>|<span data-ttu-id="a5149-134">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5149-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a5149-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a5149-135">displayName</span></span>|<span data-ttu-id="a5149-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a5149-136">String</span></span>|<span data-ttu-id="a5149-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5149-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a5149-138">description</span><span class="sxs-lookup"><span data-stu-id="a5149-138">description</span></span>|<span data-ttu-id="a5149-139">String</span><span class="sxs-lookup"><span data-stu-id="a5149-139">String</span></span>|<span data-ttu-id="a5149-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5149-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a5149-141">priority</span><span class="sxs-lookup"><span data-stu-id="a5149-141">priority</span></span>|<span data-ttu-id="a5149-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a5149-142">Int32</span></span>|<span data-ttu-id="a5149-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5149-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a5149-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5149-144">createdDateTime</span></span>|<span data-ttu-id="a5149-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5149-145">DateTimeOffset</span></span>|<span data-ttu-id="a5149-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5149-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a5149-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5149-147">lastModifiedDateTime</span></span>|<span data-ttu-id="a5149-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5149-148">DateTimeOffset</span></span>|<span data-ttu-id="a5149-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5149-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a5149-150">version</span><span class="sxs-lookup"><span data-stu-id="a5149-150">version</span></span>|<span data-ttu-id="a5149-151">Int32</span><span class="sxs-lookup"><span data-stu-id="a5149-151">Int32</span></span>|<span data-ttu-id="a5149-152">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5149-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a5149-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="a5149-153">iosRestriction</span></span>|[<span data-ttu-id="a5149-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a5149-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a5149-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a5149-155">Not yet documented</span></span>|
|<span data-ttu-id="a5149-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="a5149-156">windowsRestriction</span></span>|[<span data-ttu-id="a5149-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a5149-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a5149-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a5149-158">Not yet documented</span></span>|
|<span data-ttu-id="a5149-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="a5149-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="a5149-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a5149-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a5149-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a5149-161">Not yet documented</span></span>|
|<span data-ttu-id="a5149-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="a5149-162">androidRestriction</span></span>|[<span data-ttu-id="a5149-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a5149-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a5149-164">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a5149-164">Not yet documented</span></span>|
|<span data-ttu-id="a5149-165">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="a5149-165">macOSRestriction</span></span>|[<span data-ttu-id="a5149-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a5149-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a5149-167">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a5149-167">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a5149-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5149-168">Response</span></span>
<span data-ttu-id="a5149-169">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a5149-169">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5149-170">Пример</span><span class="sxs-lookup"><span data-stu-id="a5149-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5149-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5149-171">Request</span></span>
<span data-ttu-id="a5149-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5149-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a5149-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5149-173">Response</span></span>
<span data-ttu-id="a5149-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5149-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






