---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 660bf4532b6393592496affe8c311c4f14cfe3ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000177"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="1f9f1-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f9f1-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="1f9f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f9f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f9f1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f9f1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f9f1-107">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f9f1-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f9f1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1f9f1-108">Prerequisites</span></span>
<span data-ttu-id="1f9f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f9f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f9f1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f9f1-111">Permission type</span></span>|<span data-ttu-id="1f9f1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f9f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f9f1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f9f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f9f1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f9f1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1f9f1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f9f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f9f1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-116">Not supported.</span></span>|
|<span data-ttu-id="1f9f1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f9f1-117">Application</span></span>|<span data-ttu-id="1f9f1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f9f1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f9f1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f9f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1f9f1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1f9f1-120">Request headers</span></span>
|<span data-ttu-id="1f9f1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f9f1-121">Header</span></span>|<span data-ttu-id="1f9f1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1f9f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f9f1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f9f1-123">Authorization</span></span>|<span data-ttu-id="1f9f1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f9f1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f9f1-125">Accept</span></span>|<span data-ttu-id="1f9f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f9f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f9f1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f9f1-127">Request body</span></span>
<span data-ttu-id="1f9f1-128">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="1f9f1-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f9f1-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="1f9f1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f9f1-130">Property</span></span>|<span data-ttu-id="1f9f1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1f9f1-131">Type</span></span>|<span data-ttu-id="1f9f1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1f9f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f9f1-133">id</span><span class="sxs-lookup"><span data-stu-id="1f9f1-133">id</span></span>|<span data-ttu-id="1f9f1-134">String</span><span class="sxs-lookup"><span data-stu-id="1f9f1-134">String</span></span>|<span data-ttu-id="1f9f1-135">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f9f1-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f9f1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1f9f1-136">displayName</span></span>|<span data-ttu-id="1f9f1-137">String</span><span class="sxs-lookup"><span data-stu-id="1f9f1-137">String</span></span>|<span data-ttu-id="1f9f1-138">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f9f1-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f9f1-139">description</span><span class="sxs-lookup"><span data-stu-id="1f9f1-139">description</span></span>|<span data-ttu-id="1f9f1-140">String</span><span class="sxs-lookup"><span data-stu-id="1f9f1-140">String</span></span>|<span data-ttu-id="1f9f1-141">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f9f1-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f9f1-142">priority</span><span class="sxs-lookup"><span data-stu-id="1f9f1-142">priority</span></span>|<span data-ttu-id="1f9f1-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1f9f1-143">Int32</span></span>|<span data-ttu-id="1f9f1-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="1f9f1-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="1f9f1-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f9f1-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f9f1-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f9f1-147">createdDateTime</span></span>|<span data-ttu-id="1f9f1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f9f1-148">DateTimeOffset</span></span>|<span data-ttu-id="1f9f1-149">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f9f1-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f9f1-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f9f1-150">lastModifiedDateTime</span></span>|<span data-ttu-id="1f9f1-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f9f1-151">DateTimeOffset</span></span>|<span data-ttu-id="1f9f1-152">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f9f1-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f9f1-153">version</span><span class="sxs-lookup"><span data-stu-id="1f9f1-153">version</span></span>|<span data-ttu-id="1f9f1-154">Int32</span><span class="sxs-lookup"><span data-stu-id="1f9f1-154">Int32</span></span>|<span data-ttu-id="1f9f1-155">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f9f1-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f9f1-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1f9f1-156">roleScopeTagIds</span></span>|<span data-ttu-id="1f9f1-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1f9f1-157">String collection</span></span>|<span data-ttu-id="1f9f1-158">Необязательные теги области применения роли для ограничений регистрации.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="1f9f1-159">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f9f1-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1f9f1-160">limit</span><span class="sxs-lookup"><span data-stu-id="1f9f1-160">limit</span></span>|<span data-ttu-id="1f9f1-161">Int32</span><span class="sxs-lookup"><span data-stu-id="1f9f1-161">Int32</span></span>|<span data-ttu-id="1f9f1-162">Максимальное число устройств, которые может регистрировать пользователь</span><span class="sxs-lookup"><span data-stu-id="1f9f1-162">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="1f9f1-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f9f1-163">Response</span></span>
<span data-ttu-id="1f9f1-164">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-164">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f9f1-165">Пример</span><span class="sxs-lookup"><span data-stu-id="1f9f1-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f9f1-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f9f1-166">Request</span></span>
<span data-ttu-id="1f9f1-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="1f9f1-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f9f1-168">Response</span></span>
<span data-ttu-id="1f9f1-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f9f1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "limit": 5
}
```






