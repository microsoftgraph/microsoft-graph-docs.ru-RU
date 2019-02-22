---
title: Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Обновление свойств объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4b09aff97602974fbd4751a9392a8ff10796043
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139825"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="e145e-103">Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="e145e-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="e145e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e145e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e145e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e145e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e145e-106">Обновление свойств объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e145e-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e145e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e145e-107">Prerequisites</span></span>
<span data-ttu-id="e145e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e145e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e145e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e145e-110">Permission type</span></span>|<span data-ttu-id="e145e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e145e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e145e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e145e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e145e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e145e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e145e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e145e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e145e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e145e-115">Not supported.</span></span>|
|<span data-ttu-id="e145e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e145e-116">Application</span></span>|<span data-ttu-id="e145e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e145e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e145e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e145e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e145e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e145e-119">Request headers</span></span>
|<span data-ttu-id="e145e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e145e-120">Header</span></span>|<span data-ttu-id="e145e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e145e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e145e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e145e-122">Authorization</span></span>|<span data-ttu-id="e145e-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e145e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e145e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e145e-124">Accept</span></span>|<span data-ttu-id="e145e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e145e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e145e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e145e-126">Request body</span></span>
<span data-ttu-id="e145e-127">В теле запроса добавьте представление объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e145e-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="e145e-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e145e-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="e145e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e145e-129">Property</span></span>|<span data-ttu-id="e145e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e145e-130">Type</span></span>|<span data-ttu-id="e145e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e145e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e145e-132">id</span><span class="sxs-lookup"><span data-stu-id="e145e-132">id</span></span>|<span data-ttu-id="e145e-133">String</span><span class="sxs-lookup"><span data-stu-id="e145e-133">String</span></span>|<span data-ttu-id="e145e-134">Идентификатор конфигурации страницы состояния регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e145e-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e145e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e145e-135">displayName</span></span>|<span data-ttu-id="e145e-136">String</span><span class="sxs-lookup"><span data-stu-id="e145e-136">String</span></span>|<span data-ttu-id="e145e-137">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e145e-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e145e-138">description</span><span class="sxs-lookup"><span data-stu-id="e145e-138">description</span></span>|<span data-ttu-id="e145e-139">String</span><span class="sxs-lookup"><span data-stu-id="e145e-139">String</span></span>|<span data-ttu-id="e145e-140">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e145e-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e145e-141">priority</span><span class="sxs-lookup"><span data-stu-id="e145e-141">priority</span></span>|<span data-ttu-id="e145e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e145e-142">Int32</span></span>|<span data-ttu-id="e145e-143">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e145e-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e145e-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e145e-144">createdDateTime</span></span>|<span data-ttu-id="e145e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e145e-145">DateTimeOffset</span></span>|<span data-ttu-id="e145e-146">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e145e-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e145e-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e145e-147">lastModifiedDateTime</span></span>|<span data-ttu-id="e145e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e145e-148">DateTimeOffset</span></span>|<span data-ttu-id="e145e-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e145e-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e145e-150">version</span><span class="sxs-lookup"><span data-stu-id="e145e-150">version</span></span>|<span data-ttu-id="e145e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e145e-151">Int32</span></span>|<span data-ttu-id="e145e-152">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e145e-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e145e-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-153">iosRestriction</span></span>|[<span data-ttu-id="e145e-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e145e-155">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e145e-155">Not yet documented</span></span>|
|<span data-ttu-id="e145e-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-156">windowsRestriction</span></span>|[<span data-ttu-id="e145e-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e145e-158">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e145e-158">Not yet documented</span></span>|
|<span data-ttu-id="e145e-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="e145e-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e145e-161">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e145e-161">Not yet documented</span></span>|
|<span data-ttu-id="e145e-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-162">androidRestriction</span></span>|[<span data-ttu-id="e145e-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e145e-164">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e145e-164">Not yet documented</span></span>|
|<span data-ttu-id="e145e-165">Андроидфорворкрестриктион</span><span class="sxs-lookup"><span data-stu-id="e145e-165">androidForWorkRestriction</span></span>|[<span data-ttu-id="e145e-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e145e-167">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e145e-167">Not yet documented</span></span>|
|<span data-ttu-id="e145e-168">Макрестриктион</span><span class="sxs-lookup"><span data-stu-id="e145e-168">macRestriction</span></span>|[<span data-ttu-id="e145e-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e145e-170">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e145e-170">Not yet documented</span></span>|
|<span data-ttu-id="e145e-171">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-171">macOSRestriction</span></span>|[<span data-ttu-id="e145e-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e145e-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e145e-173">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e145e-173">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e145e-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="e145e-174">Response</span></span>
<span data-ttu-id="e145e-175">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e145e-175">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e145e-176">Пример</span><span class="sxs-lookup"><span data-stu-id="e145e-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="e145e-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="e145e-177">Request</span></span>
<span data-ttu-id="e145e-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e145e-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 2231

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
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
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

### <a name="response"></a><span data-ttu-id="e145e-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="e145e-179">Response</span></span>
<span data-ttu-id="e145e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e145e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2403

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
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
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




