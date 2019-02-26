---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 842c9d6c1cf6e805850317bb804cb8905c189134
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254179"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="c6edd-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="c6edd-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="c6edd-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6edd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6edd-105">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6edd-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6edd-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c6edd-106">Prerequisites</span></span>
<span data-ttu-id="c6edd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c6edd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c6edd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6edd-109">Permission type</span></span>|<span data-ttu-id="c6edd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6edd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6edd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6edd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c6edd-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6edd-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c6edd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6edd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6edd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6edd-114">Not supported.</span></span>|
|<span data-ttu-id="c6edd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6edd-115">Application</span></span>|<span data-ttu-id="c6edd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6edd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6edd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6edd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c6edd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6edd-118">Request headers</span></span>
|<span data-ttu-id="c6edd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6edd-119">Header</span></span>|<span data-ttu-id="c6edd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c6edd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6edd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6edd-121">Authorization</span></span>|<span data-ttu-id="c6edd-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c6edd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6edd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c6edd-123">Accept</span></span>|<span data-ttu-id="c6edd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c6edd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6edd-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c6edd-125">Request body</span></span>
<span data-ttu-id="c6edd-126">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6edd-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="c6edd-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6edd-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="c6edd-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6edd-128">Property</span></span>|<span data-ttu-id="c6edd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c6edd-129">Type</span></span>|<span data-ttu-id="c6edd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c6edd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6edd-131">id</span><span class="sxs-lookup"><span data-stu-id="c6edd-131">id</span></span>|<span data-ttu-id="c6edd-132">String</span><span class="sxs-lookup"><span data-stu-id="c6edd-132">String</span></span>|<span data-ttu-id="c6edd-133">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6edd-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c6edd-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c6edd-134">displayName</span></span>|<span data-ttu-id="c6edd-135">String</span><span class="sxs-lookup"><span data-stu-id="c6edd-135">String</span></span>|<span data-ttu-id="c6edd-136">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6edd-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c6edd-137">description</span><span class="sxs-lookup"><span data-stu-id="c6edd-137">description</span></span>|<span data-ttu-id="c6edd-138">String</span><span class="sxs-lookup"><span data-stu-id="c6edd-138">String</span></span>|<span data-ttu-id="c6edd-139">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6edd-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c6edd-140">priority</span><span class="sxs-lookup"><span data-stu-id="c6edd-140">priority</span></span>|<span data-ttu-id="c6edd-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c6edd-141">Int32</span></span>|<span data-ttu-id="c6edd-142">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6edd-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c6edd-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6edd-143">createdDateTime</span></span>|<span data-ttu-id="c6edd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6edd-144">DateTimeOffset</span></span>|<span data-ttu-id="c6edd-145">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6edd-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c6edd-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6edd-146">lastModifiedDateTime</span></span>|<span data-ttu-id="c6edd-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6edd-147">DateTimeOffset</span></span>|<span data-ttu-id="c6edd-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6edd-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c6edd-149">version</span><span class="sxs-lookup"><span data-stu-id="c6edd-149">version</span></span>|<span data-ttu-id="c6edd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c6edd-150">Int32</span></span>|<span data-ttu-id="c6edd-151">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6edd-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c6edd-152">limit</span><span class="sxs-lookup"><span data-stu-id="c6edd-152">limit</span></span>|<span data-ttu-id="c6edd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c6edd-153">Int32</span></span>|<span data-ttu-id="c6edd-154">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c6edd-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c6edd-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6edd-155">Response</span></span>
<span data-ttu-id="c6edd-156">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c6edd-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6edd-157">Пример</span><span class="sxs-lookup"><span data-stu-id="c6edd-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6edd-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6edd-158">Request</span></span>
<span data-ttu-id="c6edd-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6edd-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c6edd-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6edd-160">Response</span></span>
<span data-ttu-id="c6edd-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c6edd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



