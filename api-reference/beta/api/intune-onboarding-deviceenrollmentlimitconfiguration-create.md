---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc7ab67dc44eec17a6e7a516967d3f3b0bc644ae
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401133"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="059f5-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="059f5-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="059f5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="059f5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="059f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="059f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="059f5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="059f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="059f5-107">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="059f5-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="059f5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="059f5-108">Prerequisites</span></span>
<span data-ttu-id="059f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="059f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="059f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="059f5-111">Permission type</span></span>|<span data-ttu-id="059f5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="059f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="059f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="059f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="059f5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="059f5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="059f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="059f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="059f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="059f5-116">Not supported.</span></span>|
|<span data-ttu-id="059f5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="059f5-117">Application</span></span>|<span data-ttu-id="059f5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="059f5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="059f5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="059f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="059f5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="059f5-120">Request headers</span></span>
|<span data-ttu-id="059f5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="059f5-121">Header</span></span>|<span data-ttu-id="059f5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="059f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="059f5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="059f5-123">Authorization</span></span>|<span data-ttu-id="059f5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="059f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="059f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="059f5-125">Accept</span></span>|<span data-ttu-id="059f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="059f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="059f5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="059f5-127">Request body</span></span>
<span data-ttu-id="059f5-128">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="059f5-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="059f5-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="059f5-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="059f5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="059f5-130">Property</span></span>|<span data-ttu-id="059f5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="059f5-131">Type</span></span>|<span data-ttu-id="059f5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="059f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="059f5-133">id</span><span class="sxs-lookup"><span data-stu-id="059f5-133">id</span></span>|<span data-ttu-id="059f5-134">String</span><span class="sxs-lookup"><span data-stu-id="059f5-134">String</span></span>|<span data-ttu-id="059f5-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="059f5-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="059f5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="059f5-136">displayName</span></span>|<span data-ttu-id="059f5-137">String</span><span class="sxs-lookup"><span data-stu-id="059f5-137">String</span></span>|<span data-ttu-id="059f5-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="059f5-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="059f5-139">description</span><span class="sxs-lookup"><span data-stu-id="059f5-139">description</span></span>|<span data-ttu-id="059f5-140">String</span><span class="sxs-lookup"><span data-stu-id="059f5-140">String</span></span>|<span data-ttu-id="059f5-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="059f5-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="059f5-142">priority</span><span class="sxs-lookup"><span data-stu-id="059f5-142">priority</span></span>|<span data-ttu-id="059f5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="059f5-143">Int32</span></span>|<span data-ttu-id="059f5-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="059f5-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="059f5-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="059f5-145">createdDateTime</span></span>|<span data-ttu-id="059f5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="059f5-146">DateTimeOffset</span></span>|<span data-ttu-id="059f5-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="059f5-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="059f5-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="059f5-148">lastModifiedDateTime</span></span>|<span data-ttu-id="059f5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="059f5-149">DateTimeOffset</span></span>|<span data-ttu-id="059f5-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="059f5-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="059f5-151">version</span><span class="sxs-lookup"><span data-stu-id="059f5-151">version</span></span>|<span data-ttu-id="059f5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="059f5-152">Int32</span></span>|<span data-ttu-id="059f5-153">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="059f5-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="059f5-154">limit</span><span class="sxs-lookup"><span data-stu-id="059f5-154">limit</span></span>|<span data-ttu-id="059f5-155">Int32</span><span class="sxs-lookup"><span data-stu-id="059f5-155">Int32</span></span>|<span data-ttu-id="059f5-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="059f5-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="059f5-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="059f5-157">Response</span></span>
<span data-ttu-id="059f5-158">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="059f5-158">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="059f5-159">Пример</span><span class="sxs-lookup"><span data-stu-id="059f5-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="059f5-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="059f5-160">Request</span></span>
<span data-ttu-id="059f5-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="059f5-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="059f5-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="059f5-162">Response</span></span>
<span data-ttu-id="059f5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="059f5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




