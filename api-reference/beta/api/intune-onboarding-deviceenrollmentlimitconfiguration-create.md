---
title: Создание объекта deviceEnrollmentLimitConfiguration
description: Создание объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95431986b1b8a47c723f493295b64989bb3db3d5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165354"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="2fd80-103">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="2fd80-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="2fd80-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fd80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fd80-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2fd80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fd80-106">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fd80-106">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fd80-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2fd80-107">Prerequisites</span></span>
<span data-ttu-id="2fd80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2fd80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2fd80-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fd80-110">Permission type</span></span>|<span data-ttu-id="2fd80-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fd80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fd80-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fd80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2fd80-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fd80-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2fd80-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fd80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fd80-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fd80-115">Not supported.</span></span>|
|<span data-ttu-id="2fd80-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2fd80-116">Application</span></span>|<span data-ttu-id="2fd80-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fd80-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fd80-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fd80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2fd80-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2fd80-119">Request headers</span></span>
|<span data-ttu-id="2fd80-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2fd80-120">Header</span></span>|<span data-ttu-id="2fd80-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2fd80-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fd80-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2fd80-122">Authorization</span></span>|<span data-ttu-id="2fd80-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2fd80-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fd80-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2fd80-124">Accept</span></span>|<span data-ttu-id="2fd80-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2fd80-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fd80-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2fd80-126">Request body</span></span>
<span data-ttu-id="2fd80-127">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fd80-127">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="2fd80-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2fd80-128">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="2fd80-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fd80-129">Property</span></span>|<span data-ttu-id="2fd80-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2fd80-130">Type</span></span>|<span data-ttu-id="2fd80-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2fd80-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fd80-132">id</span><span class="sxs-lookup"><span data-stu-id="2fd80-132">id</span></span>|<span data-ttu-id="2fd80-133">String</span><span class="sxs-lookup"><span data-stu-id="2fd80-133">String</span></span>|<span data-ttu-id="2fd80-134">Идентификатор конфигурации страницы состояния регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fd80-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fd80-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2fd80-135">displayName</span></span>|<span data-ttu-id="2fd80-136">String</span><span class="sxs-lookup"><span data-stu-id="2fd80-136">String</span></span>|<span data-ttu-id="2fd80-137">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fd80-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fd80-138">description</span><span class="sxs-lookup"><span data-stu-id="2fd80-138">description</span></span>|<span data-ttu-id="2fd80-139">String</span><span class="sxs-lookup"><span data-stu-id="2fd80-139">String</span></span>|<span data-ttu-id="2fd80-140">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fd80-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fd80-141">priority</span><span class="sxs-lookup"><span data-stu-id="2fd80-141">priority</span></span>|<span data-ttu-id="2fd80-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2fd80-142">Int32</span></span>|<span data-ttu-id="2fd80-143">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fd80-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fd80-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fd80-144">createdDateTime</span></span>|<span data-ttu-id="2fd80-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fd80-145">DateTimeOffset</span></span>|<span data-ttu-id="2fd80-146">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fd80-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fd80-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fd80-147">lastModifiedDateTime</span></span>|<span data-ttu-id="2fd80-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fd80-148">DateTimeOffset</span></span>|<span data-ttu-id="2fd80-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fd80-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fd80-150">version</span><span class="sxs-lookup"><span data-stu-id="2fd80-150">version</span></span>|<span data-ttu-id="2fd80-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2fd80-151">Int32</span></span>|<span data-ttu-id="2fd80-152">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fd80-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2fd80-153">limit</span><span class="sxs-lookup"><span data-stu-id="2fd80-153">limit</span></span>|<span data-ttu-id="2fd80-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2fd80-154">Int32</span></span>|<span data-ttu-id="2fd80-155">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2fd80-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2fd80-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fd80-156">Response</span></span>
<span data-ttu-id="2fd80-157">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2fd80-157">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fd80-158">Пример</span><span class="sxs-lookup"><span data-stu-id="2fd80-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fd80-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fd80-159">Request</span></span>
<span data-ttu-id="2fd80-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fd80-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2fd80-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="2fd80-161">Response</span></span>
<span data-ttu-id="2fd80-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2fd80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




