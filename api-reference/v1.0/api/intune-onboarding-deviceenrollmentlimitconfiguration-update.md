---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8b228b1e89f308e8afdb9619dc72e43dc784371
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43418541"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="25827-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="25827-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="25827-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25827-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25827-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25827-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25827-106">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25827-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25827-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="25827-107">Prerequisites</span></span>
<span data-ttu-id="25827-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25827-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25827-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25827-110">Permission type</span></span>|<span data-ttu-id="25827-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25827-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25827-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25827-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25827-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25827-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="25827-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25827-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25827-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25827-115">Not supported.</span></span>|
|<span data-ttu-id="25827-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25827-116">Application</span></span>|<span data-ttu-id="25827-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25827-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25827-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25827-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="25827-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25827-119">Request headers</span></span>
|<span data-ttu-id="25827-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25827-120">Header</span></span>|<span data-ttu-id="25827-121">Значение</span><span class="sxs-lookup"><span data-stu-id="25827-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25827-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25827-122">Authorization</span></span>|<span data-ttu-id="25827-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25827-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25827-124">Accept</span><span class="sxs-lookup"><span data-stu-id="25827-124">Accept</span></span>|<span data-ttu-id="25827-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25827-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25827-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25827-126">Request body</span></span>
<span data-ttu-id="25827-127">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25827-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="25827-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25827-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="25827-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="25827-129">Property</span></span>|<span data-ttu-id="25827-130">Тип</span><span class="sxs-lookup"><span data-stu-id="25827-130">Type</span></span>|<span data-ttu-id="25827-131">Описание</span><span class="sxs-lookup"><span data-stu-id="25827-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25827-132">id</span><span class="sxs-lookup"><span data-stu-id="25827-132">id</span></span>|<span data-ttu-id="25827-133">String</span><span class="sxs-lookup"><span data-stu-id="25827-133">String</span></span>|<span data-ttu-id="25827-134">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25827-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25827-135">displayName</span><span class="sxs-lookup"><span data-stu-id="25827-135">displayName</span></span>|<span data-ttu-id="25827-136">Строка</span><span class="sxs-lookup"><span data-stu-id="25827-136">String</span></span>|<span data-ttu-id="25827-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25827-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25827-138">description</span><span class="sxs-lookup"><span data-stu-id="25827-138">description</span></span>|<span data-ttu-id="25827-139">String</span><span class="sxs-lookup"><span data-stu-id="25827-139">String</span></span>|<span data-ttu-id="25827-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25827-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25827-141">priority</span><span class="sxs-lookup"><span data-stu-id="25827-141">priority</span></span>|<span data-ttu-id="25827-142">Int32</span><span class="sxs-lookup"><span data-stu-id="25827-142">Int32</span></span>|<span data-ttu-id="25827-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25827-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25827-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25827-144">createdDateTime</span></span>|<span data-ttu-id="25827-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25827-145">DateTimeOffset</span></span>|<span data-ttu-id="25827-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25827-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25827-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25827-147">lastModifiedDateTime</span></span>|<span data-ttu-id="25827-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25827-148">DateTimeOffset</span></span>|<span data-ttu-id="25827-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25827-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25827-150">version</span><span class="sxs-lookup"><span data-stu-id="25827-150">version</span></span>|<span data-ttu-id="25827-151">Int32</span><span class="sxs-lookup"><span data-stu-id="25827-151">Int32</span></span>|<span data-ttu-id="25827-152">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25827-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="25827-153">limit</span><span class="sxs-lookup"><span data-stu-id="25827-153">limit</span></span>|<span data-ttu-id="25827-154">Int32</span><span class="sxs-lookup"><span data-stu-id="25827-154">Int32</span></span>|<span data-ttu-id="25827-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="25827-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="25827-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="25827-156">Response</span></span>
<span data-ttu-id="25827-157">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="25827-157">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25827-158">Пример</span><span class="sxs-lookup"><span data-stu-id="25827-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="25827-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="25827-159">Request</span></span>
<span data-ttu-id="25827-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25827-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="25827-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="25827-161">Response</span></span>
<span data-ttu-id="25827-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25827-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






