---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26c0040163b81f109a571984ead53600884fdff2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362704"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="6cd51-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="6cd51-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="6cd51-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6cd51-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cd51-105">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cd51-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cd51-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6cd51-106">Prerequisites</span></span>
<span data-ttu-id="6cd51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cd51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cd51-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cd51-109">Permission type</span></span>|<span data-ttu-id="6cd51-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cd51-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cd51-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cd51-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6cd51-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd51-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6cd51-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cd51-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cd51-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cd51-114">Not supported.</span></span>|
|<span data-ttu-id="6cd51-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cd51-115">Application</span></span>|<span data-ttu-id="6cd51-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cd51-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cd51-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cd51-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6cd51-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cd51-118">Request headers</span></span>
|<span data-ttu-id="6cd51-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6cd51-119">Header</span></span>|<span data-ttu-id="6cd51-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6cd51-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cd51-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6cd51-121">Authorization</span></span>|<span data-ttu-id="6cd51-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cd51-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cd51-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6cd51-123">Accept</span></span>|<span data-ttu-id="6cd51-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6cd51-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cd51-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cd51-125">Request body</span></span>
<span data-ttu-id="6cd51-126">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cd51-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="6cd51-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6cd51-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="6cd51-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cd51-128">Property</span></span>|<span data-ttu-id="6cd51-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6cd51-129">Type</span></span>|<span data-ttu-id="6cd51-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6cd51-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cd51-131">id</span><span class="sxs-lookup"><span data-stu-id="6cd51-131">id</span></span>|<span data-ttu-id="6cd51-132">String</span><span class="sxs-lookup"><span data-stu-id="6cd51-132">String</span></span>|<span data-ttu-id="6cd51-133">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cd51-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6cd51-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6cd51-134">displayName</span></span>|<span data-ttu-id="6cd51-135">Строка</span><span class="sxs-lookup"><span data-stu-id="6cd51-135">String</span></span>|<span data-ttu-id="6cd51-136">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cd51-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6cd51-137">description</span><span class="sxs-lookup"><span data-stu-id="6cd51-137">description</span></span>|<span data-ttu-id="6cd51-138">String</span><span class="sxs-lookup"><span data-stu-id="6cd51-138">String</span></span>|<span data-ttu-id="6cd51-139">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cd51-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6cd51-140">priority</span><span class="sxs-lookup"><span data-stu-id="6cd51-140">priority</span></span>|<span data-ttu-id="6cd51-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6cd51-141">Int32</span></span>|<span data-ttu-id="6cd51-142">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cd51-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6cd51-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cd51-143">createdDateTime</span></span>|<span data-ttu-id="6cd51-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cd51-144">DateTimeOffset</span></span>|<span data-ttu-id="6cd51-145">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cd51-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6cd51-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cd51-146">lastModifiedDateTime</span></span>|<span data-ttu-id="6cd51-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cd51-147">DateTimeOffset</span></span>|<span data-ttu-id="6cd51-148">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cd51-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6cd51-149">version</span><span class="sxs-lookup"><span data-stu-id="6cd51-149">version</span></span>|<span data-ttu-id="6cd51-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6cd51-150">Int32</span></span>|<span data-ttu-id="6cd51-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cd51-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6cd51-152">limit</span><span class="sxs-lookup"><span data-stu-id="6cd51-152">limit</span></span>|<span data-ttu-id="6cd51-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6cd51-153">Int32</span></span>|<span data-ttu-id="6cd51-154">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6cd51-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6cd51-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cd51-155">Response</span></span>
<span data-ttu-id="6cd51-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6cd51-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cd51-157">Пример</span><span class="sxs-lookup"><span data-stu-id="6cd51-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cd51-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cd51-158">Request</span></span>
<span data-ttu-id="6cd51-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cd51-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6cd51-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cd51-160">Response</span></span>
<span data-ttu-id="6cd51-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cd51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




