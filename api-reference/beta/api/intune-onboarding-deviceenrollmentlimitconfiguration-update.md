---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6446818b4f4b5e117b8278a1b0a74bb997dfcbd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170898"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="6032b-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="6032b-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="6032b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6032b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6032b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6032b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6032b-106">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6032b-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6032b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6032b-107">Prerequisites</span></span>
<span data-ttu-id="6032b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6032b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6032b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6032b-110">Permission type</span></span>|<span data-ttu-id="6032b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6032b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6032b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6032b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6032b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6032b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6032b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6032b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6032b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6032b-115">Not supported.</span></span>|
|<span data-ttu-id="6032b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6032b-116">Application</span></span>|<span data-ttu-id="6032b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6032b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6032b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6032b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6032b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6032b-119">Request headers</span></span>
|<span data-ttu-id="6032b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6032b-120">Header</span></span>|<span data-ttu-id="6032b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6032b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6032b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6032b-122">Authorization</span></span>|<span data-ttu-id="6032b-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6032b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6032b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6032b-124">Accept</span></span>|<span data-ttu-id="6032b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6032b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6032b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6032b-126">Request body</span></span>
<span data-ttu-id="6032b-127">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6032b-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="6032b-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6032b-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="6032b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6032b-129">Property</span></span>|<span data-ttu-id="6032b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6032b-130">Type</span></span>|<span data-ttu-id="6032b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6032b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6032b-132">id</span><span class="sxs-lookup"><span data-stu-id="6032b-132">id</span></span>|<span data-ttu-id="6032b-133">String</span><span class="sxs-lookup"><span data-stu-id="6032b-133">String</span></span>|<span data-ttu-id="6032b-134">Идентификатор конфигурации страницы состояния регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6032b-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6032b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6032b-135">displayName</span></span>|<span data-ttu-id="6032b-136">String</span><span class="sxs-lookup"><span data-stu-id="6032b-136">String</span></span>|<span data-ttu-id="6032b-137">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6032b-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6032b-138">description</span><span class="sxs-lookup"><span data-stu-id="6032b-138">description</span></span>|<span data-ttu-id="6032b-139">String</span><span class="sxs-lookup"><span data-stu-id="6032b-139">String</span></span>|<span data-ttu-id="6032b-140">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6032b-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6032b-141">priority</span><span class="sxs-lookup"><span data-stu-id="6032b-141">priority</span></span>|<span data-ttu-id="6032b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6032b-142">Int32</span></span>|<span data-ttu-id="6032b-143">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6032b-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6032b-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6032b-144">createdDateTime</span></span>|<span data-ttu-id="6032b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6032b-145">DateTimeOffset</span></span>|<span data-ttu-id="6032b-146">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6032b-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6032b-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6032b-147">lastModifiedDateTime</span></span>|<span data-ttu-id="6032b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6032b-148">DateTimeOffset</span></span>|<span data-ttu-id="6032b-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6032b-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6032b-150">version</span><span class="sxs-lookup"><span data-stu-id="6032b-150">version</span></span>|<span data-ttu-id="6032b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6032b-151">Int32</span></span>|<span data-ttu-id="6032b-152">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6032b-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6032b-153">limit</span><span class="sxs-lookup"><span data-stu-id="6032b-153">limit</span></span>|<span data-ttu-id="6032b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6032b-154">Int32</span></span>|<span data-ttu-id="6032b-155">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6032b-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6032b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="6032b-156">Response</span></span>
<span data-ttu-id="6032b-157">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6032b-157">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6032b-158">Пример</span><span class="sxs-lookup"><span data-stu-id="6032b-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="6032b-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="6032b-159">Request</span></span>
<span data-ttu-id="6032b-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6032b-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="6032b-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="6032b-161">Response</span></span>
<span data-ttu-id="6032b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6032b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




