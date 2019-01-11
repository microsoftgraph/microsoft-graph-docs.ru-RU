---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bd4b1c581260a7cd1438ddad6bc2e486af1ac679
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832893"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="546a8-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="546a8-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="546a8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="546a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="546a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="546a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="546a8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="546a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="546a8-107">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="546a8-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="546a8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="546a8-108">Prerequisites</span></span>
<span data-ttu-id="546a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="546a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="546a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="546a8-111">Permission type</span></span>|<span data-ttu-id="546a8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="546a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="546a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="546a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="546a8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="546a8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="546a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="546a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="546a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="546a8-116">Not supported.</span></span>|
|<span data-ttu-id="546a8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="546a8-117">Application</span></span>|<span data-ttu-id="546a8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="546a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="546a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="546a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="546a8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="546a8-120">Request headers</span></span>
|<span data-ttu-id="546a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="546a8-121">Header</span></span>|<span data-ttu-id="546a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="546a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="546a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="546a8-123">Authorization</span></span>|<span data-ttu-id="546a8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="546a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="546a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="546a8-125">Accept</span></span>|<span data-ttu-id="546a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="546a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="546a8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="546a8-127">Request body</span></span>
<span data-ttu-id="546a8-128">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="546a8-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="546a8-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="546a8-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="546a8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="546a8-130">Property</span></span>|<span data-ttu-id="546a8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="546a8-131">Type</span></span>|<span data-ttu-id="546a8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="546a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="546a8-133">id</span><span class="sxs-lookup"><span data-stu-id="546a8-133">id</span></span>|<span data-ttu-id="546a8-134">String</span><span class="sxs-lookup"><span data-stu-id="546a8-134">String</span></span>|<span data-ttu-id="546a8-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="546a8-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="546a8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="546a8-136">displayName</span></span>|<span data-ttu-id="546a8-137">String</span><span class="sxs-lookup"><span data-stu-id="546a8-137">String</span></span>|<span data-ttu-id="546a8-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="546a8-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="546a8-139">описание</span><span class="sxs-lookup"><span data-stu-id="546a8-139">description</span></span>|<span data-ttu-id="546a8-140">String</span><span class="sxs-lookup"><span data-stu-id="546a8-140">String</span></span>|<span data-ttu-id="546a8-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="546a8-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="546a8-142">priority</span><span class="sxs-lookup"><span data-stu-id="546a8-142">priority</span></span>|<span data-ttu-id="546a8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="546a8-143">Int32</span></span>|<span data-ttu-id="546a8-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="546a8-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="546a8-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="546a8-145">createdDateTime</span></span>|<span data-ttu-id="546a8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="546a8-146">DateTimeOffset</span></span>|<span data-ttu-id="546a8-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="546a8-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="546a8-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="546a8-148">lastModifiedDateTime</span></span>|<span data-ttu-id="546a8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="546a8-149">DateTimeOffset</span></span>|<span data-ttu-id="546a8-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="546a8-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="546a8-151">version</span><span class="sxs-lookup"><span data-stu-id="546a8-151">version</span></span>|<span data-ttu-id="546a8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="546a8-152">Int32</span></span>|<span data-ttu-id="546a8-153">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="546a8-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="546a8-154">limit</span><span class="sxs-lookup"><span data-stu-id="546a8-154">limit</span></span>|<span data-ttu-id="546a8-155">Int32</span><span class="sxs-lookup"><span data-stu-id="546a8-155">Int32</span></span>|<span data-ttu-id="546a8-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="546a8-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="546a8-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="546a8-157">Response</span></span>
<span data-ttu-id="546a8-158">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="546a8-158">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="546a8-159">Пример</span><span class="sxs-lookup"><span data-stu-id="546a8-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="546a8-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="546a8-160">Request</span></span>
<span data-ttu-id="546a8-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="546a8-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 196

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="546a8-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="546a8-162">Response</span></span>
<span data-ttu-id="546a8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="546a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





