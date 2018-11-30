---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
ms.openlocfilehash: f8fe820d63a2e6a5b3393033c49139ad85a4eb06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026887"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="ccd5c-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="ccd5c-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="ccd5c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ccd5c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ccd5c-105">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd5c-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ccd5c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ccd5c-106">Prerequisites</span></span>
<span data-ttu-id="ccd5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccd5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccd5c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccd5c-109">Permission type</span></span>|<span data-ttu-id="ccd5c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccd5c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccd5c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccd5c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ccd5c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccd5c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ccd5c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccd5c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccd5c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd5c-114">Not supported.</span></span>|
|<span data-ttu-id="ccd5c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccd5c-115">Application</span></span>|<span data-ttu-id="ccd5c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd5c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccd5c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccd5c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ccd5c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccd5c-118">Request headers</span></span>
|<span data-ttu-id="ccd5c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccd5c-119">Header</span></span>|<span data-ttu-id="ccd5c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ccd5c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccd5c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccd5c-121">Authorization</span></span>|<span data-ttu-id="ccd5c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ccd5c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccd5c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ccd5c-123">Accept</span></span>|<span data-ttu-id="ccd5c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ccd5c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccd5c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccd5c-125">Request body</span></span>
<span data-ttu-id="ccd5c-126">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccd5c-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="ccd5c-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ccd5c-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="ccd5c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccd5c-128">Property</span></span>|<span data-ttu-id="ccd5c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ccd5c-129">Type</span></span>|<span data-ttu-id="ccd5c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ccd5c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccd5c-131">id</span><span class="sxs-lookup"><span data-stu-id="ccd5c-131">id</span></span>|<span data-ttu-id="ccd5c-132">String</span><span class="sxs-lookup"><span data-stu-id="ccd5c-132">String</span></span>|<span data-ttu-id="ccd5c-133">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd5c-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ccd5c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ccd5c-134">displayName</span></span>|<span data-ttu-id="ccd5c-135">String</span><span class="sxs-lookup"><span data-stu-id="ccd5c-135">String</span></span>|<span data-ttu-id="ccd5c-136">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd5c-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ccd5c-137">описание</span><span class="sxs-lookup"><span data-stu-id="ccd5c-137">description</span></span>|<span data-ttu-id="ccd5c-138">String</span><span class="sxs-lookup"><span data-stu-id="ccd5c-138">String</span></span>|<span data-ttu-id="ccd5c-139">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd5c-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ccd5c-140">priority</span><span class="sxs-lookup"><span data-stu-id="ccd5c-140">priority</span></span>|<span data-ttu-id="ccd5c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ccd5c-141">Int32</span></span>|<span data-ttu-id="ccd5c-142">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd5c-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ccd5c-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ccd5c-143">createdDateTime</span></span>|<span data-ttu-id="ccd5c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccd5c-144">DateTimeOffset</span></span>|<span data-ttu-id="ccd5c-145">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd5c-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ccd5c-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccd5c-146">lastModifiedDateTime</span></span>|<span data-ttu-id="ccd5c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccd5c-147">DateTimeOffset</span></span>|<span data-ttu-id="ccd5c-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd5c-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ccd5c-149">version</span><span class="sxs-lookup"><span data-stu-id="ccd5c-149">version</span></span>|<span data-ttu-id="ccd5c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ccd5c-150">Int32</span></span>|<span data-ttu-id="ccd5c-151">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd5c-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ccd5c-152">limit</span><span class="sxs-lookup"><span data-stu-id="ccd5c-152">limit</span></span>|<span data-ttu-id="ccd5c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ccd5c-153">Int32</span></span>|<span data-ttu-id="ccd5c-154">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ccd5c-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ccd5c-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccd5c-155">Response</span></span>
<span data-ttu-id="ccd5c-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ccd5c-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccd5c-157">Пример</span><span class="sxs-lookup"><span data-stu-id="ccd5c-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="ccd5c-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccd5c-158">Request</span></span>
<span data-ttu-id="ccd5c-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccd5c-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="ccd5c-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccd5c-160">Response</span></span>
<span data-ttu-id="ccd5c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ccd5c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



