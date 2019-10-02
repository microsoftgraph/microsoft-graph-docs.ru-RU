---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 48eee8e954f46e7fc65b1a1c512bdc1b47be3233
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362648"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="f01b3-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="f01b3-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="f01b3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f01b3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f01b3-105">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f01b3-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f01b3-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f01b3-106">Prerequisites</span></span>
<span data-ttu-id="f01b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f01b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f01b3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f01b3-109">Permission type</span></span>|<span data-ttu-id="f01b3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f01b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f01b3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f01b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f01b3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f01b3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f01b3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f01b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f01b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f01b3-114">Not supported.</span></span>|
|<span data-ttu-id="f01b3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f01b3-115">Application</span></span>|<span data-ttu-id="f01b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f01b3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f01b3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f01b3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f01b3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f01b3-118">Request headers</span></span>
|<span data-ttu-id="f01b3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f01b3-119">Header</span></span>|<span data-ttu-id="f01b3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f01b3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f01b3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f01b3-121">Authorization</span></span>|<span data-ttu-id="f01b3-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f01b3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f01b3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f01b3-123">Accept</span></span>|<span data-ttu-id="f01b3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f01b3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f01b3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f01b3-125">Request body</span></span>
<span data-ttu-id="f01b3-126">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f01b3-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="f01b3-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f01b3-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="f01b3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f01b3-128">Property</span></span>|<span data-ttu-id="f01b3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f01b3-129">Type</span></span>|<span data-ttu-id="f01b3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f01b3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f01b3-131">id</span><span class="sxs-lookup"><span data-stu-id="f01b3-131">id</span></span>|<span data-ttu-id="f01b3-132">String</span><span class="sxs-lookup"><span data-stu-id="f01b3-132">String</span></span>|<span data-ttu-id="f01b3-133">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f01b3-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f01b3-134">displayName</span><span class="sxs-lookup"><span data-stu-id="f01b3-134">displayName</span></span>|<span data-ttu-id="f01b3-135">Строка</span><span class="sxs-lookup"><span data-stu-id="f01b3-135">String</span></span>|<span data-ttu-id="f01b3-136">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f01b3-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f01b3-137">description</span><span class="sxs-lookup"><span data-stu-id="f01b3-137">description</span></span>|<span data-ttu-id="f01b3-138">String</span><span class="sxs-lookup"><span data-stu-id="f01b3-138">String</span></span>|<span data-ttu-id="f01b3-139">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f01b3-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f01b3-140">priority</span><span class="sxs-lookup"><span data-stu-id="f01b3-140">priority</span></span>|<span data-ttu-id="f01b3-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f01b3-141">Int32</span></span>|<span data-ttu-id="f01b3-142">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f01b3-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f01b3-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f01b3-143">createdDateTime</span></span>|<span data-ttu-id="f01b3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f01b3-144">DateTimeOffset</span></span>|<span data-ttu-id="f01b3-145">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f01b3-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f01b3-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f01b3-146">lastModifiedDateTime</span></span>|<span data-ttu-id="f01b3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f01b3-147">DateTimeOffset</span></span>|<span data-ttu-id="f01b3-148">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f01b3-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f01b3-149">version</span><span class="sxs-lookup"><span data-stu-id="f01b3-149">version</span></span>|<span data-ttu-id="f01b3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f01b3-150">Int32</span></span>|<span data-ttu-id="f01b3-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f01b3-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f01b3-152">limit</span><span class="sxs-lookup"><span data-stu-id="f01b3-152">limit</span></span>|<span data-ttu-id="f01b3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f01b3-153">Int32</span></span>|<span data-ttu-id="f01b3-154">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f01b3-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f01b3-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f01b3-155">Response</span></span>
<span data-ttu-id="f01b3-156">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f01b3-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f01b3-157">Пример</span><span class="sxs-lookup"><span data-stu-id="f01b3-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="f01b3-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="f01b3-158">Request</span></span>
<span data-ttu-id="f01b3-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f01b3-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f01b3-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="f01b3-160">Response</span></span>
<span data-ttu-id="f01b3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f01b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




