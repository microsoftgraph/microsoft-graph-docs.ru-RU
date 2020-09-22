---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e4ab07894288c65839c6f11474180fcb24276a70
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075256"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="d1901-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1901-103">Create deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="d1901-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1901-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1901-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1901-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1901-106">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1901-106">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1901-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d1901-107">Prerequisites</span></span>
<span data-ttu-id="d1901-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1901-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1901-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1901-110">Permission type</span></span>|<span data-ttu-id="d1901-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1901-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1901-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1901-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1901-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1901-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d1901-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1901-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1901-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1901-115">Not supported.</span></span>|
|<span data-ttu-id="d1901-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1901-116">Application</span></span>|<span data-ttu-id="d1901-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1901-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1901-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1901-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d1901-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d1901-119">Request headers</span></span>
|<span data-ttu-id="d1901-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1901-120">Header</span></span>|<span data-ttu-id="d1901-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d1901-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1901-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1901-122">Authorization</span></span>|<span data-ttu-id="d1901-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1901-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1901-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d1901-124">Accept</span></span>|<span data-ttu-id="d1901-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1901-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1901-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1901-126">Request body</span></span>
<span data-ttu-id="d1901-127">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1901-127">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="d1901-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d1901-128">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="d1901-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1901-129">Property</span></span>|<span data-ttu-id="d1901-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d1901-130">Type</span></span>|<span data-ttu-id="d1901-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d1901-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1901-132">id</span><span class="sxs-lookup"><span data-stu-id="d1901-132">id</span></span>|<span data-ttu-id="d1901-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d1901-133">String</span></span>|<span data-ttu-id="d1901-134">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1901-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1901-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d1901-135">displayName</span></span>|<span data-ttu-id="d1901-136">Строка</span><span class="sxs-lookup"><span data-stu-id="d1901-136">String</span></span>|<span data-ttu-id="d1901-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1901-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1901-138">description</span><span class="sxs-lookup"><span data-stu-id="d1901-138">description</span></span>|<span data-ttu-id="d1901-139">Строка</span><span class="sxs-lookup"><span data-stu-id="d1901-139">String</span></span>|<span data-ttu-id="d1901-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1901-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1901-141">priority</span><span class="sxs-lookup"><span data-stu-id="d1901-141">priority</span></span>|<span data-ttu-id="d1901-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d1901-142">Int32</span></span>|<span data-ttu-id="d1901-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1901-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1901-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1901-144">createdDateTime</span></span>|<span data-ttu-id="d1901-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1901-145">DateTimeOffset</span></span>|<span data-ttu-id="d1901-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1901-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1901-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1901-147">lastModifiedDateTime</span></span>|<span data-ttu-id="d1901-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1901-148">DateTimeOffset</span></span>|<span data-ttu-id="d1901-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1901-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1901-150">version</span><span class="sxs-lookup"><span data-stu-id="d1901-150">version</span></span>|<span data-ttu-id="d1901-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d1901-151">Int32</span></span>|<span data-ttu-id="d1901-152">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1901-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1901-153">limit</span><span class="sxs-lookup"><span data-stu-id="d1901-153">limit</span></span>|<span data-ttu-id="d1901-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d1901-154">Int32</span></span>|<span data-ttu-id="d1901-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d1901-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d1901-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1901-156">Response</span></span>
<span data-ttu-id="d1901-157">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1901-157">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1901-158">Пример</span><span class="sxs-lookup"><span data-stu-id="d1901-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1901-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1901-159">Request</span></span>
<span data-ttu-id="d1901-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1901-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1901-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1901-161">Response</span></span>
<span data-ttu-id="d1901-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1901-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









