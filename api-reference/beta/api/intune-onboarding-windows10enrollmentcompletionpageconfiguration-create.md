---
title: Создание windows10EnrollmentCompletionPageConfiguration
description: Создание нового объекта windows10EnrollmentCompletionPageConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a46ca35809f28effdf45a5f85b8da171b30c9698
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178453"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="4925e-103">Создание windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="4925e-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

<span data-ttu-id="4925e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4925e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4925e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4925e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4925e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4925e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4925e-107">Создание нового объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4925e-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4925e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4925e-108">Prerequisites</span></span>
<span data-ttu-id="4925e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4925e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4925e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4925e-111">Permission type</span></span>|<span data-ttu-id="4925e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4925e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4925e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4925e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4925e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4925e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4925e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4925e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4925e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4925e-116">Not supported.</span></span>|
|<span data-ttu-id="4925e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4925e-117">Application</span></span>|<span data-ttu-id="4925e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4925e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4925e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4925e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4925e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4925e-120">Request headers</span></span>
|<span data-ttu-id="4925e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4925e-121">Header</span></span>|<span data-ttu-id="4925e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4925e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4925e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4925e-123">Authorization</span></span>|<span data-ttu-id="4925e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4925e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4925e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4925e-125">Accept</span></span>|<span data-ttu-id="4925e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4925e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4925e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4925e-127">Request body</span></span>
<span data-ttu-id="4925e-128">В тексте запроса добавьте представление объекта windows10EnrollmentCompletionPageConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4925e-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="4925e-129">В следующей таблице приведены свойства, необходимые при создании windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4925e-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="4925e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4925e-130">Property</span></span>|<span data-ttu-id="4925e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4925e-131">Type</span></span>|<span data-ttu-id="4925e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4925e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4925e-133">id</span><span class="sxs-lookup"><span data-stu-id="4925e-133">id</span></span>|<span data-ttu-id="4925e-134">String</span><span class="sxs-lookup"><span data-stu-id="4925e-134">String</span></span>|<span data-ttu-id="4925e-135">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4925e-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4925e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4925e-136">displayName</span></span>|<span data-ttu-id="4925e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4925e-137">String</span></span>|<span data-ttu-id="4925e-138">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4925e-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4925e-139">description</span><span class="sxs-lookup"><span data-stu-id="4925e-139">description</span></span>|<span data-ttu-id="4925e-140">String</span><span class="sxs-lookup"><span data-stu-id="4925e-140">String</span></span>|<span data-ttu-id="4925e-141">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4925e-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4925e-142">priority</span><span class="sxs-lookup"><span data-stu-id="4925e-142">priority</span></span>|<span data-ttu-id="4925e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4925e-143">Int32</span></span>|<span data-ttu-id="4925e-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="4925e-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="4925e-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="4925e-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="4925e-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4925e-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4925e-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4925e-147">createdDateTime</span></span>|<span data-ttu-id="4925e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4925e-148">DateTimeOffset</span></span>|<span data-ttu-id="4925e-149">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4925e-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4925e-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4925e-150">lastModifiedDateTime</span></span>|<span data-ttu-id="4925e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4925e-151">DateTimeOffset</span></span>|<span data-ttu-id="4925e-152">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4925e-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4925e-153">version</span><span class="sxs-lookup"><span data-stu-id="4925e-153">version</span></span>|<span data-ttu-id="4925e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="4925e-154">Int32</span></span>|<span data-ttu-id="4925e-155">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4925e-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4925e-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4925e-156">roleScopeTagIds</span></span>|<span data-ttu-id="4925e-157">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4925e-157">String collection</span></span>|<span data-ttu-id="4925e-158">Необязательные теги области применения роли для ограничений регистрации.</span><span class="sxs-lookup"><span data-stu-id="4925e-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="4925e-159">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4925e-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4925e-160">шовинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="4925e-160">showInstallationProgress</span></span>|<span data-ttu-id="4925e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4925e-161">Boolean</span></span>|<span data-ttu-id="4925e-162">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="4925e-162">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="4925e-163">блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="4925e-163">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="4925e-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="4925e-164">Boolean</span></span>|<span data-ttu-id="4925e-165">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="4925e-165">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="4925e-166">алловдевицересетонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="4925e-166">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="4925e-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="4925e-167">Boolean</span></span>|<span data-ttu-id="4925e-168">Разрешение или блокировка сброса устройства при сбое установки</span><span class="sxs-lookup"><span data-stu-id="4925e-168">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="4925e-169">алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="4925e-169">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="4925e-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="4925e-170">Boolean</span></span>|<span data-ttu-id="4925e-171">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="4925e-171">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="4925e-172">кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="4925e-172">customErrorMessage</span></span>|<span data-ttu-id="4925e-173">Строка</span><span class="sxs-lookup"><span data-stu-id="4925e-173">String</span></span>|<span data-ttu-id="4925e-174">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="4925e-174">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="4925e-175">инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="4925e-175">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="4925e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4925e-176">Int32</span></span>|<span data-ttu-id="4925e-177">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="4925e-177">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="4925e-178">алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="4925e-178">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="4925e-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="4925e-179">Boolean</span></span>|<span data-ttu-id="4925e-180">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="4925e-180">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="4925e-181">селектедмобилеаппидс</span><span class="sxs-lookup"><span data-stu-id="4925e-181">selectedMobileAppIds</span></span>|<span data-ttu-id="4925e-182">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4925e-182">String collection</span></span>|<span data-ttu-id="4925e-183">Выбранные приложения для отслеживания состояния установки</span><span class="sxs-lookup"><span data-stu-id="4925e-183">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="4925e-184">траккинсталлпрогрессфораутопилотонли</span><span class="sxs-lookup"><span data-stu-id="4925e-184">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="4925e-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="4925e-185">Boolean</span></span>|<span data-ttu-id="4925e-186">Показывать только ход выполнения установки для сценариев автоматической пилотной установки</span><span class="sxs-lookup"><span data-stu-id="4925e-186">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="4925e-187">дисаблеусерстатустраккингафтерфирстусер</span><span class="sxs-lookup"><span data-stu-id="4925e-187">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="4925e-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="4925e-188">Boolean</span></span>|<span data-ttu-id="4925e-189">Показывать только сведения о ходе установки для первой процедуры регистрации пользователя</span><span class="sxs-lookup"><span data-stu-id="4925e-189">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="4925e-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="4925e-190">Response</span></span>
<span data-ttu-id="4925e-191">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4925e-191">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4925e-192">Пример</span><span class="sxs-lookup"><span data-stu-id="4925e-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="4925e-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="4925e-193">Request</span></span>
<span data-ttu-id="4925e-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4925e-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="4925e-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="4925e-195">Response</span></span>
<span data-ttu-id="4925e-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4925e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



