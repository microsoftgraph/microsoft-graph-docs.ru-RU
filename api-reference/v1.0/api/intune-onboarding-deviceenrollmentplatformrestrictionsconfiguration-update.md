---
title: Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Обновление свойств объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b8b877e81512bf6994cc29b9bcec1e7f943f98c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255901"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="9a8d8-103">Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a8d8-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="9a8d8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a8d8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a8d8-105">Обновление свойств объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a8d8-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a8d8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9a8d8-106">Prerequisites</span></span>
<span data-ttu-id="9a8d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a8d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9a8d8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a8d8-109">Permission type</span></span>|<span data-ttu-id="9a8d8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a8d8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a8d8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a8d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9a8d8-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a8d8-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9a8d8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a8d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a8d8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a8d8-114">Not supported.</span></span>|
|<span data-ttu-id="9a8d8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a8d8-115">Application</span></span>|<span data-ttu-id="9a8d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a8d8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a8d8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a8d8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9a8d8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a8d8-118">Request headers</span></span>
|<span data-ttu-id="9a8d8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a8d8-119">Header</span></span>|<span data-ttu-id="9a8d8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9a8d8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a8d8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a8d8-121">Authorization</span></span>|<span data-ttu-id="9a8d8-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9a8d8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a8d8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9a8d8-123">Accept</span></span>|<span data-ttu-id="9a8d8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9a8d8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a8d8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a8d8-125">Request body</span></span>
<span data-ttu-id="9a8d8-126">В теле запроса добавьте представление объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a8d8-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="9a8d8-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a8d8-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="9a8d8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a8d8-128">Property</span></span>|<span data-ttu-id="9a8d8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9a8d8-129">Type</span></span>|<span data-ttu-id="9a8d8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9a8d8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a8d8-131">id</span><span class="sxs-lookup"><span data-stu-id="9a8d8-131">id</span></span>|<span data-ttu-id="9a8d8-132">String</span><span class="sxs-lookup"><span data-stu-id="9a8d8-132">String</span></span>|<span data-ttu-id="9a8d8-133">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a8d8-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a8d8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9a8d8-134">displayName</span></span>|<span data-ttu-id="9a8d8-135">String</span><span class="sxs-lookup"><span data-stu-id="9a8d8-135">String</span></span>|<span data-ttu-id="9a8d8-136">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a8d8-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a8d8-137">description</span><span class="sxs-lookup"><span data-stu-id="9a8d8-137">description</span></span>|<span data-ttu-id="9a8d8-138">String</span><span class="sxs-lookup"><span data-stu-id="9a8d8-138">String</span></span>|<span data-ttu-id="9a8d8-139">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a8d8-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a8d8-140">priority</span><span class="sxs-lookup"><span data-stu-id="9a8d8-140">priority</span></span>|<span data-ttu-id="9a8d8-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9a8d8-141">Int32</span></span>|<span data-ttu-id="9a8d8-142">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a8d8-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a8d8-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a8d8-143">createdDateTime</span></span>|<span data-ttu-id="9a8d8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a8d8-144">DateTimeOffset</span></span>|<span data-ttu-id="9a8d8-145">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a8d8-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a8d8-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a8d8-146">lastModifiedDateTime</span></span>|<span data-ttu-id="9a8d8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a8d8-147">DateTimeOffset</span></span>|<span data-ttu-id="9a8d8-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a8d8-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a8d8-149">version</span><span class="sxs-lookup"><span data-stu-id="9a8d8-149">version</span></span>|<span data-ttu-id="9a8d8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9a8d8-150">Int32</span></span>|<span data-ttu-id="9a8d8-151">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a8d8-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9a8d8-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="9a8d8-152">iosRestriction</span></span>|[<span data-ttu-id="9a8d8-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9a8d8-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9a8d8-154">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9a8d8-154">Not yet documented</span></span>|
|<span data-ttu-id="9a8d8-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="9a8d8-155">windowsRestriction</span></span>|[<span data-ttu-id="9a8d8-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9a8d8-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9a8d8-157">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9a8d8-157">Not yet documented</span></span>|
|<span data-ttu-id="9a8d8-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="9a8d8-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="9a8d8-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9a8d8-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9a8d8-160">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9a8d8-160">Not yet documented</span></span>|
|<span data-ttu-id="9a8d8-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="9a8d8-161">androidRestriction</span></span>|[<span data-ttu-id="9a8d8-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9a8d8-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9a8d8-163">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9a8d8-163">Not yet documented</span></span>|
|<span data-ttu-id="9a8d8-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="9a8d8-164">macOSRestriction</span></span>|[<span data-ttu-id="9a8d8-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="9a8d8-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="9a8d8-166">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9a8d8-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9a8d8-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a8d8-167">Response</span></span>
<span data-ttu-id="9a8d8-168">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9a8d8-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a8d8-169">Пример</span><span class="sxs-lookup"><span data-stu-id="9a8d8-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a8d8-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a8d8-170">Request</span></span>
<span data-ttu-id="9a8d8-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a8d8-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9a8d8-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a8d8-172">Response</span></span>
<span data-ttu-id="9a8d8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9a8d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



