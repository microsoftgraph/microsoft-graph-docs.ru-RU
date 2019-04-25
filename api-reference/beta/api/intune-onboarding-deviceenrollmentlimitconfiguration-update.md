---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 775eba06cce66394f448f305d10f80ca9ec16822
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32529291"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="16f04-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="16f04-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="16f04-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16f04-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16f04-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16f04-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16f04-106">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16f04-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16f04-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="16f04-107">Prerequisites</span></span>
<span data-ttu-id="16f04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16f04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16f04-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16f04-110">Permission type</span></span>|<span data-ttu-id="16f04-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16f04-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16f04-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16f04-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16f04-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16f04-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="16f04-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16f04-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16f04-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16f04-115">Not supported.</span></span>|
|<span data-ttu-id="16f04-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16f04-116">Application</span></span>|<span data-ttu-id="16f04-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16f04-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16f04-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16f04-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="16f04-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16f04-119">Request headers</span></span>
|<span data-ttu-id="16f04-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16f04-120">Header</span></span>|<span data-ttu-id="16f04-121">Значение</span><span class="sxs-lookup"><span data-stu-id="16f04-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16f04-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16f04-122">Authorization</span></span>|<span data-ttu-id="16f04-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16f04-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16f04-124">Accept</span><span class="sxs-lookup"><span data-stu-id="16f04-124">Accept</span></span>|<span data-ttu-id="16f04-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16f04-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16f04-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16f04-126">Request body</span></span>
<span data-ttu-id="16f04-127">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16f04-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="16f04-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16f04-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="16f04-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="16f04-129">Property</span></span>|<span data-ttu-id="16f04-130">Тип</span><span class="sxs-lookup"><span data-stu-id="16f04-130">Type</span></span>|<span data-ttu-id="16f04-131">Описание</span><span class="sxs-lookup"><span data-stu-id="16f04-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16f04-132">id</span><span class="sxs-lookup"><span data-stu-id="16f04-132">id</span></span>|<span data-ttu-id="16f04-133">Строка</span><span class="sxs-lookup"><span data-stu-id="16f04-133">String</span></span>|<span data-ttu-id="16f04-134">Идентификатор конфигурации страницы состояния регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f04-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="16f04-135">displayName</span><span class="sxs-lookup"><span data-stu-id="16f04-135">displayName</span></span>|<span data-ttu-id="16f04-136">String</span><span class="sxs-lookup"><span data-stu-id="16f04-136">String</span></span>|<span data-ttu-id="16f04-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f04-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="16f04-138">description</span><span class="sxs-lookup"><span data-stu-id="16f04-138">description</span></span>|<span data-ttu-id="16f04-139">String</span><span class="sxs-lookup"><span data-stu-id="16f04-139">String</span></span>|<span data-ttu-id="16f04-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f04-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="16f04-141">priority</span><span class="sxs-lookup"><span data-stu-id="16f04-141">priority</span></span>|<span data-ttu-id="16f04-142">Int32</span><span class="sxs-lookup"><span data-stu-id="16f04-142">Int32</span></span>|<span data-ttu-id="16f04-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f04-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="16f04-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16f04-144">createdDateTime</span></span>|<span data-ttu-id="16f04-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16f04-145">DateTimeOffset</span></span>|<span data-ttu-id="16f04-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f04-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="16f04-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16f04-147">lastModifiedDateTime</span></span>|<span data-ttu-id="16f04-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16f04-148">DateTimeOffset</span></span>|<span data-ttu-id="16f04-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f04-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="16f04-150">version</span><span class="sxs-lookup"><span data-stu-id="16f04-150">version</span></span>|<span data-ttu-id="16f04-151">Int32</span><span class="sxs-lookup"><span data-stu-id="16f04-151">Int32</span></span>|<span data-ttu-id="16f04-152">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16f04-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="16f04-153">limit</span><span class="sxs-lookup"><span data-stu-id="16f04-153">limit</span></span>|<span data-ttu-id="16f04-154">Int32</span><span class="sxs-lookup"><span data-stu-id="16f04-154">Int32</span></span>|<span data-ttu-id="16f04-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="16f04-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="16f04-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="16f04-156">Response</span></span>
<span data-ttu-id="16f04-157">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="16f04-157">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16f04-158">Пример</span><span class="sxs-lookup"><span data-stu-id="16f04-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="16f04-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="16f04-159">Request</span></span>
<span data-ttu-id="16f04-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16f04-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16f04-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="16f04-161">Response</span></span>
<span data-ttu-id="16f04-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16f04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





