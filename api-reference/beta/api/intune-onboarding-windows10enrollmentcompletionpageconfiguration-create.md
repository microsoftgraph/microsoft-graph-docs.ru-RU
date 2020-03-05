---
title: Создание windows10EnrollmentCompletionPageConfiguration
description: Создание нового объекта windows10EnrollmentCompletionPageConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a3efa2a669ac11123bd4480b7a3092717528c932
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461636"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="c61fb-103">Создание windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="c61fb-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

<span data-ttu-id="c61fb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c61fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c61fb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c61fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c61fb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c61fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c61fb-107">Создание нового объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c61fb-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c61fb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c61fb-108">Prerequisites</span></span>
<span data-ttu-id="c61fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c61fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c61fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c61fb-111">Permission type</span></span>|<span data-ttu-id="c61fb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c61fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c61fb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c61fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c61fb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c61fb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c61fb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c61fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c61fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c61fb-116">Not supported.</span></span>|
|<span data-ttu-id="c61fb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c61fb-117">Application</span></span>|<span data-ttu-id="c61fb-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c61fb-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c61fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c61fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c61fb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c61fb-120">Request headers</span></span>
|<span data-ttu-id="c61fb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c61fb-121">Header</span></span>|<span data-ttu-id="c61fb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c61fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c61fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c61fb-123">Authorization</span></span>|<span data-ttu-id="c61fb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c61fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c61fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c61fb-125">Accept</span></span>|<span data-ttu-id="c61fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c61fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c61fb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c61fb-127">Request body</span></span>
<span data-ttu-id="c61fb-128">В тексте запроса добавьте представление объекта windows10EnrollmentCompletionPageConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c61fb-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="c61fb-129">В следующей таблице приведены свойства, необходимые при создании windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c61fb-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="c61fb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c61fb-130">Property</span></span>|<span data-ttu-id="c61fb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c61fb-131">Type</span></span>|<span data-ttu-id="c61fb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c61fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c61fb-133">id</span><span class="sxs-lookup"><span data-stu-id="c61fb-133">id</span></span>|<span data-ttu-id="c61fb-134">String</span><span class="sxs-lookup"><span data-stu-id="c61fb-134">String</span></span>|<span data-ttu-id="c61fb-135">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c61fb-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c61fb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c61fb-136">displayName</span></span>|<span data-ttu-id="c61fb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c61fb-137">String</span></span>|<span data-ttu-id="c61fb-138">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c61fb-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c61fb-139">description</span><span class="sxs-lookup"><span data-stu-id="c61fb-139">description</span></span>|<span data-ttu-id="c61fb-140">String</span><span class="sxs-lookup"><span data-stu-id="c61fb-140">String</span></span>|<span data-ttu-id="c61fb-141">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c61fb-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c61fb-142">priority</span><span class="sxs-lookup"><span data-stu-id="c61fb-142">priority</span></span>|<span data-ttu-id="c61fb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c61fb-143">Int32</span></span>|<span data-ttu-id="c61fb-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="c61fb-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="c61fb-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="c61fb-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="c61fb-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c61fb-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c61fb-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c61fb-147">createdDateTime</span></span>|<span data-ttu-id="c61fb-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c61fb-148">DateTimeOffset</span></span>|<span data-ttu-id="c61fb-149">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c61fb-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c61fb-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c61fb-150">lastModifiedDateTime</span></span>|<span data-ttu-id="c61fb-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c61fb-151">DateTimeOffset</span></span>|<span data-ttu-id="c61fb-152">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c61fb-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c61fb-153">version</span><span class="sxs-lookup"><span data-stu-id="c61fb-153">version</span></span>|<span data-ttu-id="c61fb-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c61fb-154">Int32</span></span>|<span data-ttu-id="c61fb-155">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c61fb-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c61fb-156">шовинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="c61fb-156">showInstallationProgress</span></span>|<span data-ttu-id="c61fb-157">Логический</span><span class="sxs-lookup"><span data-stu-id="c61fb-157">Boolean</span></span>|<span data-ttu-id="c61fb-158">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="c61fb-158">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="c61fb-159">блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="c61fb-159">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="c61fb-160">Логический</span><span class="sxs-lookup"><span data-stu-id="c61fb-160">Boolean</span></span>|<span data-ttu-id="c61fb-161">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="c61fb-161">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="c61fb-162">алловдевицересетонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="c61fb-162">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="c61fb-163">Логический</span><span class="sxs-lookup"><span data-stu-id="c61fb-163">Boolean</span></span>|<span data-ttu-id="c61fb-164">Разрешение или блокировка сброса устройства при сбое установки</span><span class="sxs-lookup"><span data-stu-id="c61fb-164">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="c61fb-165">алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="c61fb-165">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="c61fb-166">Логический</span><span class="sxs-lookup"><span data-stu-id="c61fb-166">Boolean</span></span>|<span data-ttu-id="c61fb-167">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="c61fb-167">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="c61fb-168">кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="c61fb-168">customErrorMessage</span></span>|<span data-ttu-id="c61fb-169">String</span><span class="sxs-lookup"><span data-stu-id="c61fb-169">String</span></span>|<span data-ttu-id="c61fb-170">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="c61fb-170">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="c61fb-171">инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="c61fb-171">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="c61fb-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c61fb-172">Int32</span></span>|<span data-ttu-id="c61fb-173">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="c61fb-173">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="c61fb-174">алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="c61fb-174">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="c61fb-175">Логический</span><span class="sxs-lookup"><span data-stu-id="c61fb-175">Boolean</span></span>|<span data-ttu-id="c61fb-176">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="c61fb-176">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="c61fb-177">селектедмобилеаппидс</span><span class="sxs-lookup"><span data-stu-id="c61fb-177">selectedMobileAppIds</span></span>|<span data-ttu-id="c61fb-178">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c61fb-178">String collection</span></span>|<span data-ttu-id="c61fb-179">Выбранные приложения для отслеживания состояния установки</span><span class="sxs-lookup"><span data-stu-id="c61fb-179">Selected applications to track the installation status</span></span>|
|<span data-ttu-id="c61fb-180">траккинсталлпрогрессфораутопилотонли</span><span class="sxs-lookup"><span data-stu-id="c61fb-180">trackInstallProgressForAutopilotOnly</span></span>|<span data-ttu-id="c61fb-181">Логический</span><span class="sxs-lookup"><span data-stu-id="c61fb-181">Boolean</span></span>|<span data-ttu-id="c61fb-182">Показывать только ход выполнения установки для сценариев автоматической пилотной установки</span><span class="sxs-lookup"><span data-stu-id="c61fb-182">Only show installation progress for Autopilot enrollment scenarios</span></span>|
|<span data-ttu-id="c61fb-183">дисаблеусерстатустраккингафтерфирстусер</span><span class="sxs-lookup"><span data-stu-id="c61fb-183">disableUserStatusTrackingAfterFirstUser</span></span>|<span data-ttu-id="c61fb-184">Логический</span><span class="sxs-lookup"><span data-stu-id="c61fb-184">Boolean</span></span>|<span data-ttu-id="c61fb-185">Показывать только сведения о ходе установки для первой процедуры регистрации пользователя</span><span class="sxs-lookup"><span data-stu-id="c61fb-185">Only show installation progress for first user post enrollment</span></span>|



## <a name="response"></a><span data-ttu-id="c61fb-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="c61fb-186">Response</span></span>
<span data-ttu-id="c61fb-187">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c61fb-187">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c61fb-188">Пример</span><span class="sxs-lookup"><span data-stu-id="c61fb-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="c61fb-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="c61fb-189">Request</span></span>
<span data-ttu-id="c61fb-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c61fb-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="c61fb-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="c61fb-191">Response</span></span>
<span data-ttu-id="c61fb-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c61fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





