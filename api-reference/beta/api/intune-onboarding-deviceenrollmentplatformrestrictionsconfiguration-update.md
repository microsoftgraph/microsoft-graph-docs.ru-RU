---
title: Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Обновление свойств объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2897815a7324f88d4c10c4e5c940bc2d6b078cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528885"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="273c2-103">Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="273c2-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="273c2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="273c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="273c2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="273c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="273c2-106">Обновление свойств объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="273c2-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="273c2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="273c2-107">Prerequisites</span></span>
<span data-ttu-id="273c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="273c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="273c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="273c2-110">Permission type</span></span>|<span data-ttu-id="273c2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="273c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="273c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="273c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="273c2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="273c2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="273c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="273c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="273c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="273c2-115">Not supported.</span></span>|
|<span data-ttu-id="273c2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="273c2-116">Application</span></span>|<span data-ttu-id="273c2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="273c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="273c2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="273c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="273c2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="273c2-119">Request headers</span></span>
|<span data-ttu-id="273c2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="273c2-120">Header</span></span>|<span data-ttu-id="273c2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="273c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="273c2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="273c2-122">Authorization</span></span>|<span data-ttu-id="273c2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="273c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="273c2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="273c2-124">Accept</span></span>|<span data-ttu-id="273c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="273c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="273c2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="273c2-126">Request body</span></span>
<span data-ttu-id="273c2-127">В теле запроса добавьте представление объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="273c2-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="273c2-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="273c2-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="273c2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="273c2-129">Property</span></span>|<span data-ttu-id="273c2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="273c2-130">Type</span></span>|<span data-ttu-id="273c2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="273c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="273c2-132">id</span><span class="sxs-lookup"><span data-stu-id="273c2-132">id</span></span>|<span data-ttu-id="273c2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="273c2-133">String</span></span>|<span data-ttu-id="273c2-134">Идентификатор конфигурации страницы состояния регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="273c2-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="273c2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="273c2-135">displayName</span></span>|<span data-ttu-id="273c2-136">String</span><span class="sxs-lookup"><span data-stu-id="273c2-136">String</span></span>|<span data-ttu-id="273c2-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="273c2-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="273c2-138">description</span><span class="sxs-lookup"><span data-stu-id="273c2-138">description</span></span>|<span data-ttu-id="273c2-139">String</span><span class="sxs-lookup"><span data-stu-id="273c2-139">String</span></span>|<span data-ttu-id="273c2-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="273c2-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="273c2-141">priority</span><span class="sxs-lookup"><span data-stu-id="273c2-141">priority</span></span>|<span data-ttu-id="273c2-142">Int32</span><span class="sxs-lookup"><span data-stu-id="273c2-142">Int32</span></span>|<span data-ttu-id="273c2-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="273c2-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="273c2-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="273c2-144">createdDateTime</span></span>|<span data-ttu-id="273c2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="273c2-145">DateTimeOffset</span></span>|<span data-ttu-id="273c2-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="273c2-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="273c2-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="273c2-147">lastModifiedDateTime</span></span>|<span data-ttu-id="273c2-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="273c2-148">DateTimeOffset</span></span>|<span data-ttu-id="273c2-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="273c2-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="273c2-150">version</span><span class="sxs-lookup"><span data-stu-id="273c2-150">version</span></span>|<span data-ttu-id="273c2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="273c2-151">Int32</span></span>|<span data-ttu-id="273c2-152">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="273c2-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="273c2-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-153">iosRestriction</span></span>|[<span data-ttu-id="273c2-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="273c2-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="273c2-155">Not yet documented</span></span>|
|<span data-ttu-id="273c2-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-156">windowsRestriction</span></span>|[<span data-ttu-id="273c2-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="273c2-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="273c2-158">Not yet documented</span></span>|
|<span data-ttu-id="273c2-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="273c2-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="273c2-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="273c2-161">Not yet documented</span></span>|
|<span data-ttu-id="273c2-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-162">androidRestriction</span></span>|[<span data-ttu-id="273c2-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="273c2-164">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="273c2-164">Not yet documented</span></span>|
|<span data-ttu-id="273c2-165">Андроидфорворкрестриктион</span><span class="sxs-lookup"><span data-stu-id="273c2-165">androidForWorkRestriction</span></span>|[<span data-ttu-id="273c2-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="273c2-167">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="273c2-167">Not yet documented</span></span>|
|<span data-ttu-id="273c2-168">Макрестриктион</span><span class="sxs-lookup"><span data-stu-id="273c2-168">macRestriction</span></span>|[<span data-ttu-id="273c2-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="273c2-170">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="273c2-170">Not yet documented</span></span>|
|<span data-ttu-id="273c2-171">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-171">macOSRestriction</span></span>|[<span data-ttu-id="273c2-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="273c2-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="273c2-173">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="273c2-173">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="273c2-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="273c2-174">Response</span></span>
<span data-ttu-id="273c2-175">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="273c2-175">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="273c2-176">Пример</span><span class="sxs-lookup"><span data-stu-id="273c2-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="273c2-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="273c2-177">Request</span></span>
<span data-ttu-id="273c2-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="273c2-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="273c2-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="273c2-179">Response</span></span>
<span data-ttu-id="273c2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="273c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





