---
title: Обновление объекта deviceEnrollmentLimitConfiguration
description: Обновление свойств объекта deviceEnrollmentLimitConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34854bb09daf1b6e36f54315e6741a6b3ce85177
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462364"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="efb8f-103">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="efb8f-103">Update deviceEnrollmentLimitConfiguration</span></span>

<span data-ttu-id="efb8f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="efb8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efb8f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efb8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efb8f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efb8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efb8f-107">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="efb8f-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efb8f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="efb8f-108">Prerequisites</span></span>
<span data-ttu-id="efb8f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efb8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efb8f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efb8f-111">Permission type</span></span>|<span data-ttu-id="efb8f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efb8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efb8f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efb8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efb8f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb8f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="efb8f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efb8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efb8f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efb8f-116">Not supported.</span></span>|
|<span data-ttu-id="efb8f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efb8f-117">Application</span></span>|<span data-ttu-id="efb8f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb8f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efb8f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efb8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="efb8f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="efb8f-120">Request headers</span></span>
|<span data-ttu-id="efb8f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efb8f-121">Header</span></span>|<span data-ttu-id="efb8f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="efb8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efb8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="efb8f-123">Authorization</span></span>|<span data-ttu-id="efb8f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efb8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efb8f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="efb8f-125">Accept</span></span>|<span data-ttu-id="efb8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efb8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efb8f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efb8f-127">Request body</span></span>
<span data-ttu-id="efb8f-128">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efb8f-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="efb8f-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="efb8f-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="efb8f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="efb8f-130">Property</span></span>|<span data-ttu-id="efb8f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="efb8f-131">Type</span></span>|<span data-ttu-id="efb8f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="efb8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efb8f-133">id</span><span class="sxs-lookup"><span data-stu-id="efb8f-133">id</span></span>|<span data-ttu-id="efb8f-134">String</span><span class="sxs-lookup"><span data-stu-id="efb8f-134">String</span></span>|<span data-ttu-id="efb8f-135">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efb8f-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="efb8f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="efb8f-136">displayName</span></span>|<span data-ttu-id="efb8f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="efb8f-137">String</span></span>|<span data-ttu-id="efb8f-138">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efb8f-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="efb8f-139">description</span><span class="sxs-lookup"><span data-stu-id="efb8f-139">description</span></span>|<span data-ttu-id="efb8f-140">String</span><span class="sxs-lookup"><span data-stu-id="efb8f-140">String</span></span>|<span data-ttu-id="efb8f-141">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efb8f-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="efb8f-142">priority</span><span class="sxs-lookup"><span data-stu-id="efb8f-142">priority</span></span>|<span data-ttu-id="efb8f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="efb8f-143">Int32</span></span>|<span data-ttu-id="efb8f-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="efb8f-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="efb8f-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="efb8f-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="efb8f-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efb8f-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="efb8f-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efb8f-147">createdDateTime</span></span>|<span data-ttu-id="efb8f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efb8f-148">DateTimeOffset</span></span>|<span data-ttu-id="efb8f-149">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efb8f-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="efb8f-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efb8f-150">lastModifiedDateTime</span></span>|<span data-ttu-id="efb8f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efb8f-151">DateTimeOffset</span></span>|<span data-ttu-id="efb8f-152">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efb8f-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="efb8f-153">version</span><span class="sxs-lookup"><span data-stu-id="efb8f-153">version</span></span>|<span data-ttu-id="efb8f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="efb8f-154">Int32</span></span>|<span data-ttu-id="efb8f-155">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efb8f-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="efb8f-156">limit</span><span class="sxs-lookup"><span data-stu-id="efb8f-156">limit</span></span>|<span data-ttu-id="efb8f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="efb8f-157">Int32</span></span>|<span data-ttu-id="efb8f-158">Максимальное число устройств, которые может регистрировать пользователь</span><span class="sxs-lookup"><span data-stu-id="efb8f-158">The maximum number of devices that a user can enroll</span></span>|



## <a name="response"></a><span data-ttu-id="efb8f-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="efb8f-159">Response</span></span>
<span data-ttu-id="efb8f-160">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="efb8f-160">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efb8f-161">Пример</span><span class="sxs-lookup"><span data-stu-id="efb8f-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="efb8f-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="efb8f-162">Request</span></span>
<span data-ttu-id="efb8f-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efb8f-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="efb8f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="efb8f-164">Response</span></span>
<span data-ttu-id="efb8f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efb8f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





