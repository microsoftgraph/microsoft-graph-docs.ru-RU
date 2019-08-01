---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c202ba50223fc09284c775714a0aa448f8fb2210
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018010"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="b044f-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="b044f-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="b044f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b044f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b044f-105">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b044f-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b044f-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b044f-106">Prerequisites</span></span>
<span data-ttu-id="b044f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b044f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b044f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b044f-109">Permission type</span></span>|<span data-ttu-id="b044f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b044f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b044f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b044f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b044f-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b044f-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b044f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b044f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b044f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b044f-114">Not supported.</span></span>|
|<span data-ttu-id="b044f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b044f-115">Application</span></span>|<span data-ttu-id="b044f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b044f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b044f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b044f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b044f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b044f-118">Request headers</span></span>
|<span data-ttu-id="b044f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b044f-119">Header</span></span>|<span data-ttu-id="b044f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b044f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b044f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b044f-121">Authorization</span></span>|<span data-ttu-id="b044f-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b044f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b044f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b044f-123">Accept</span></span>|<span data-ttu-id="b044f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b044f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b044f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b044f-125">Request body</span></span>
<span data-ttu-id="b044f-126">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b044f-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="b044f-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b044f-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="b044f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b044f-128">Property</span></span>|<span data-ttu-id="b044f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b044f-129">Type</span></span>|<span data-ttu-id="b044f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b044f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b044f-131">id</span><span class="sxs-lookup"><span data-stu-id="b044f-131">id</span></span>|<span data-ttu-id="b044f-132">String</span><span class="sxs-lookup"><span data-stu-id="b044f-132">String</span></span>|<span data-ttu-id="b044f-133">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b044f-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b044f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b044f-134">displayName</span></span>|<span data-ttu-id="b044f-135">Строка</span><span class="sxs-lookup"><span data-stu-id="b044f-135">String</span></span>|<span data-ttu-id="b044f-136">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b044f-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b044f-137">description</span><span class="sxs-lookup"><span data-stu-id="b044f-137">description</span></span>|<span data-ttu-id="b044f-138">String</span><span class="sxs-lookup"><span data-stu-id="b044f-138">String</span></span>|<span data-ttu-id="b044f-139">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b044f-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b044f-140">priority</span><span class="sxs-lookup"><span data-stu-id="b044f-140">priority</span></span>|<span data-ttu-id="b044f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b044f-141">Int32</span></span>|<span data-ttu-id="b044f-142">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b044f-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b044f-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b044f-143">createdDateTime</span></span>|<span data-ttu-id="b044f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b044f-144">DateTimeOffset</span></span>|<span data-ttu-id="b044f-145">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b044f-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b044f-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b044f-146">lastModifiedDateTime</span></span>|<span data-ttu-id="b044f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b044f-147">DateTimeOffset</span></span>|<span data-ttu-id="b044f-148">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b044f-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b044f-149">version</span><span class="sxs-lookup"><span data-stu-id="b044f-149">version</span></span>|<span data-ttu-id="b044f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b044f-150">Int32</span></span>|<span data-ttu-id="b044f-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b044f-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b044f-152">limit</span><span class="sxs-lookup"><span data-stu-id="b044f-152">limit</span></span>|<span data-ttu-id="b044f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b044f-153">Int32</span></span>|<span data-ttu-id="b044f-154">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b044f-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b044f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="b044f-155">Response</span></span>
<span data-ttu-id="b044f-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b044f-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b044f-157">Пример</span><span class="sxs-lookup"><span data-stu-id="b044f-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="b044f-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="b044f-158">Request</span></span>
<span data-ttu-id="b044f-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b044f-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b044f-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="b044f-160">Response</span></span>
<span data-ttu-id="b044f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b044f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



