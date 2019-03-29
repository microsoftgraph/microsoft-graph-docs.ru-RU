---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c54a7bba58e64fc9f74053cc40e43517bc65a881
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964698"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="10ec6-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="10ec6-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="10ec6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10ec6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10ec6-105">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10ec6-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10ec6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="10ec6-106">Prerequisites</span></span>
<span data-ttu-id="10ec6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10ec6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10ec6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10ec6-109">Permission type</span></span>|<span data-ttu-id="10ec6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10ec6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10ec6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10ec6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="10ec6-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10ec6-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10ec6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10ec6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10ec6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ec6-114">Not supported.</span></span>|
|<span data-ttu-id="10ec6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10ec6-115">Application</span></span>|<span data-ttu-id="10ec6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ec6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10ec6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10ec6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="10ec6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10ec6-118">Request headers</span></span>
|<span data-ttu-id="10ec6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10ec6-119">Header</span></span>|<span data-ttu-id="10ec6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="10ec6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10ec6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10ec6-121">Authorization</span></span>|<span data-ttu-id="10ec6-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10ec6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10ec6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="10ec6-123">Accept</span></span>|<span data-ttu-id="10ec6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="10ec6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10ec6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10ec6-125">Request body</span></span>
<span data-ttu-id="10ec6-126">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10ec6-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="10ec6-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10ec6-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="10ec6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="10ec6-128">Property</span></span>|<span data-ttu-id="10ec6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="10ec6-129">Type</span></span>|<span data-ttu-id="10ec6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="10ec6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10ec6-131">id</span><span class="sxs-lookup"><span data-stu-id="10ec6-131">id</span></span>|<span data-ttu-id="10ec6-132">Строка</span><span class="sxs-lookup"><span data-stu-id="10ec6-132">String</span></span>|<span data-ttu-id="10ec6-133">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10ec6-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10ec6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="10ec6-134">displayName</span></span>|<span data-ttu-id="10ec6-135">String</span><span class="sxs-lookup"><span data-stu-id="10ec6-135">String</span></span>|<span data-ttu-id="10ec6-136">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10ec6-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10ec6-137">description</span><span class="sxs-lookup"><span data-stu-id="10ec6-137">description</span></span>|<span data-ttu-id="10ec6-138">String</span><span class="sxs-lookup"><span data-stu-id="10ec6-138">String</span></span>|<span data-ttu-id="10ec6-139">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10ec6-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10ec6-140">priority</span><span class="sxs-lookup"><span data-stu-id="10ec6-140">priority</span></span>|<span data-ttu-id="10ec6-141">Int32</span><span class="sxs-lookup"><span data-stu-id="10ec6-141">Int32</span></span>|<span data-ttu-id="10ec6-142">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10ec6-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10ec6-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10ec6-143">createdDateTime</span></span>|<span data-ttu-id="10ec6-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10ec6-144">DateTimeOffset</span></span>|<span data-ttu-id="10ec6-145">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10ec6-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10ec6-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10ec6-146">lastModifiedDateTime</span></span>|<span data-ttu-id="10ec6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10ec6-147">DateTimeOffset</span></span>|<span data-ttu-id="10ec6-148">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10ec6-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10ec6-149">version</span><span class="sxs-lookup"><span data-stu-id="10ec6-149">version</span></span>|<span data-ttu-id="10ec6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="10ec6-150">Int32</span></span>|<span data-ttu-id="10ec6-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10ec6-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="10ec6-152">limit</span><span class="sxs-lookup"><span data-stu-id="10ec6-152">limit</span></span>|<span data-ttu-id="10ec6-153">Int32</span><span class="sxs-lookup"><span data-stu-id="10ec6-153">Int32</span></span>|<span data-ttu-id="10ec6-154">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="10ec6-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="10ec6-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ec6-155">Response</span></span>
<span data-ttu-id="10ec6-156">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="10ec6-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10ec6-157">Пример</span><span class="sxs-lookup"><span data-stu-id="10ec6-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="10ec6-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="10ec6-158">Request</span></span>
<span data-ttu-id="10ec6-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10ec6-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10ec6-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ec6-160">Response</span></span>
<span data-ttu-id="10ec6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10ec6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



