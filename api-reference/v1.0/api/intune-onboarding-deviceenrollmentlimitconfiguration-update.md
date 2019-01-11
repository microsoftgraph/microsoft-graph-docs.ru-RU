---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f41238c42159f40821b2913f51e0b46a1f21725d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804916"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="47181-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="47181-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="47181-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="47181-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47181-105">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47181-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47181-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="47181-106">Prerequisites</span></span>
<span data-ttu-id="47181-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47181-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47181-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47181-109">Permission type</span></span>|<span data-ttu-id="47181-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47181-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47181-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47181-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47181-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47181-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="47181-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47181-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47181-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47181-114">Not supported.</span></span>|
|<span data-ttu-id="47181-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47181-115">Application</span></span>|<span data-ttu-id="47181-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47181-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47181-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47181-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="47181-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47181-118">Request headers</span></span>
|<span data-ttu-id="47181-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47181-119">Header</span></span>|<span data-ttu-id="47181-120">Значение</span><span class="sxs-lookup"><span data-stu-id="47181-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47181-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47181-121">Authorization</span></span>|<span data-ttu-id="47181-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="47181-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47181-123">Accept</span><span class="sxs-lookup"><span data-stu-id="47181-123">Accept</span></span>|<span data-ttu-id="47181-124">application/json</span><span class="sxs-lookup"><span data-stu-id="47181-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47181-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47181-125">Request body</span></span>
<span data-ttu-id="47181-126">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47181-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="47181-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47181-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="47181-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="47181-128">Property</span></span>|<span data-ttu-id="47181-129">Тип</span><span class="sxs-lookup"><span data-stu-id="47181-129">Type</span></span>|<span data-ttu-id="47181-130">Описание</span><span class="sxs-lookup"><span data-stu-id="47181-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47181-131">id</span><span class="sxs-lookup"><span data-stu-id="47181-131">id</span></span>|<span data-ttu-id="47181-132">String</span><span class="sxs-lookup"><span data-stu-id="47181-132">String</span></span>|<span data-ttu-id="47181-133">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47181-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="47181-134">displayName</span><span class="sxs-lookup"><span data-stu-id="47181-134">displayName</span></span>|<span data-ttu-id="47181-135">String</span><span class="sxs-lookup"><span data-stu-id="47181-135">String</span></span>|<span data-ttu-id="47181-136">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47181-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="47181-137">описание</span><span class="sxs-lookup"><span data-stu-id="47181-137">description</span></span>|<span data-ttu-id="47181-138">String</span><span class="sxs-lookup"><span data-stu-id="47181-138">String</span></span>|<span data-ttu-id="47181-139">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47181-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="47181-140">priority</span><span class="sxs-lookup"><span data-stu-id="47181-140">priority</span></span>|<span data-ttu-id="47181-141">Int32</span><span class="sxs-lookup"><span data-stu-id="47181-141">Int32</span></span>|<span data-ttu-id="47181-142">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47181-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="47181-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47181-143">createdDateTime</span></span>|<span data-ttu-id="47181-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47181-144">DateTimeOffset</span></span>|<span data-ttu-id="47181-145">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47181-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="47181-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47181-146">lastModifiedDateTime</span></span>|<span data-ttu-id="47181-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47181-147">DateTimeOffset</span></span>|<span data-ttu-id="47181-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47181-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="47181-149">version</span><span class="sxs-lookup"><span data-stu-id="47181-149">version</span></span>|<span data-ttu-id="47181-150">Int32</span><span class="sxs-lookup"><span data-stu-id="47181-150">Int32</span></span>|<span data-ttu-id="47181-151">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47181-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="47181-152">limit</span><span class="sxs-lookup"><span data-stu-id="47181-152">limit</span></span>|<span data-ttu-id="47181-153">Int32</span><span class="sxs-lookup"><span data-stu-id="47181-153">Int32</span></span>|<span data-ttu-id="47181-154">Н/Д</span><span class="sxs-lookup"><span data-stu-id="47181-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="47181-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="47181-155">Response</span></span>
<span data-ttu-id="47181-156">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="47181-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47181-157">Пример</span><span class="sxs-lookup"><span data-stu-id="47181-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="47181-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="47181-158">Request</span></span>
<span data-ttu-id="47181-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47181-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="47181-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="47181-160">Response</span></span>
<span data-ttu-id="47181-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="47181-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```



