---
title: Обновление windows10EnrollmentCompletionPageConfiguration
description: Обновление свойств объекта windows10EnrollmentCompletionPageConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9524480c41d3e915e4767ce958052b1ebb45bd7c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461573"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="03259-103">Обновление windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="03259-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

<span data-ttu-id="03259-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="03259-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03259-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03259-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03259-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03259-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03259-107">Обновление свойств объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="03259-107">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03259-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03259-108">Prerequisites</span></span>
<span data-ttu-id="03259-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03259-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03259-111">Permission type</span></span>|<span data-ttu-id="03259-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03259-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03259-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03259-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03259-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03259-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="03259-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03259-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03259-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03259-116">Not supported.</span></span>|
|<span data-ttu-id="03259-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03259-117">Application</span></span>|<span data-ttu-id="03259-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03259-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03259-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03259-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="03259-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03259-120">Request headers</span></span>
|<span data-ttu-id="03259-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03259-121">Header</span></span>|<span data-ttu-id="03259-122">Значение</span><span class="sxs-lookup"><span data-stu-id="03259-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03259-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03259-123">Authorization</span></span>|<span data-ttu-id="03259-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03259-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03259-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03259-125">Accept</span></span>|<span data-ttu-id="03259-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03259-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03259-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03259-127">Request body</span></span>
<span data-ttu-id="03259-128">В тексте запроса добавьте представление объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03259-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="03259-129">В следующей таблице приведены свойства, необходимые при создании [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03259-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="03259-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="03259-130">Property</span></span>|<span data-ttu-id="03259-131">Тип</span><span class="sxs-lookup"><span data-stu-id="03259-131">Type</span></span>|<span data-ttu-id="03259-132">Описание</span><span class="sxs-lookup"><span data-stu-id="03259-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03259-133">id</span><span class="sxs-lookup"><span data-stu-id="03259-133">id</span></span>|<span data-ttu-id="03259-134">String</span><span class="sxs-lookup"><span data-stu-id="03259-134">String</span></span>|<span data-ttu-id="03259-135">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03259-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="03259-136">displayName</span><span class="sxs-lookup"><span data-stu-id="03259-136">displayName</span></span>|<span data-ttu-id="03259-137">Строка</span><span class="sxs-lookup"><span data-stu-id="03259-137">String</span></span>|<span data-ttu-id="03259-138">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03259-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="03259-139">description</span><span class="sxs-lookup"><span data-stu-id="03259-139">description</span></span>|<span data-ttu-id="03259-140">String</span><span class="sxs-lookup"><span data-stu-id="03259-140">String</span></span>|<span data-ttu-id="03259-141">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03259-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="03259-142">priority</span><span class="sxs-lookup"><span data-stu-id="03259-142">priority</span></span>|<span data-ttu-id="03259-143">Int32</span><span class="sxs-lookup"><span data-stu-id="03259-143">Int32</span></span>|<span data-ttu-id="03259-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="03259-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="03259-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="03259-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="03259-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03259-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="03259-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03259-147">createdDateTime</span></span>|<span data-ttu-id="03259-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03259-148">DateTimeOffset</span></span>|<span data-ttu-id="03259-149">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03259-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="03259-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03259-150">lastModifiedDateTime</span></span>|<span data-ttu-id="03259-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03259-151">DateTimeOffset</span></span>|<span data-ttu-id="03259-152">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03259-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="03259-153">version</span><span class="sxs-lookup"><span data-stu-id="03259-153">version</span></span>|<span data-ttu-id="03259-154">Int32</span><span class="sxs-lookup"><span data-stu-id="03259-154">Int32</span></span>|<span data-ttu-id="03259-155">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03259-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="03259-156">шовинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="03259-156">showInstallationProgress</span></span>|<span data-ttu-id="03259-157">Логический</span><span class="sxs-lookup"><span data-stu-id="03259-157">Boolean</span></span>|<span data-ttu-id="03259-158">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="03259-158">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="03259-159">блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="03259-159">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="03259-160">Логический</span><span class="sxs-lookup"><span data-stu-id="03259-160">Boolean</span></span>|<span data-ttu-id="03259-161">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="03259-161">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="03259-162">алловдевицересетонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="03259-162">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="03259-163">Логический</span><span class="sxs-lookup"><span data-stu-id="03259-163">Boolean</span></span>|<span data-ttu-id="03259-164">Разрешение или блокировка сброса устройства при сбое установки</span><span class="sxs-lookup"><span data-stu-id="03259-164">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="03259-165">алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="03259-165">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="03259-166">Логический</span><span class="sxs-lookup"><span data-stu-id="03259-166">Boolean</span></span>|<span data-ttu-id="03259-167">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="03259-167">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="03259-168">кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="03259-168">customErrorMessage</span></span>|<span data-ttu-id="03259-169">String</span><span class="sxs-lookup"><span data-stu-id="03259-169">String</span></span>|<span data-ttu-id="03259-170">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="03259-170">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="03259-171">инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="03259-171">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="03259-172">Int32</span><span class="sxs-lookup"><span data-stu-id="03259-172">Int32</span></span>|<span data-ttu-id="03259-173">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="03259-173">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="03259-174">алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="03259-174">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="03259-175">Логический</span><span class="sxs-lookup"><span data-stu-id="03259-175">Boolean</span></span>|<span data-ttu-id="03259-176">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="03259-176">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="03259-177">селектедмобилеаппидс</span><span class="sxs-lookup"><span data-stu-id="03259-177">selectedMobileAppIds</span></span>|<span data-ttu-id="03259-178">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="03259-178">String collection</span></span>|<span data-ttu-id="03259-179">Выбранные приложения для отслеживания состояния установки</span><span class="sxs-lookup"><span data-stu-id="03259-179">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="03259-180">траккинсталлпрогрессфораутопилотонли</span><span class="sxs-lookup"><span data-stu-id="03259-180">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="03259-181">Логический</span><span class="sxs-lookup"><span data-stu-id="03259-181">Boolean</span></span>|<span data-ttu-id="03259-182">Показывать только ход выполнения установки для сценариев автоматической пилотной установки</span><span class="sxs-lookup"><span data-stu-id="03259-182">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="03259-183">дисаблеусерстатустраккингафтерфирстусер</span><span class="sxs-lookup"><span data-stu-id="03259-183">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="03259-184">Логический</span><span class="sxs-lookup"><span data-stu-id="03259-184">Boolean</span></span>|<span data-ttu-id="03259-185">Показывать только сведения о ходе установки для первой процедуры регистрации пользователя</span><span class="sxs-lookup"><span data-stu-id="03259-185">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="03259-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="03259-186">Response</span></span>
<span data-ttu-id="03259-187">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03259-187">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03259-188">Пример</span><span class="sxs-lookup"><span data-stu-id="03259-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="03259-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="03259-189">Request</span></span>
<span data-ttu-id="03259-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03259-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03259-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="03259-191">Response</span></span>
<span data-ttu-id="03259-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03259-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





