---
title: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 82ff5652cb70cb05f8df5620ba1ef59f601d6645
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846930"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="1495c-103">Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="1495c-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="1495c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1495c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1495c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1495c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1495c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1495c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1495c-107">Создание объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1495c-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1495c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1495c-108">Prerequisites</span></span>
<span data-ttu-id="1495c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1495c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1495c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1495c-111">Permission type</span></span>|<span data-ttu-id="1495c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1495c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1495c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1495c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1495c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1495c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1495c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1495c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1495c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1495c-116">Not supported.</span></span>|
|<span data-ttu-id="1495c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1495c-117">Application</span></span>|<span data-ttu-id="1495c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1495c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1495c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1495c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1495c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1495c-120">Request headers</span></span>
|<span data-ttu-id="1495c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1495c-121">Header</span></span>|<span data-ttu-id="1495c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1495c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1495c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1495c-123">Authorization</span></span>|<span data-ttu-id="1495c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1495c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1495c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1495c-125">Accept</span></span>|<span data-ttu-id="1495c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1495c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1495c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1495c-127">Request body</span></span>
<span data-ttu-id="1495c-128">В теле запроса добавьте представление объекта deviceEnrollmentPlatformRestrictionsConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1495c-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="1495c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1495c-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="1495c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1495c-130">Property</span></span>|<span data-ttu-id="1495c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1495c-131">Type</span></span>|<span data-ttu-id="1495c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1495c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1495c-133">id</span><span class="sxs-lookup"><span data-stu-id="1495c-133">id</span></span>|<span data-ttu-id="1495c-134">String</span><span class="sxs-lookup"><span data-stu-id="1495c-134">String</span></span>|<span data-ttu-id="1495c-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1495c-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1495c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1495c-136">displayName</span></span>|<span data-ttu-id="1495c-137">String</span><span class="sxs-lookup"><span data-stu-id="1495c-137">String</span></span>|<span data-ttu-id="1495c-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1495c-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1495c-139">описание</span><span class="sxs-lookup"><span data-stu-id="1495c-139">description</span></span>|<span data-ttu-id="1495c-140">String</span><span class="sxs-lookup"><span data-stu-id="1495c-140">String</span></span>|<span data-ttu-id="1495c-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1495c-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1495c-142">priority</span><span class="sxs-lookup"><span data-stu-id="1495c-142">priority</span></span>|<span data-ttu-id="1495c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1495c-143">Int32</span></span>|<span data-ttu-id="1495c-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1495c-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1495c-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1495c-145">createdDateTime</span></span>|<span data-ttu-id="1495c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1495c-146">DateTimeOffset</span></span>|<span data-ttu-id="1495c-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1495c-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1495c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1495c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="1495c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1495c-149">DateTimeOffset</span></span>|<span data-ttu-id="1495c-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1495c-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1495c-151">version</span><span class="sxs-lookup"><span data-stu-id="1495c-151">version</span></span>|<span data-ttu-id="1495c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1495c-152">Int32</span></span>|<span data-ttu-id="1495c-153">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1495c-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1495c-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-154">iosRestriction</span></span>|[<span data-ttu-id="1495c-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1495c-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1495c-156">Not yet documented</span></span>|
|<span data-ttu-id="1495c-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-157">windowsRestriction</span></span>|[<span data-ttu-id="1495c-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1495c-159">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1495c-159">Not yet documented</span></span>|
|<span data-ttu-id="1495c-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="1495c-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1495c-162">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1495c-162">Not yet documented</span></span>|
|<span data-ttu-id="1495c-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-163">androidRestriction</span></span>|[<span data-ttu-id="1495c-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1495c-165">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1495c-165">Not yet documented</span></span>|
|<span data-ttu-id="1495c-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="1495c-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1495c-168">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1495c-168">Not yet documented</span></span>|
|<span data-ttu-id="1495c-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-169">macRestriction</span></span>|[<span data-ttu-id="1495c-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1495c-171">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1495c-171">Not yet documented</span></span>|
|<span data-ttu-id="1495c-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-172">macOSRestriction</span></span>|[<span data-ttu-id="1495c-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1495c-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1495c-174">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1495c-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1495c-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="1495c-175">Response</span></span>
<span data-ttu-id="1495c-176">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1495c-176">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1495c-177">Пример</span><span class="sxs-lookup"><span data-stu-id="1495c-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="1495c-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="1495c-178">Request</span></span>
<span data-ttu-id="1495c-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1495c-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 2295

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="1495c-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="1495c-180">Response</span></span>
<span data-ttu-id="1495c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1495c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





