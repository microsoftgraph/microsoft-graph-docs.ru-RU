---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ba360475199d47bda3b2c65ee6c7991bbb8fb91
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135021"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="d50a6-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="d50a6-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="d50a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d50a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d50a6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d50a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d50a6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d50a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d50a6-107">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d50a6-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d50a6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d50a6-108">Prerequisites</span></span>
<span data-ttu-id="d50a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d50a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d50a6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d50a6-111">Permission type</span></span>|<span data-ttu-id="d50a6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d50a6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d50a6-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d50a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d50a6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d50a6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d50a6-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d50a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d50a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d50a6-116">Not supported.</span></span>|
|<span data-ttu-id="d50a6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d50a6-117">Application</span></span>|<span data-ttu-id="d50a6-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d50a6-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d50a6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d50a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d50a6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d50a6-120">Request headers</span></span>
|<span data-ttu-id="d50a6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d50a6-121">Header</span></span>|<span data-ttu-id="d50a6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d50a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d50a6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d50a6-123">Authorization</span></span>|<span data-ttu-id="d50a6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d50a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d50a6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d50a6-125">Accept</span></span>|<span data-ttu-id="d50a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d50a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d50a6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d50a6-127">Request body</span></span>
<span data-ttu-id="d50a6-128">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d50a6-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="d50a6-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d50a6-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="d50a6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d50a6-130">Property</span></span>|<span data-ttu-id="d50a6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d50a6-131">Type</span></span>|<span data-ttu-id="d50a6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d50a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d50a6-133">id</span><span class="sxs-lookup"><span data-stu-id="d50a6-133">id</span></span>|<span data-ttu-id="d50a6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d50a6-134">String</span></span>|<span data-ttu-id="d50a6-135">Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d50a6-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d50a6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d50a6-136">displayName</span></span>|<span data-ttu-id="d50a6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d50a6-137">String</span></span>|<span data-ttu-id="d50a6-138">Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d50a6-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d50a6-139">description</span><span class="sxs-lookup"><span data-stu-id="d50a6-139">description</span></span>|<span data-ttu-id="d50a6-140">Строка</span><span class="sxs-lookup"><span data-stu-id="d50a6-140">String</span></span>|<span data-ttu-id="d50a6-141">Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d50a6-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d50a6-142">priority</span><span class="sxs-lookup"><span data-stu-id="d50a6-142">priority</span></span>|<span data-ttu-id="d50a6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d50a6-143">Int32</span></span>|<span data-ttu-id="d50a6-144">Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации.</span><span class="sxs-lookup"><span data-stu-id="d50a6-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="d50a6-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="d50a6-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="d50a6-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d50a6-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d50a6-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d50a6-147">createdDateTime</span></span>|<span data-ttu-id="d50a6-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d50a6-148">DateTimeOffset</span></span>|<span data-ttu-id="d50a6-149">Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d50a6-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d50a6-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d50a6-150">lastModifiedDateTime</span></span>|<span data-ttu-id="d50a6-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d50a6-151">DateTimeOffset</span></span>|<span data-ttu-id="d50a6-152">Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d50a6-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d50a6-153">version</span><span class="sxs-lookup"><span data-stu-id="d50a6-153">version</span></span>|<span data-ttu-id="d50a6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d50a6-154">Int32</span></span>|<span data-ttu-id="d50a6-155">Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d50a6-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d50a6-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d50a6-156">roleScopeTagIds</span></span>|<span data-ttu-id="d50a6-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d50a6-157">String collection</span></span>|<span data-ttu-id="d50a6-158">Необязательные теги области ролей для ограничений регистрации.</span><span class="sxs-lookup"><span data-stu-id="d50a6-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="d50a6-159">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d50a6-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d50a6-160">limit</span><span class="sxs-lookup"><span data-stu-id="d50a6-160">limit</span></span>|<span data-ttu-id="d50a6-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d50a6-161">Int32</span></span>|<span data-ttu-id="d50a6-162">Максимальное число устройств, которые пользователь может записать</span><span class="sxs-lookup"><span data-stu-id="d50a6-162">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="d50a6-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="d50a6-163">Response</span></span>
<span data-ttu-id="d50a6-164">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d50a6-164">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d50a6-165">Пример</span><span class="sxs-lookup"><span data-stu-id="d50a6-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="d50a6-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="d50a6-166">Request</span></span>
<span data-ttu-id="d50a6-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d50a6-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d50a6-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="d50a6-168">Response</span></span>
<span data-ttu-id="d50a6-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d50a6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




