---
title: Обновление windows10EnrollmentCompletionPageConfiguration
description: Обновление свойств объекта windows10EnrollmentCompletionPageConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a6b886b9a8b2b4ef87ee29b6fb728afb34f55018
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941451"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="42238-103">Обновление windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="42238-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="42238-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42238-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42238-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42238-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42238-106">Обновление свойств объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="42238-106">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42238-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="42238-107">Prerequisites</span></span>
<span data-ttu-id="42238-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42238-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42238-110">Permission type</span></span>|<span data-ttu-id="42238-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42238-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42238-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42238-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42238-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42238-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="42238-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42238-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42238-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42238-115">Not supported.</span></span>|
|<span data-ttu-id="42238-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42238-116">Application</span></span>|<span data-ttu-id="42238-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42238-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42238-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42238-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="42238-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="42238-119">Request headers</span></span>
|<span data-ttu-id="42238-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42238-120">Header</span></span>|<span data-ttu-id="42238-121">Значение</span><span class="sxs-lookup"><span data-stu-id="42238-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42238-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42238-122">Authorization</span></span>|<span data-ttu-id="42238-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42238-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42238-124">Accept</span><span class="sxs-lookup"><span data-stu-id="42238-124">Accept</span></span>|<span data-ttu-id="42238-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42238-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42238-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42238-126">Request body</span></span>
<span data-ttu-id="42238-127">В тексте запроса добавьте представление объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42238-127">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="42238-128">В следующей таблице приведены свойства, необходимые при создании [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42238-128">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="42238-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="42238-129">Property</span></span>|<span data-ttu-id="42238-130">Тип</span><span class="sxs-lookup"><span data-stu-id="42238-130">Type</span></span>|<span data-ttu-id="42238-131">Описание</span><span class="sxs-lookup"><span data-stu-id="42238-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42238-132">id</span><span class="sxs-lookup"><span data-stu-id="42238-132">id</span></span>|<span data-ttu-id="42238-133">String</span><span class="sxs-lookup"><span data-stu-id="42238-133">String</span></span>|<span data-ttu-id="42238-134">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42238-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42238-135">displayName</span><span class="sxs-lookup"><span data-stu-id="42238-135">displayName</span></span>|<span data-ttu-id="42238-136">Строка</span><span class="sxs-lookup"><span data-stu-id="42238-136">String</span></span>|<span data-ttu-id="42238-137">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42238-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42238-138">description</span><span class="sxs-lookup"><span data-stu-id="42238-138">description</span></span>|<span data-ttu-id="42238-139">String</span><span class="sxs-lookup"><span data-stu-id="42238-139">String</span></span>|<span data-ttu-id="42238-140">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42238-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42238-141">priority</span><span class="sxs-lookup"><span data-stu-id="42238-141">priority</span></span>|<span data-ttu-id="42238-142">Int32</span><span class="sxs-lookup"><span data-stu-id="42238-142">Int32</span></span>|<span data-ttu-id="42238-143">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="42238-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="42238-144">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="42238-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="42238-145">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42238-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42238-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42238-146">createdDateTime</span></span>|<span data-ttu-id="42238-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42238-147">DateTimeOffset</span></span>|<span data-ttu-id="42238-148">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42238-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42238-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42238-149">lastModifiedDateTime</span></span>|<span data-ttu-id="42238-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42238-150">DateTimeOffset</span></span>|<span data-ttu-id="42238-151">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42238-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42238-152">version</span><span class="sxs-lookup"><span data-stu-id="42238-152">version</span></span>|<span data-ttu-id="42238-153">Int32</span><span class="sxs-lookup"><span data-stu-id="42238-153">Int32</span></span>|<span data-ttu-id="42238-154">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42238-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="42238-155">шовинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="42238-155">showInstallationProgress</span></span>|<span data-ttu-id="42238-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="42238-156">Boolean</span></span>|<span data-ttu-id="42238-157">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="42238-157">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="42238-158">блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="42238-158">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="42238-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="42238-159">Boolean</span></span>|<span data-ttu-id="42238-160">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="42238-160">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="42238-161">алловдевицересетонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="42238-161">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="42238-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="42238-162">Boolean</span></span>|<span data-ttu-id="42238-163">Разрешение или блокировка сброса устройства при сбое установки</span><span class="sxs-lookup"><span data-stu-id="42238-163">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="42238-164">алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="42238-164">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="42238-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="42238-165">Boolean</span></span>|<span data-ttu-id="42238-166">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="42238-166">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="42238-167">кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="42238-167">customErrorMessage</span></span>|<span data-ttu-id="42238-168">Строка</span><span class="sxs-lookup"><span data-stu-id="42238-168">String</span></span>|<span data-ttu-id="42238-169">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="42238-169">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="42238-170">инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="42238-170">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="42238-171">Int32</span><span class="sxs-lookup"><span data-stu-id="42238-171">Int32</span></span>|<span data-ttu-id="42238-172">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="42238-172">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="42238-173">алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="42238-173">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="42238-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="42238-174">Boolean</span></span>|<span data-ttu-id="42238-175">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="42238-175">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="42238-176">селектедмобилеаппидс</span><span class="sxs-lookup"><span data-stu-id="42238-176">selectedMobileAppIds</span></span>|<span data-ttu-id="42238-177">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="42238-177">String collection</span></span>|<span data-ttu-id="42238-178">Выбранные приложения для отслеживания состояния установки</span><span class="sxs-lookup"><span data-stu-id="42238-178">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="42238-179">траккинсталлпрогрессфораутопилотонли</span><span class="sxs-lookup"><span data-stu-id="42238-179">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="42238-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="42238-180">Boolean</span></span>|<span data-ttu-id="42238-181">Показывать только ход выполнения установки для сценариев автоматической пилотной установки</span><span class="sxs-lookup"><span data-stu-id="42238-181">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="42238-182">дисаблеусерстатустраккингафтерфирстусер</span><span class="sxs-lookup"><span data-stu-id="42238-182">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="42238-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="42238-183">Boolean</span></span>|<span data-ttu-id="42238-184">Показывать только сведения о ходе установки для первой процедуры регистрации пользователя</span><span class="sxs-lookup"><span data-stu-id="42238-184">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="42238-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="42238-185">Response</span></span>
<span data-ttu-id="42238-186">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42238-186">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42238-187">Пример</span><span class="sxs-lookup"><span data-stu-id="42238-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="42238-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="42238-188">Request</span></span>
<span data-ttu-id="42238-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42238-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 684

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
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

### <a name="response"></a><span data-ttu-id="42238-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="42238-190">Response</span></span>
<span data-ttu-id="42238-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42238-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 856

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "77bf8248-8248-77bf-4882-bf774882bf77",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
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





