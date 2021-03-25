---
title: Обновление windows10EnrollmentCompletionPageConfiguration
description: Обновление свойств объекта Windows10EnrollmentCompletionPageConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b5eec2b016fc6a61e5e241997bbb9a722ef5b27
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152588"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="d89da-103">Обновление windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="d89da-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

<span data-ttu-id="d89da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d89da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d89da-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d89da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d89da-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d89da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d89da-107">Обновление свойств объекта [Windows10EnrollmentCompletionPageConfiguration.](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d89da-107">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d89da-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d89da-108">Prerequisites</span></span>
<span data-ttu-id="d89da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d89da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d89da-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d89da-111">Permission type</span></span>|<span data-ttu-id="d89da-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d89da-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d89da-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d89da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d89da-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d89da-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d89da-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d89da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d89da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d89da-116">Not supported.</span></span>|
|<span data-ttu-id="d89da-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d89da-117">Application</span></span>|<span data-ttu-id="d89da-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d89da-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d89da-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d89da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d89da-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d89da-120">Request headers</span></span>
|<span data-ttu-id="d89da-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d89da-121">Header</span></span>|<span data-ttu-id="d89da-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d89da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d89da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d89da-123">Authorization</span></span>|<span data-ttu-id="d89da-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d89da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d89da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d89da-125">Accept</span></span>|<span data-ttu-id="d89da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d89da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d89da-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d89da-127">Request body</span></span>
<span data-ttu-id="d89da-128">В теле запроса предоставляем представление JSON для [объекта Windows10EnrollmentCompletionPageConfiguration.](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d89da-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="d89da-129">В следующей таблице показаны свойства, необходимые при создании [windows10EnrollmentCompletionPageConfiguration.](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d89da-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="d89da-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d89da-130">Property</span></span>|<span data-ttu-id="d89da-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d89da-131">Type</span></span>|<span data-ttu-id="d89da-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d89da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d89da-133">id</span><span class="sxs-lookup"><span data-stu-id="d89da-133">id</span></span>|<span data-ttu-id="d89da-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d89da-134">String</span></span>|<span data-ttu-id="d89da-135">Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d89da-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d89da-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d89da-136">displayName</span></span>|<span data-ttu-id="d89da-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d89da-137">String</span></span>|<span data-ttu-id="d89da-138">Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d89da-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d89da-139">description</span><span class="sxs-lookup"><span data-stu-id="d89da-139">description</span></span>|<span data-ttu-id="d89da-140">Строка</span><span class="sxs-lookup"><span data-stu-id="d89da-140">String</span></span>|<span data-ttu-id="d89da-141">Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d89da-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d89da-142">priority</span><span class="sxs-lookup"><span data-stu-id="d89da-142">priority</span></span>|<span data-ttu-id="d89da-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d89da-143">Int32</span></span>|<span data-ttu-id="d89da-144">Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации.</span><span class="sxs-lookup"><span data-stu-id="d89da-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="d89da-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="d89da-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="d89da-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d89da-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d89da-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d89da-147">createdDateTime</span></span>|<span data-ttu-id="d89da-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d89da-148">DateTimeOffset</span></span>|<span data-ttu-id="d89da-149">Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d89da-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d89da-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d89da-150">lastModifiedDateTime</span></span>|<span data-ttu-id="d89da-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d89da-151">DateTimeOffset</span></span>|<span data-ttu-id="d89da-152">Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d89da-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d89da-153">version</span><span class="sxs-lookup"><span data-stu-id="d89da-153">version</span></span>|<span data-ttu-id="d89da-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d89da-154">Int32</span></span>|<span data-ttu-id="d89da-155">Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d89da-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d89da-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d89da-156">roleScopeTagIds</span></span>|<span data-ttu-id="d89da-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d89da-157">String collection</span></span>|<span data-ttu-id="d89da-158">Необязательные теги области ролей для ограничений регистрации.</span><span class="sxs-lookup"><span data-stu-id="d89da-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="d89da-159">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d89da-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d89da-160">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="d89da-160">showInstallationProgress</span></span>|<span data-ttu-id="d89da-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d89da-161">Boolean</span></span>|<span data-ttu-id="d89da-162">Показать пользователю или скрыть ход установки</span><span class="sxs-lookup"><span data-stu-id="d89da-162">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="d89da-163">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="d89da-163">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="d89da-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="d89da-164">Boolean</span></span>|<span data-ttu-id="d89da-165">Разрешить пользователю повторно повторить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="d89da-165">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="d89da-166">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d89da-166">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="d89da-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="d89da-167">Boolean</span></span>|<span data-ttu-id="d89da-168">Разрешить или заблокировать сброс устройства при сбое установки</span><span class="sxs-lookup"><span data-stu-id="d89da-168">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="d89da-169">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d89da-169">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="d89da-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="d89da-170">Boolean</span></span>|<span data-ttu-id="d89da-171">Разрешить или заблокировать коллекцию журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="d89da-171">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="d89da-172">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="d89da-172">customErrorMessage</span></span>|<span data-ttu-id="d89da-173">Строка</span><span class="sxs-lookup"><span data-stu-id="d89da-173">String</span></span>|<span data-ttu-id="d89da-174">Настройка настраиваемой ошибки для демонстрации при сбое установки</span><span class="sxs-lookup"><span data-stu-id="d89da-174">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="d89da-175">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d89da-175">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="d89da-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d89da-176">Int32</span></span>|<span data-ttu-id="d89da-177">Установите время выполнения установки за несколько минут</span><span class="sxs-lookup"><span data-stu-id="d89da-177">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="d89da-178">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d89da-178">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="d89da-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="d89da-179">Boolean</span></span>|<span data-ttu-id="d89da-180">Разрешить пользователю продолжить использование устройства при сбое установки</span><span class="sxs-lookup"><span data-stu-id="d89da-180">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="d89da-181">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="d89da-181">selectedMobileAppIds</span></span>|<span data-ttu-id="d89da-182">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d89da-182">String collection</span></span>|<span data-ttu-id="d89da-183">Выбранные приложения для отслеживания состояния установки</span><span class="sxs-lookup"><span data-stu-id="d89da-183">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="d89da-184">trackInstallProgressForAutopilotOnly</span><span class="sxs-lookup"><span data-stu-id="d89da-184">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="d89da-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="d89da-185">Boolean</span></span>|<span data-ttu-id="d89da-186">Только показать ход установки для сценариев регистрации автопилота</span><span class="sxs-lookup"><span data-stu-id="d89da-186">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="d89da-187">disableUserStatusTrackingAfterFirstUser</span><span class="sxs-lookup"><span data-stu-id="d89da-187">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="d89da-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d89da-188">Boolean</span></span>|<span data-ttu-id="d89da-189">Только показать ход установки для первого регистрации после пользователя</span><span class="sxs-lookup"><span data-stu-id="d89da-189">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="d89da-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="d89da-190">Response</span></span>
<span data-ttu-id="d89da-191">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект Windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d89da-191">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d89da-192">Пример</span><span class="sxs-lookup"><span data-stu-id="d89da-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="d89da-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="d89da-193">Request</span></span>
<span data-ttu-id="d89da-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d89da-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 746

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ],
  "trackInstallProgressForAutopilotOnly": true,
  "disableUserStatusTrackingAfterFirstUser": true
}
```

### <a name="response"></a><span data-ttu-id="d89da-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="d89da-195">Response</span></span>
<span data-ttu-id="d89da-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d89da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "77bf8248-8248-77bf-4882-bf774882bf77",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ],
  "trackInstallProgressForAutopilotOnly": true,
  "disableUserStatusTrackingAfterFirstUser": true
}
```




