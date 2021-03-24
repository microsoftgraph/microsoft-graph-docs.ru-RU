---
title: Создание deviceComanagementAuthorityConfiguration
description: Создание нового объекта deviceComanagementAuthorityConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 726113e94e51bb2eb0dc9b996f87d9a070a3bf6b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135147"
---
# <a name="create-devicecomanagementauthorityconfiguration"></a><span data-ttu-id="3e1ea-103">Создание deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e1ea-103">Create deviceComanagementAuthorityConfiguration</span></span>

<span data-ttu-id="3e1ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e1ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e1ea-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e1ea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e1ea-107">Создание нового [объекта deviceComanagementAuthorityConfiguration.](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-107">Create a new [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e1ea-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3e1ea-108">Prerequisites</span></span>
<span data-ttu-id="3e1ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e1ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e1ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e1ea-111">Permission type</span></span>|<span data-ttu-id="3e1ea-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e1ea-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e1ea-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e1ea-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3e1ea-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e1ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-116">Not supported.</span></span>|
|<span data-ttu-id="3e1ea-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3e1ea-117">Application</span></span>|<span data-ttu-id="3e1ea-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e1ea-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e1ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e1ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3e1ea-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3e1ea-120">Request headers</span></span>
|<span data-ttu-id="3e1ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e1ea-121">Header</span></span>|<span data-ttu-id="3e1ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e1ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e1ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e1ea-123">Authorization</span></span>|<span data-ttu-id="3e1ea-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e1ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e1ea-125">Accept</span></span>|<span data-ttu-id="3e1ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e1ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e1ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e1ea-127">Request body</span></span>
<span data-ttu-id="3e1ea-128">В теле запроса поставляем представление JSON для объекта deviceComanagementAuthorityConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-128">In the request body, supply a JSON representation for the deviceComanagementAuthorityConfiguration object.</span></span>

<span data-ttu-id="3e1ea-129">В следующей таблице показаны свойства, необходимые при создании устройстваComanagementAuthorityConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-129">The following table shows the properties that are required when you create the deviceComanagementAuthorityConfiguration.</span></span>

|<span data-ttu-id="3e1ea-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e1ea-130">Property</span></span>|<span data-ttu-id="3e1ea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3e1ea-131">Type</span></span>|<span data-ttu-id="3e1ea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3e1ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e1ea-133">id</span><span class="sxs-lookup"><span data-stu-id="3e1ea-133">id</span></span>|<span data-ttu-id="3e1ea-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3e1ea-134">String</span></span>|<span data-ttu-id="3e1ea-135">Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e1ea-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3e1ea-136">displayName</span></span>|<span data-ttu-id="3e1ea-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3e1ea-137">String</span></span>|<span data-ttu-id="3e1ea-138">Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e1ea-139">description</span><span class="sxs-lookup"><span data-stu-id="3e1ea-139">description</span></span>|<span data-ttu-id="3e1ea-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3e1ea-140">String</span></span>|<span data-ttu-id="3e1ea-141">Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e1ea-142">priority</span><span class="sxs-lookup"><span data-stu-id="3e1ea-142">priority</span></span>|<span data-ttu-id="3e1ea-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3e1ea-143">Int32</span></span>|<span data-ttu-id="3e1ea-144">Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="3e1ea-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="3e1ea-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e1ea-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e1ea-147">createdDateTime</span></span>|<span data-ttu-id="3e1ea-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e1ea-148">DateTimeOffset</span></span>|<span data-ttu-id="3e1ea-149">Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e1ea-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e1ea-150">lastModifiedDateTime</span></span>|<span data-ttu-id="3e1ea-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e1ea-151">DateTimeOffset</span></span>|<span data-ttu-id="3e1ea-152">Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e1ea-153">version</span><span class="sxs-lookup"><span data-stu-id="3e1ea-153">version</span></span>|<span data-ttu-id="3e1ea-154">Int32</span><span class="sxs-lookup"><span data-stu-id="3e1ea-154">Int32</span></span>|<span data-ttu-id="3e1ea-155">Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e1ea-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3e1ea-156">roleScopeTagIds</span></span>|<span data-ttu-id="3e1ea-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3e1ea-157">String collection</span></span>|<span data-ttu-id="3e1ea-158">Необязательные теги области ролей для ограничений регистрации.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="3e1ea-159">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e1ea-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e1ea-160">managedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="3e1ea-160">managedDeviceAuthority</span></span>|<span data-ttu-id="3e1ea-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3e1ea-161">Int32</span></span>|<span data-ttu-id="3e1ea-162">Конфигурация Управления CoManagement ManagedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="3e1ea-162">CoManagement Authority configuration ManagedDeviceAuthority</span></span>|
|<span data-ttu-id="3e1ea-163">installConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="3e1ea-163">installConfigurationManagerAgent</span></span>|<span data-ttu-id="3e1ea-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e1ea-164">Boolean</span></span>|<span data-ttu-id="3e1ea-165">Конфигурация Управления CoManagement InstallConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="3e1ea-165">CoManagement Authority configuration InstallConfigurationManagerAgent</span></span>|
|<span data-ttu-id="3e1ea-166">configurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="3e1ea-166">configurationManagerAgentCommandLineArgument</span></span>|<span data-ttu-id="3e1ea-167">Строка</span><span class="sxs-lookup"><span data-stu-id="3e1ea-167">String</span></span>|<span data-ttu-id="3e1ea-168">Конфигурация CoManagement Authority ConfigurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="3e1ea-168">CoManagement Authority configuration ConfigurationManagerAgentCommandLineArgument</span></span>|



## <a name="response"></a><span data-ttu-id="3e1ea-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e1ea-169">Response</span></span>
<span data-ttu-id="3e1ea-170">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-170">If successful, this method returns a `201 Created` response code and a [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e1ea-171">Пример</span><span class="sxs-lookup"><span data-stu-id="3e1ea-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e1ea-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e1ea-172">Request</span></span>
<span data-ttu-id="3e1ea-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="3e1ea-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e1ea-174">Response</span></span>
<span data-ttu-id="3e1ea-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e1ea-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




