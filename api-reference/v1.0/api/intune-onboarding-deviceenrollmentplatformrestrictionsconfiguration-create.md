---
title: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
ms.openlocfilehash: 2815043ae2a0c6f8c2130c413b15337c05fc1749
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324264"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="1d6ef-103">Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="1d6ef-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="1d6ef-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d6ef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d6ef-105">Создание объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d6ef-105">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d6ef-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1d6ef-106">Prerequisites</span></span>
<span data-ttu-id="1d6ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d6ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d6ef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d6ef-109">Permission type</span></span>|<span data-ttu-id="1d6ef-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d6ef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d6ef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d6ef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1d6ef-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d6ef-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1d6ef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d6ef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d6ef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d6ef-114">Not supported.</span></span>|
|<span data-ttu-id="1d6ef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d6ef-115">Application</span></span>|<span data-ttu-id="1d6ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d6ef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d6ef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d6ef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1d6ef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d6ef-118">Request headers</span></span>
|<span data-ttu-id="1d6ef-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d6ef-119">Header</span></span>|<span data-ttu-id="1d6ef-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1d6ef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d6ef-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d6ef-121">Authorization</span></span>|<span data-ttu-id="1d6ef-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1d6ef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d6ef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1d6ef-123">Accept</span></span>|<span data-ttu-id="1d6ef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1d6ef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d6ef-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d6ef-125">Request body</span></span>
<span data-ttu-id="1d6ef-126">В теле запроса добавьте представление объекта deviceEnrollmentPlatformRestrictionsConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d6ef-126">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="1d6ef-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1d6ef-127">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="1d6ef-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d6ef-128">Property</span></span>|<span data-ttu-id="1d6ef-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1d6ef-129">Type</span></span>|<span data-ttu-id="1d6ef-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1d6ef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d6ef-131">id</span><span class="sxs-lookup"><span data-stu-id="1d6ef-131">id</span></span>|<span data-ttu-id="1d6ef-132">String</span><span class="sxs-lookup"><span data-stu-id="1d6ef-132">String</span></span>|<span data-ttu-id="1d6ef-133">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d6ef-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1d6ef-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1d6ef-134">displayName</span></span>|<span data-ttu-id="1d6ef-135">String</span><span class="sxs-lookup"><span data-stu-id="1d6ef-135">String</span></span>|<span data-ttu-id="1d6ef-136">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d6ef-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1d6ef-137">описание</span><span class="sxs-lookup"><span data-stu-id="1d6ef-137">description</span></span>|<span data-ttu-id="1d6ef-138">String</span><span class="sxs-lookup"><span data-stu-id="1d6ef-138">String</span></span>|<span data-ttu-id="1d6ef-139">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d6ef-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1d6ef-140">priority</span><span class="sxs-lookup"><span data-stu-id="1d6ef-140">priority</span></span>|<span data-ttu-id="1d6ef-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1d6ef-141">Int32</span></span>|<span data-ttu-id="1d6ef-142">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d6ef-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1d6ef-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d6ef-143">createdDateTime</span></span>|<span data-ttu-id="1d6ef-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d6ef-144">DateTimeOffset</span></span>|<span data-ttu-id="1d6ef-145">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d6ef-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1d6ef-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d6ef-146">lastModifiedDateTime</span></span>|<span data-ttu-id="1d6ef-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d6ef-147">DateTimeOffset</span></span>|<span data-ttu-id="1d6ef-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d6ef-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1d6ef-149">version</span><span class="sxs-lookup"><span data-stu-id="1d6ef-149">version</span></span>|<span data-ttu-id="1d6ef-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1d6ef-150">Int32</span></span>|<span data-ttu-id="1d6ef-151">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d6ef-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1d6ef-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="1d6ef-152">iosRestriction</span></span>|[<span data-ttu-id="1d6ef-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1d6ef-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1d6ef-154">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1d6ef-154">Not yet documented</span></span>|
|<span data-ttu-id="1d6ef-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="1d6ef-155">windowsRestriction</span></span>|[<span data-ttu-id="1d6ef-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1d6ef-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1d6ef-157">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1d6ef-157">Not yet documented</span></span>|
|<span data-ttu-id="1d6ef-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="1d6ef-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="1d6ef-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1d6ef-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1d6ef-160">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1d6ef-160">Not yet documented</span></span>|
|<span data-ttu-id="1d6ef-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="1d6ef-161">androidRestriction</span></span>|[<span data-ttu-id="1d6ef-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1d6ef-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1d6ef-163">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1d6ef-163">Not yet documented</span></span>|
|<span data-ttu-id="1d6ef-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="1d6ef-164">macOSRestriction</span></span>|[<span data-ttu-id="1d6ef-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1d6ef-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1d6ef-166">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1d6ef-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1d6ef-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d6ef-167">Response</span></span>
<span data-ttu-id="1d6ef-168">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1d6ef-168">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d6ef-169">Пример</span><span class="sxs-lookup"><span data-stu-id="1d6ef-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d6ef-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d6ef-170">Request</span></span>
<span data-ttu-id="1d6ef-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d6ef-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1d6ef-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d6ef-172">Response</span></span>
<span data-ttu-id="1d6ef-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1d6ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



