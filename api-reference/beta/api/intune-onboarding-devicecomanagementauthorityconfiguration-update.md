---
title: Обновление deviceComanagementAuthorityConfiguration
description: Обновление свойств объекта deviceComanagementAuthorityConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ab03be505736eb358e784d68ce97fd924526a9a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135091"
---
# <a name="update-devicecomanagementauthorityconfiguration"></a><span data-ttu-id="aabd6-103">Обновление deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="aabd6-103">Update deviceComanagementAuthorityConfiguration</span></span>

<span data-ttu-id="aabd6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aabd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aabd6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aabd6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aabd6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aabd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aabd6-107">Обновление свойств объекта [deviceComanagementAuthorityConfiguration.](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aabd6-107">Update the properties of a [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aabd6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aabd6-108">Prerequisites</span></span>
<span data-ttu-id="aabd6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aabd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aabd6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aabd6-111">Permission type</span></span>|<span data-ttu-id="aabd6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aabd6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aabd6-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aabd6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aabd6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aabd6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aabd6-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aabd6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aabd6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aabd6-116">Not supported.</span></span>|
|<span data-ttu-id="aabd6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="aabd6-117">Application</span></span>|<span data-ttu-id="aabd6-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aabd6-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aabd6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aabd6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aabd6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aabd6-120">Request headers</span></span>
|<span data-ttu-id="aabd6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aabd6-121">Header</span></span>|<span data-ttu-id="aabd6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aabd6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aabd6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aabd6-123">Authorization</span></span>|<span data-ttu-id="aabd6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aabd6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aabd6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aabd6-125">Accept</span></span>|<span data-ttu-id="aabd6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aabd6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aabd6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aabd6-127">Request body</span></span>
<span data-ttu-id="aabd6-128">В теле запроса поставляем представление JSON для [объекта deviceComanagementAuthorityConfiguration.](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aabd6-128">In the request body, supply a JSON representation for the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

<span data-ttu-id="aabd6-129">В следующей таблице показаны свойства, необходимые при создании [устройстваComanagementAuthorityConfiguration.](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aabd6-129">The following table shows the properties that are required when you create the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md).</span></span>

|<span data-ttu-id="aabd6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aabd6-130">Property</span></span>|<span data-ttu-id="aabd6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aabd6-131">Type</span></span>|<span data-ttu-id="aabd6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aabd6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aabd6-133">id</span><span class="sxs-lookup"><span data-stu-id="aabd6-133">id</span></span>|<span data-ttu-id="aabd6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="aabd6-134">String</span></span>|<span data-ttu-id="aabd6-135">Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aabd6-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aabd6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="aabd6-136">displayName</span></span>|<span data-ttu-id="aabd6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="aabd6-137">String</span></span>|<span data-ttu-id="aabd6-138">Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aabd6-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aabd6-139">description</span><span class="sxs-lookup"><span data-stu-id="aabd6-139">description</span></span>|<span data-ttu-id="aabd6-140">Строка</span><span class="sxs-lookup"><span data-stu-id="aabd6-140">String</span></span>|<span data-ttu-id="aabd6-141">Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aabd6-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aabd6-142">priority</span><span class="sxs-lookup"><span data-stu-id="aabd6-142">priority</span></span>|<span data-ttu-id="aabd6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="aabd6-143">Int32</span></span>|<span data-ttu-id="aabd6-144">Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации.</span><span class="sxs-lookup"><span data-stu-id="aabd6-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="aabd6-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="aabd6-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="aabd6-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aabd6-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aabd6-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aabd6-147">createdDateTime</span></span>|<span data-ttu-id="aabd6-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aabd6-148">DateTimeOffset</span></span>|<span data-ttu-id="aabd6-149">Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aabd6-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aabd6-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aabd6-150">lastModifiedDateTime</span></span>|<span data-ttu-id="aabd6-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aabd6-151">DateTimeOffset</span></span>|<span data-ttu-id="aabd6-152">Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aabd6-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aabd6-153">version</span><span class="sxs-lookup"><span data-stu-id="aabd6-153">version</span></span>|<span data-ttu-id="aabd6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="aabd6-154">Int32</span></span>|<span data-ttu-id="aabd6-155">Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aabd6-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aabd6-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aabd6-156">roleScopeTagIds</span></span>|<span data-ttu-id="aabd6-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aabd6-157">String collection</span></span>|<span data-ttu-id="aabd6-158">Необязательные теги области ролей для ограничений регистрации.</span><span class="sxs-lookup"><span data-stu-id="aabd6-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="aabd6-159">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aabd6-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="aabd6-160">managedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="aabd6-160">managedDeviceAuthority</span></span>|<span data-ttu-id="aabd6-161">Int32</span><span class="sxs-lookup"><span data-stu-id="aabd6-161">Int32</span></span>|<span data-ttu-id="aabd6-162">Конфигурация Управления CoManagement ManagedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="aabd6-162">CoManagement Authority configuration ManagedDeviceAuthority</span></span>|
|<span data-ttu-id="aabd6-163">installConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="aabd6-163">installConfigurationManagerAgent</span></span>|<span data-ttu-id="aabd6-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="aabd6-164">Boolean</span></span>|<span data-ttu-id="aabd6-165">Конфигурация Управления CoManagement InstallConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="aabd6-165">CoManagement Authority configuration InstallConfigurationManagerAgent</span></span>|
|<span data-ttu-id="aabd6-166">configurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="aabd6-166">configurationManagerAgentCommandLineArgument</span></span>|<span data-ttu-id="aabd6-167">Строка</span><span class="sxs-lookup"><span data-stu-id="aabd6-167">String</span></span>|<span data-ttu-id="aabd6-168">Конфигурация CoManagement Authority ConfigurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="aabd6-168">CoManagement Authority configuration ConfigurationManagerAgentCommandLineArgument</span></span>|



## <a name="response"></a><span data-ttu-id="aabd6-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="aabd6-169">Response</span></span>
<span data-ttu-id="aabd6-170">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aabd6-170">If successful, this method returns a `200 OK` response code and an updated [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aabd6-171">Пример</span><span class="sxs-lookup"><span data-stu-id="aabd6-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="aabd6-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="aabd6-172">Request</span></span>
<span data-ttu-id="aabd6-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aabd6-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "managedDeviceAuthority": 6,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "Configuration Manager Agent Command Line Argument value"
}
```

### <a name="response"></a><span data-ttu-id="aabd6-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="aabd6-174">Response</span></span>
<span data-ttu-id="aabd6-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aabd6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 617

{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "id": "0ba0057f-057f-0ba0-7f05-a00b7f05a00b",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "managedDeviceAuthority": 6,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "Configuration Manager Agent Command Line Argument value"
}
```




