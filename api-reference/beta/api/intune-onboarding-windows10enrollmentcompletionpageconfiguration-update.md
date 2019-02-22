---
title: Обновление windows10EnrollmentCompletionPageConfiguration
description: Обновление свойств объекта windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3576371d7e213e1c2c5ae2436339be226ebd2506
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171080"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="40336-103">Обновление windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="40336-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="40336-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40336-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40336-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40336-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40336-106">Обновление свойств объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="40336-106">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40336-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="40336-107">Prerequisites</span></span>
<span data-ttu-id="40336-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="40336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="40336-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40336-110">Permission type</span></span>|<span data-ttu-id="40336-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40336-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40336-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40336-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40336-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40336-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="40336-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40336-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40336-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40336-115">Not supported.</span></span>|
|<span data-ttu-id="40336-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40336-116">Application</span></span>|<span data-ttu-id="40336-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40336-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40336-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40336-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="40336-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40336-119">Request headers</span></span>
|<span data-ttu-id="40336-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40336-120">Header</span></span>|<span data-ttu-id="40336-121">Значение</span><span class="sxs-lookup"><span data-stu-id="40336-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40336-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40336-122">Authorization</span></span>|<span data-ttu-id="40336-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="40336-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40336-124">Accept</span><span class="sxs-lookup"><span data-stu-id="40336-124">Accept</span></span>|<span data-ttu-id="40336-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40336-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40336-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40336-126">Request body</span></span>
<span data-ttu-id="40336-127">В тексте запроса добавьте представление объекта [Windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40336-127">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="40336-128">В следующей таблице приведены свойства, необходимые при создании [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40336-128">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="40336-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="40336-129">Property</span></span>|<span data-ttu-id="40336-130">Тип</span><span class="sxs-lookup"><span data-stu-id="40336-130">Type</span></span>|<span data-ttu-id="40336-131">Описание</span><span class="sxs-lookup"><span data-stu-id="40336-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40336-132">id</span><span class="sxs-lookup"><span data-stu-id="40336-132">id</span></span>|<span data-ttu-id="40336-133">String</span><span class="sxs-lookup"><span data-stu-id="40336-133">String</span></span>|<span data-ttu-id="40336-134">Идентификатор конфигурации страницы состояния регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40336-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="40336-135">displayName</span><span class="sxs-lookup"><span data-stu-id="40336-135">displayName</span></span>|<span data-ttu-id="40336-136">String</span><span class="sxs-lookup"><span data-stu-id="40336-136">String</span></span>|<span data-ttu-id="40336-137">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40336-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="40336-138">description</span><span class="sxs-lookup"><span data-stu-id="40336-138">description</span></span>|<span data-ttu-id="40336-139">String</span><span class="sxs-lookup"><span data-stu-id="40336-139">String</span></span>|<span data-ttu-id="40336-140">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40336-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="40336-141">priority</span><span class="sxs-lookup"><span data-stu-id="40336-141">priority</span></span>|<span data-ttu-id="40336-142">Int32</span><span class="sxs-lookup"><span data-stu-id="40336-142">Int32</span></span>|<span data-ttu-id="40336-143">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40336-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="40336-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40336-144">createdDateTime</span></span>|<span data-ttu-id="40336-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40336-145">DateTimeOffset</span></span>|<span data-ttu-id="40336-146">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40336-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="40336-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40336-147">lastModifiedDateTime</span></span>|<span data-ttu-id="40336-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40336-148">DateTimeOffset</span></span>|<span data-ttu-id="40336-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40336-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="40336-150">version</span><span class="sxs-lookup"><span data-stu-id="40336-150">version</span></span>|<span data-ttu-id="40336-151">Int32</span><span class="sxs-lookup"><span data-stu-id="40336-151">Int32</span></span>|<span data-ttu-id="40336-152">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40336-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="40336-153">Шовинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="40336-153">showInstallationProgress</span></span>|<span data-ttu-id="40336-154">Логический</span><span class="sxs-lookup"><span data-stu-id="40336-154">Boolean</span></span>|<span data-ttu-id="40336-155">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="40336-155">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="40336-156">Блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="40336-156">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="40336-157">Логический</span><span class="sxs-lookup"><span data-stu-id="40336-157">Boolean</span></span>|<span data-ttu-id="40336-158">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="40336-158">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="40336-159">Алловдевицересетонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="40336-159">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="40336-160">Логический</span><span class="sxs-lookup"><span data-stu-id="40336-160">Boolean</span></span>|<span data-ttu-id="40336-161">Разрешение или блокировка сброса устройства при сбое установки</span><span class="sxs-lookup"><span data-stu-id="40336-161">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="40336-162">Алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="40336-162">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="40336-163">Логический</span><span class="sxs-lookup"><span data-stu-id="40336-163">Boolean</span></span>|<span data-ttu-id="40336-164">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="40336-164">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="40336-165">Кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="40336-165">customErrorMessage</span></span>|<span data-ttu-id="40336-166">String</span><span class="sxs-lookup"><span data-stu-id="40336-166">String</span></span>|<span data-ttu-id="40336-167">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="40336-167">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="40336-168">Инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="40336-168">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="40336-169">Int32</span><span class="sxs-lookup"><span data-stu-id="40336-169">Int32</span></span>|<span data-ttu-id="40336-170">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="40336-170">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="40336-171">Алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="40336-171">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="40336-172">Логический</span><span class="sxs-lookup"><span data-stu-id="40336-172">Boolean</span></span>|<span data-ttu-id="40336-173">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="40336-173">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="40336-174">Селектедмобилеаппидс</span><span class="sxs-lookup"><span data-stu-id="40336-174">selectedMobileAppIds</span></span>|<span data-ttu-id="40336-175">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="40336-175">String collection</span></span>|<span data-ttu-id="40336-176">Выбранные приложения для отслеживания состояния установки</span><span class="sxs-lookup"><span data-stu-id="40336-176">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="40336-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="40336-177">Response</span></span>
<span data-ttu-id="40336-178">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40336-178">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40336-179">Пример</span><span class="sxs-lookup"><span data-stu-id="40336-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="40336-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="40336-180">Request</span></span>
<span data-ttu-id="40336-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40336-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 583

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="40336-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="40336-182">Response</span></span>
<span data-ttu-id="40336-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40336-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 755

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
  ]
}
```




