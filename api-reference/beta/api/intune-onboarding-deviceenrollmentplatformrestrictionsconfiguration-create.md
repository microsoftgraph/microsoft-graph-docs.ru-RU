---
title: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b2910d8b87535464f449a8649173102aab8b134
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407279"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="edfcf-103">Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="edfcf-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="edfcf-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="edfcf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="edfcf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edfcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="edfcf-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edfcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edfcf-107">Создание объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edfcf-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edfcf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="edfcf-108">Prerequisites</span></span>
<span data-ttu-id="edfcf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="edfcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="edfcf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edfcf-111">Permission type</span></span>|<span data-ttu-id="edfcf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="edfcf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edfcf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edfcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="edfcf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edfcf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="edfcf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edfcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edfcf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edfcf-116">Not supported.</span></span>|
|<span data-ttu-id="edfcf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edfcf-117">Application</span></span>|<span data-ttu-id="edfcf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edfcf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edfcf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edfcf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="edfcf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edfcf-120">Request headers</span></span>
|<span data-ttu-id="edfcf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="edfcf-121">Header</span></span>|<span data-ttu-id="edfcf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="edfcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edfcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="edfcf-123">Authorization</span></span>|<span data-ttu-id="edfcf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="edfcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edfcf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="edfcf-125">Accept</span></span>|<span data-ttu-id="edfcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edfcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edfcf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="edfcf-127">Request body</span></span>
<span data-ttu-id="edfcf-128">В теле запроса добавьте представление объекта deviceEnrollmentPlatformRestrictionsConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edfcf-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="edfcf-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="edfcf-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="edfcf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="edfcf-130">Property</span></span>|<span data-ttu-id="edfcf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="edfcf-131">Type</span></span>|<span data-ttu-id="edfcf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="edfcf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edfcf-133">id</span><span class="sxs-lookup"><span data-stu-id="edfcf-133">id</span></span>|<span data-ttu-id="edfcf-134">String</span><span class="sxs-lookup"><span data-stu-id="edfcf-134">String</span></span>|<span data-ttu-id="edfcf-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edfcf-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edfcf-136">displayName</span><span class="sxs-lookup"><span data-stu-id="edfcf-136">displayName</span></span>|<span data-ttu-id="edfcf-137">String</span><span class="sxs-lookup"><span data-stu-id="edfcf-137">String</span></span>|<span data-ttu-id="edfcf-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edfcf-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edfcf-139">description</span><span class="sxs-lookup"><span data-stu-id="edfcf-139">description</span></span>|<span data-ttu-id="edfcf-140">String</span><span class="sxs-lookup"><span data-stu-id="edfcf-140">String</span></span>|<span data-ttu-id="edfcf-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edfcf-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edfcf-142">priority</span><span class="sxs-lookup"><span data-stu-id="edfcf-142">priority</span></span>|<span data-ttu-id="edfcf-143">Int32</span><span class="sxs-lookup"><span data-stu-id="edfcf-143">Int32</span></span>|<span data-ttu-id="edfcf-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edfcf-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edfcf-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="edfcf-145">createdDateTime</span></span>|<span data-ttu-id="edfcf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edfcf-146">DateTimeOffset</span></span>|<span data-ttu-id="edfcf-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edfcf-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edfcf-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="edfcf-148">lastModifiedDateTime</span></span>|<span data-ttu-id="edfcf-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edfcf-149">DateTimeOffset</span></span>|<span data-ttu-id="edfcf-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edfcf-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edfcf-151">version</span><span class="sxs-lookup"><span data-stu-id="edfcf-151">version</span></span>|<span data-ttu-id="edfcf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="edfcf-152">Int32</span></span>|<span data-ttu-id="edfcf-153">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edfcf-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="edfcf-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-154">iosRestriction</span></span>|[<span data-ttu-id="edfcf-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="edfcf-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="edfcf-156">Not yet documented</span></span>|
|<span data-ttu-id="edfcf-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-157">windowsRestriction</span></span>|[<span data-ttu-id="edfcf-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="edfcf-159">Н/Д</span><span class="sxs-lookup"><span data-stu-id="edfcf-159">Not yet documented</span></span>|
|<span data-ttu-id="edfcf-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="edfcf-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="edfcf-162">Н/Д</span><span class="sxs-lookup"><span data-stu-id="edfcf-162">Not yet documented</span></span>|
|<span data-ttu-id="edfcf-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-163">androidRestriction</span></span>|[<span data-ttu-id="edfcf-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="edfcf-165">Н/Д</span><span class="sxs-lookup"><span data-stu-id="edfcf-165">Not yet documented</span></span>|
|<span data-ttu-id="edfcf-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="edfcf-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="edfcf-168">Н/Д</span><span class="sxs-lookup"><span data-stu-id="edfcf-168">Not yet documented</span></span>|
|<span data-ttu-id="edfcf-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-169">macRestriction</span></span>|[<span data-ttu-id="edfcf-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="edfcf-171">Н/Д</span><span class="sxs-lookup"><span data-stu-id="edfcf-171">Not yet documented</span></span>|
|<span data-ttu-id="edfcf-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-172">macOSRestriction</span></span>|[<span data-ttu-id="edfcf-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="edfcf-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="edfcf-174">Н/Д</span><span class="sxs-lookup"><span data-stu-id="edfcf-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="edfcf-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="edfcf-175">Response</span></span>
<span data-ttu-id="edfcf-176">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="edfcf-176">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edfcf-177">Пример</span><span class="sxs-lookup"><span data-stu-id="edfcf-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="edfcf-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="edfcf-178">Request</span></span>
<span data-ttu-id="edfcf-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edfcf-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="edfcf-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="edfcf-180">Response</span></span>
<span data-ttu-id="edfcf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="edfcf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




