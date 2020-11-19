---
title: Обновление Девицекоманажементаусоритиконфигуратион
description: Обновление свойств объекта Девицекоманажементаусоритиконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8a9e6ed4177c866d7945841cc4ca66404faea895
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302056"
---
# <a name="update-devicecomanagementauthorityconfiguration"></a><span data-ttu-id="cc228-103">Обновление Девицекоманажементаусоритиконфигуратион</span><span class="sxs-lookup"><span data-stu-id="cc228-103">Update deviceComanagementAuthorityConfiguration</span></span>

<span data-ttu-id="cc228-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc228-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc228-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc228-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc228-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc228-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc228-107">Обновление свойств объекта [девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cc228-107">Update the properties of a [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc228-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cc228-108">Prerequisites</span></span>
<span data-ttu-id="cc228-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc228-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc228-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc228-111">Permission type</span></span>|<span data-ttu-id="cc228-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc228-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc228-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc228-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc228-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc228-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cc228-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc228-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc228-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc228-116">Not supported.</span></span>|
|<span data-ttu-id="cc228-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cc228-117">Application</span></span>|<span data-ttu-id="cc228-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc228-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc228-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc228-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cc228-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cc228-120">Request headers</span></span>
|<span data-ttu-id="cc228-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc228-121">Header</span></span>|<span data-ttu-id="cc228-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cc228-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc228-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc228-123">Authorization</span></span>|<span data-ttu-id="cc228-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc228-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc228-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc228-125">Accept</span></span>|<span data-ttu-id="cc228-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc228-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc228-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc228-127">Request body</span></span>
<span data-ttu-id="cc228-128">В тексте запроса добавьте представление объекта [девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc228-128">In the request body, supply a JSON representation for the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>

<span data-ttu-id="cc228-129">В следующей таблице приведены свойства, необходимые при создании [девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc228-129">The following table shows the properties that are required when you create the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md).</span></span>

|<span data-ttu-id="cc228-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc228-130">Property</span></span>|<span data-ttu-id="cc228-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cc228-131">Type</span></span>|<span data-ttu-id="cc228-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cc228-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc228-133">id</span><span class="sxs-lookup"><span data-stu-id="cc228-133">id</span></span>|<span data-ttu-id="cc228-134">String</span><span class="sxs-lookup"><span data-stu-id="cc228-134">String</span></span>|<span data-ttu-id="cc228-135">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc228-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cc228-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cc228-136">displayName</span></span>|<span data-ttu-id="cc228-137">String</span><span class="sxs-lookup"><span data-stu-id="cc228-137">String</span></span>|<span data-ttu-id="cc228-138">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc228-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cc228-139">description</span><span class="sxs-lookup"><span data-stu-id="cc228-139">description</span></span>|<span data-ttu-id="cc228-140">String</span><span class="sxs-lookup"><span data-stu-id="cc228-140">String</span></span>|<span data-ttu-id="cc228-141">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc228-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cc228-142">priority</span><span class="sxs-lookup"><span data-stu-id="cc228-142">priority</span></span>|<span data-ttu-id="cc228-143">Int32</span><span class="sxs-lookup"><span data-stu-id="cc228-143">Int32</span></span>|<span data-ttu-id="cc228-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="cc228-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="cc228-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="cc228-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="cc228-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc228-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cc228-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc228-147">createdDateTime</span></span>|<span data-ttu-id="cc228-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc228-148">DateTimeOffset</span></span>|<span data-ttu-id="cc228-149">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc228-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cc228-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc228-150">lastModifiedDateTime</span></span>|<span data-ttu-id="cc228-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc228-151">DateTimeOffset</span></span>|<span data-ttu-id="cc228-152">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc228-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cc228-153">version</span><span class="sxs-lookup"><span data-stu-id="cc228-153">version</span></span>|<span data-ttu-id="cc228-154">Int32</span><span class="sxs-lookup"><span data-stu-id="cc228-154">Int32</span></span>|<span data-ttu-id="cc228-155">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc228-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cc228-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cc228-156">roleScopeTagIds</span></span>|<span data-ttu-id="cc228-157">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cc228-157">String collection</span></span>|<span data-ttu-id="cc228-158">Необязательные теги области применения роли для ограничений регистрации.</span><span class="sxs-lookup"><span data-stu-id="cc228-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="cc228-159">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc228-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cc228-160">манажеддевицеаусорити</span><span class="sxs-lookup"><span data-stu-id="cc228-160">managedDeviceAuthority</span></span>|<span data-ttu-id="cc228-161">Int32</span><span class="sxs-lookup"><span data-stu-id="cc228-161">Int32</span></span>|<span data-ttu-id="cc228-162">Конфигурация центра управления Манажеддевицеаусорити</span><span class="sxs-lookup"><span data-stu-id="cc228-162">CoManagement Authority configuration ManagedDeviceAuthority</span></span>|
|<span data-ttu-id="cc228-163">инсталлконфигуратионманажеражент</span><span class="sxs-lookup"><span data-stu-id="cc228-163">installConfigurationManagerAgent</span></span>|<span data-ttu-id="cc228-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc228-164">Boolean</span></span>|<span data-ttu-id="cc228-165">Конфигурация центра управления Инсталлконфигуратионманажеражент</span><span class="sxs-lookup"><span data-stu-id="cc228-165">CoManagement Authority configuration InstallConfigurationManagerAgent</span></span>|
|<span data-ttu-id="cc228-166">конфигуратионманажераженткоммандлинеаргумент</span><span class="sxs-lookup"><span data-stu-id="cc228-166">configurationManagerAgentCommandLineArgument</span></span>|<span data-ttu-id="cc228-167">String</span><span class="sxs-lookup"><span data-stu-id="cc228-167">String</span></span>|<span data-ttu-id="cc228-168">Конфигурация центра управления Конфигуратионманажераженткоммандлинеаргумент</span><span class="sxs-lookup"><span data-stu-id="cc228-168">CoManagement Authority configuration ConfigurationManagerAgentCommandLineArgument</span></span>|



## <a name="response"></a><span data-ttu-id="cc228-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc228-169">Response</span></span>
<span data-ttu-id="cc228-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицекоманажементаусоритиконфигуратион](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc228-170">If successful, this method returns a `200 OK` response code and an updated [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc228-171">Пример</span><span class="sxs-lookup"><span data-stu-id="cc228-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc228-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc228-172">Request</span></span>
<span data-ttu-id="cc228-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc228-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cc228-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc228-174">Response</span></span>
<span data-ttu-id="cc228-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc228-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




