---
title: Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Обновление свойств объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a0fe37e0391c55a8b53a38d923543cb7b12f390
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974719"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="ffad2-103">Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="ffad2-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="ffad2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ffad2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffad2-105">Обновление свойств объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffad2-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffad2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ffad2-106">Prerequisites</span></span>
<span data-ttu-id="ffad2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffad2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffad2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffad2-109">Permission type</span></span>|<span data-ttu-id="ffad2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffad2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffad2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffad2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ffad2-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffad2-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ffad2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffad2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffad2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffad2-114">Not supported.</span></span>|
|<span data-ttu-id="ffad2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffad2-115">Application</span></span>|<span data-ttu-id="ffad2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffad2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffad2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffad2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ffad2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffad2-118">Request headers</span></span>
|<span data-ttu-id="ffad2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffad2-119">Header</span></span>|<span data-ttu-id="ffad2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ffad2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffad2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffad2-121">Authorization</span></span>|<span data-ttu-id="ffad2-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffad2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffad2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ffad2-123">Accept</span></span>|<span data-ttu-id="ffad2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ffad2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffad2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ffad2-125">Request body</span></span>
<span data-ttu-id="ffad2-126">В теле запроса добавьте представление объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffad2-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="ffad2-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffad2-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="ffad2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffad2-128">Property</span></span>|<span data-ttu-id="ffad2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ffad2-129">Type</span></span>|<span data-ttu-id="ffad2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ffad2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffad2-131">id</span><span class="sxs-lookup"><span data-stu-id="ffad2-131">id</span></span>|<span data-ttu-id="ffad2-132">String</span><span class="sxs-lookup"><span data-stu-id="ffad2-132">String</span></span>|<span data-ttu-id="ffad2-133">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffad2-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffad2-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ffad2-134">displayName</span></span>|<span data-ttu-id="ffad2-135">Строка</span><span class="sxs-lookup"><span data-stu-id="ffad2-135">String</span></span>|<span data-ttu-id="ffad2-136">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffad2-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffad2-137">description</span><span class="sxs-lookup"><span data-stu-id="ffad2-137">description</span></span>|<span data-ttu-id="ffad2-138">String</span><span class="sxs-lookup"><span data-stu-id="ffad2-138">String</span></span>|<span data-ttu-id="ffad2-139">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffad2-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffad2-140">priority</span><span class="sxs-lookup"><span data-stu-id="ffad2-140">priority</span></span>|<span data-ttu-id="ffad2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ffad2-141">Int32</span></span>|<span data-ttu-id="ffad2-142">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffad2-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffad2-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffad2-143">createdDateTime</span></span>|<span data-ttu-id="ffad2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffad2-144">DateTimeOffset</span></span>|<span data-ttu-id="ffad2-145">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffad2-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffad2-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffad2-146">lastModifiedDateTime</span></span>|<span data-ttu-id="ffad2-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffad2-147">DateTimeOffset</span></span>|<span data-ttu-id="ffad2-148">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffad2-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffad2-149">version</span><span class="sxs-lookup"><span data-stu-id="ffad2-149">version</span></span>|<span data-ttu-id="ffad2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ffad2-150">Int32</span></span>|<span data-ttu-id="ffad2-151">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffad2-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ffad2-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="ffad2-152">iosRestriction</span></span>|[<span data-ttu-id="ffad2-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ffad2-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ffad2-154">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ffad2-154">Not yet documented</span></span>|
|<span data-ttu-id="ffad2-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="ffad2-155">windowsRestriction</span></span>|[<span data-ttu-id="ffad2-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ffad2-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ffad2-157">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ffad2-157">Not yet documented</span></span>|
|<span data-ttu-id="ffad2-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="ffad2-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="ffad2-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ffad2-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ffad2-160">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ffad2-160">Not yet documented</span></span>|
|<span data-ttu-id="ffad2-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="ffad2-161">androidRestriction</span></span>|[<span data-ttu-id="ffad2-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ffad2-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ffad2-163">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ffad2-163">Not yet documented</span></span>|
|<span data-ttu-id="ffad2-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="ffad2-164">macOSRestriction</span></span>|[<span data-ttu-id="ffad2-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ffad2-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ffad2-166">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ffad2-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ffad2-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffad2-167">Response</span></span>
<span data-ttu-id="ffad2-168">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ffad2-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffad2-169">Пример</span><span class="sxs-lookup"><span data-stu-id="ffad2-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffad2-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffad2-170">Request</span></span>
<span data-ttu-id="ffad2-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffad2-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="ffad2-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffad2-172">Response</span></span>
<span data-ttu-id="ffad2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ffad2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



