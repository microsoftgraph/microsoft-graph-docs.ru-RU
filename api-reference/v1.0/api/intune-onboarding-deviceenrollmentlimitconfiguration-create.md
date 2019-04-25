---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a331e49ea65450012d5f632b88579044382c9a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567370"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="598b2-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="598b2-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="598b2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="598b2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="598b2-105">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="598b2-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="598b2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="598b2-106">Prerequisites</span></span>
<span data-ttu-id="598b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="598b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="598b2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="598b2-109">Permission type</span></span>|<span data-ttu-id="598b2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="598b2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="598b2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="598b2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="598b2-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="598b2-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="598b2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="598b2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="598b2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="598b2-114">Not supported.</span></span>|
|<span data-ttu-id="598b2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="598b2-115">Application</span></span>|<span data-ttu-id="598b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="598b2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="598b2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="598b2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="598b2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="598b2-118">Request headers</span></span>
|<span data-ttu-id="598b2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="598b2-119">Header</span></span>|<span data-ttu-id="598b2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="598b2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="598b2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="598b2-121">Authorization</span></span>|<span data-ttu-id="598b2-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="598b2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="598b2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="598b2-123">Accept</span></span>|<span data-ttu-id="598b2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="598b2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="598b2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="598b2-125">Request body</span></span>
<span data-ttu-id="598b2-126">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="598b2-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="598b2-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="598b2-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="598b2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="598b2-128">Property</span></span>|<span data-ttu-id="598b2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="598b2-129">Type</span></span>|<span data-ttu-id="598b2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="598b2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="598b2-131">id</span><span class="sxs-lookup"><span data-stu-id="598b2-131">id</span></span>|<span data-ttu-id="598b2-132">Строка</span><span class="sxs-lookup"><span data-stu-id="598b2-132">String</span></span>|<span data-ttu-id="598b2-133">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="598b2-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="598b2-134">displayName</span><span class="sxs-lookup"><span data-stu-id="598b2-134">displayName</span></span>|<span data-ttu-id="598b2-135">String</span><span class="sxs-lookup"><span data-stu-id="598b2-135">String</span></span>|<span data-ttu-id="598b2-136">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="598b2-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="598b2-137">description</span><span class="sxs-lookup"><span data-stu-id="598b2-137">description</span></span>|<span data-ttu-id="598b2-138">String</span><span class="sxs-lookup"><span data-stu-id="598b2-138">String</span></span>|<span data-ttu-id="598b2-139">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="598b2-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="598b2-140">priority</span><span class="sxs-lookup"><span data-stu-id="598b2-140">priority</span></span>|<span data-ttu-id="598b2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="598b2-141">Int32</span></span>|<span data-ttu-id="598b2-142">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="598b2-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="598b2-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="598b2-143">createdDateTime</span></span>|<span data-ttu-id="598b2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="598b2-144">DateTimeOffset</span></span>|<span data-ttu-id="598b2-145">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="598b2-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="598b2-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="598b2-146">lastModifiedDateTime</span></span>|<span data-ttu-id="598b2-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="598b2-147">DateTimeOffset</span></span>|<span data-ttu-id="598b2-148">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="598b2-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="598b2-149">version</span><span class="sxs-lookup"><span data-stu-id="598b2-149">version</span></span>|<span data-ttu-id="598b2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="598b2-150">Int32</span></span>|<span data-ttu-id="598b2-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="598b2-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="598b2-152">limit</span><span class="sxs-lookup"><span data-stu-id="598b2-152">limit</span></span>|<span data-ttu-id="598b2-153">Int32</span><span class="sxs-lookup"><span data-stu-id="598b2-153">Int32</span></span>|<span data-ttu-id="598b2-154">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="598b2-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="598b2-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="598b2-155">Response</span></span>
<span data-ttu-id="598b2-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="598b2-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="598b2-157">Пример</span><span class="sxs-lookup"><span data-stu-id="598b2-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="598b2-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="598b2-158">Request</span></span>
<span data-ttu-id="598b2-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="598b2-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="598b2-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="598b2-160">Response</span></span>
<span data-ttu-id="598b2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="598b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



