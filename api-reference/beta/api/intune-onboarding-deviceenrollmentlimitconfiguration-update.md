---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b8dbadcacb8d791c35a14b3714d1f7f0c3bcfac
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981253"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="7c32c-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c32c-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="7c32c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c32c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c32c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c32c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c32c-106">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c32c-106">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c32c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7c32c-107">Prerequisites</span></span>
<span data-ttu-id="7c32c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c32c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c32c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c32c-110">Permission type</span></span>|<span data-ttu-id="7c32c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c32c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c32c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c32c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c32c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c32c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c32c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c32c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c32c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c32c-115">Not supported.</span></span>|
|<span data-ttu-id="7c32c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c32c-116">Application</span></span>|<span data-ttu-id="7c32c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c32c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c32c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c32c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7c32c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c32c-119">Request headers</span></span>
|<span data-ttu-id="7c32c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c32c-120">Header</span></span>|<span data-ttu-id="7c32c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7c32c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c32c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c32c-122">Authorization</span></span>|<span data-ttu-id="7c32c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c32c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c32c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7c32c-124">Accept</span></span>|<span data-ttu-id="7c32c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c32c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c32c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c32c-126">Request body</span></span>
<span data-ttu-id="7c32c-127">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c32c-127">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="7c32c-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c32c-128">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="7c32c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c32c-129">Property</span></span>|<span data-ttu-id="7c32c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7c32c-130">Type</span></span>|<span data-ttu-id="7c32c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7c32c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c32c-132">id</span><span class="sxs-lookup"><span data-stu-id="7c32c-132">id</span></span>|<span data-ttu-id="7c32c-133">String</span><span class="sxs-lookup"><span data-stu-id="7c32c-133">String</span></span>|<span data-ttu-id="7c32c-134">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c32c-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c32c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7c32c-135">displayName</span></span>|<span data-ttu-id="7c32c-136">Строка</span><span class="sxs-lookup"><span data-stu-id="7c32c-136">String</span></span>|<span data-ttu-id="7c32c-137">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c32c-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c32c-138">description</span><span class="sxs-lookup"><span data-stu-id="7c32c-138">description</span></span>|<span data-ttu-id="7c32c-139">String</span><span class="sxs-lookup"><span data-stu-id="7c32c-139">String</span></span>|<span data-ttu-id="7c32c-140">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c32c-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c32c-141">priority</span><span class="sxs-lookup"><span data-stu-id="7c32c-141">priority</span></span>|<span data-ttu-id="7c32c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7c32c-142">Int32</span></span>|<span data-ttu-id="7c32c-143">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="7c32c-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="7c32c-144">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="7c32c-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="7c32c-145">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c32c-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c32c-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c32c-146">createdDateTime</span></span>|<span data-ttu-id="7c32c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c32c-147">DateTimeOffset</span></span>|<span data-ttu-id="7c32c-148">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c32c-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c32c-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c32c-149">lastModifiedDateTime</span></span>|<span data-ttu-id="7c32c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c32c-150">DateTimeOffset</span></span>|<span data-ttu-id="7c32c-151">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c32c-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c32c-152">version</span><span class="sxs-lookup"><span data-stu-id="7c32c-152">version</span></span>|<span data-ttu-id="7c32c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="7c32c-153">Int32</span></span>|<span data-ttu-id="7c32c-154">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c32c-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c32c-155">limit</span><span class="sxs-lookup"><span data-stu-id="7c32c-155">limit</span></span>|<span data-ttu-id="7c32c-156">Int32</span><span class="sxs-lookup"><span data-stu-id="7c32c-156">Int32</span></span>|<span data-ttu-id="7c32c-157">Максимальное число устройств, которые может регистрировать пользователь</span><span class="sxs-lookup"><span data-stu-id="7c32c-157">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="7c32c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c32c-158">Response</span></span>
<span data-ttu-id="7c32c-159">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7c32c-159">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c32c-160">Пример</span><span class="sxs-lookup"><span data-stu-id="7c32c-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c32c-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c32c-161">Request</span></span>
<span data-ttu-id="7c32c-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c32c-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c32c-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c32c-163">Response</span></span>
<span data-ttu-id="7c32c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c32c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





