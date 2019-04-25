---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c54a7bba58e64fc9f74053cc40e43517bc65a881
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582789"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="6e217-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e217-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="6e217-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e217-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e217-105">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e217-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e217-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6e217-106">Prerequisites</span></span>
<span data-ttu-id="6e217-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e217-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e217-109">Permission type</span></span>|<span data-ttu-id="6e217-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e217-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e217-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e217-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e217-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e217-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6e217-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e217-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e217-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e217-114">Not supported.</span></span>|
|<span data-ttu-id="6e217-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e217-115">Application</span></span>|<span data-ttu-id="6e217-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e217-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e217-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e217-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6e217-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e217-118">Request headers</span></span>
|<span data-ttu-id="6e217-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e217-119">Header</span></span>|<span data-ttu-id="6e217-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6e217-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e217-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e217-121">Authorization</span></span>|<span data-ttu-id="6e217-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e217-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e217-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6e217-123">Accept</span></span>|<span data-ttu-id="6e217-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6e217-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e217-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e217-125">Request body</span></span>
<span data-ttu-id="6e217-126">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e217-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="6e217-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e217-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="6e217-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e217-128">Property</span></span>|<span data-ttu-id="6e217-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6e217-129">Type</span></span>|<span data-ttu-id="6e217-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6e217-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e217-131">id</span><span class="sxs-lookup"><span data-stu-id="6e217-131">id</span></span>|<span data-ttu-id="6e217-132">Строка</span><span class="sxs-lookup"><span data-stu-id="6e217-132">String</span></span>|<span data-ttu-id="6e217-133">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e217-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e217-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6e217-134">displayName</span></span>|<span data-ttu-id="6e217-135">String</span><span class="sxs-lookup"><span data-stu-id="6e217-135">String</span></span>|<span data-ttu-id="6e217-136">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e217-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e217-137">description</span><span class="sxs-lookup"><span data-stu-id="6e217-137">description</span></span>|<span data-ttu-id="6e217-138">String</span><span class="sxs-lookup"><span data-stu-id="6e217-138">String</span></span>|<span data-ttu-id="6e217-139">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e217-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e217-140">priority</span><span class="sxs-lookup"><span data-stu-id="6e217-140">priority</span></span>|<span data-ttu-id="6e217-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6e217-141">Int32</span></span>|<span data-ttu-id="6e217-142">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e217-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e217-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e217-143">createdDateTime</span></span>|<span data-ttu-id="6e217-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e217-144">DateTimeOffset</span></span>|<span data-ttu-id="6e217-145">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e217-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e217-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e217-146">lastModifiedDateTime</span></span>|<span data-ttu-id="6e217-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e217-147">DateTimeOffset</span></span>|<span data-ttu-id="6e217-148">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e217-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e217-149">version</span><span class="sxs-lookup"><span data-stu-id="6e217-149">version</span></span>|<span data-ttu-id="6e217-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6e217-150">Int32</span></span>|<span data-ttu-id="6e217-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e217-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6e217-152">limit</span><span class="sxs-lookup"><span data-stu-id="6e217-152">limit</span></span>|<span data-ttu-id="6e217-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6e217-153">Int32</span></span>|<span data-ttu-id="6e217-154">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6e217-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6e217-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e217-155">Response</span></span>
<span data-ttu-id="6e217-156">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6e217-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e217-157">Пример</span><span class="sxs-lookup"><span data-stu-id="6e217-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e217-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e217-158">Request</span></span>
<span data-ttu-id="6e217-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e217-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6e217-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e217-160">Response</span></span>
<span data-ttu-id="6e217-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e217-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



