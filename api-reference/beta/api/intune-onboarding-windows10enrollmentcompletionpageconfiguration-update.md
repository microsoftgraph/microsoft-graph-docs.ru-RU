---
title: Обновление windows10EnrollmentCompletionPageConfiguration
description: Обновление свойств объекта windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 862ec01be1bd6b99351d9b01f16797ae4a376e75
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981134"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="ea264-103">Обновление windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea264-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="ea264-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea264-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea264-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea264-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea264-106">Обновление свойств объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ea264-106">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea264-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea264-107">Prerequisites</span></span>
<span data-ttu-id="ea264-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea264-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea264-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea264-110">Permission type</span></span>|<span data-ttu-id="ea264-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea264-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea264-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea264-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea264-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea264-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ea264-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea264-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea264-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea264-115">Not supported.</span></span>|
|<span data-ttu-id="ea264-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea264-116">Application</span></span>|<span data-ttu-id="ea264-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea264-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea264-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea264-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ea264-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea264-119">Request headers</span></span>
|<span data-ttu-id="ea264-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea264-120">Header</span></span>|<span data-ttu-id="ea264-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ea264-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea264-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea264-122">Authorization</span></span>|<span data-ttu-id="ea264-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea264-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea264-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ea264-124">Accept</span></span>|<span data-ttu-id="ea264-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea264-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea264-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea264-126">Request body</span></span>
<span data-ttu-id="ea264-127">В тексте запроса добавьте представление объекта [Windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea264-127">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="ea264-128">В следующей таблице приведены свойства, необходимые при создании [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea264-128">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="ea264-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea264-129">Property</span></span>|<span data-ttu-id="ea264-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ea264-130">Type</span></span>|<span data-ttu-id="ea264-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ea264-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea264-132">id</span><span class="sxs-lookup"><span data-stu-id="ea264-132">id</span></span>|<span data-ttu-id="ea264-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ea264-133">String</span></span>|<span data-ttu-id="ea264-134">Идентификатор конфигурации страницы состояния регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea264-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea264-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ea264-135">displayName</span></span>|<span data-ttu-id="ea264-136">String</span><span class="sxs-lookup"><span data-stu-id="ea264-136">String</span></span>|<span data-ttu-id="ea264-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea264-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea264-138">description</span><span class="sxs-lookup"><span data-stu-id="ea264-138">description</span></span>|<span data-ttu-id="ea264-139">String</span><span class="sxs-lookup"><span data-stu-id="ea264-139">String</span></span>|<span data-ttu-id="ea264-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea264-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea264-141">priority</span><span class="sxs-lookup"><span data-stu-id="ea264-141">priority</span></span>|<span data-ttu-id="ea264-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ea264-142">Int32</span></span>|<span data-ttu-id="ea264-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea264-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea264-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea264-144">createdDateTime</span></span>|<span data-ttu-id="ea264-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea264-145">DateTimeOffset</span></span>|<span data-ttu-id="ea264-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea264-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea264-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea264-147">lastModifiedDateTime</span></span>|<span data-ttu-id="ea264-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea264-148">DateTimeOffset</span></span>|<span data-ttu-id="ea264-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea264-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea264-150">version</span><span class="sxs-lookup"><span data-stu-id="ea264-150">version</span></span>|<span data-ttu-id="ea264-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ea264-151">Int32</span></span>|<span data-ttu-id="ea264-152">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea264-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea264-153">Шовинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="ea264-153">showInstallationProgress</span></span>|<span data-ttu-id="ea264-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea264-154">Boolean</span></span>|<span data-ttu-id="ea264-155">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="ea264-155">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="ea264-156">Блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="ea264-156">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="ea264-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea264-157">Boolean</span></span>|<span data-ttu-id="ea264-158">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="ea264-158">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="ea264-159">Алловдевицересетонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="ea264-159">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="ea264-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea264-160">Boolean</span></span>|<span data-ttu-id="ea264-161">Разрешение или блокировка сброса устройства при сбое установки</span><span class="sxs-lookup"><span data-stu-id="ea264-161">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="ea264-162">Алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="ea264-162">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="ea264-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea264-163">Boolean</span></span>|<span data-ttu-id="ea264-164">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="ea264-164">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="ea264-165">Кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="ea264-165">customErrorMessage</span></span>|<span data-ttu-id="ea264-166">String</span><span class="sxs-lookup"><span data-stu-id="ea264-166">String</span></span>|<span data-ttu-id="ea264-167">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="ea264-167">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="ea264-168">Инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="ea264-168">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="ea264-169">Int32</span><span class="sxs-lookup"><span data-stu-id="ea264-169">Int32</span></span>|<span data-ttu-id="ea264-170">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="ea264-170">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="ea264-171">Алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="ea264-171">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="ea264-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea264-172">Boolean</span></span>|<span data-ttu-id="ea264-173">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="ea264-173">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="ea264-174">Селектедмобилеаппидс</span><span class="sxs-lookup"><span data-stu-id="ea264-174">selectedMobileAppIds</span></span>|<span data-ttu-id="ea264-175">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ea264-175">String collection</span></span>|<span data-ttu-id="ea264-176">Выбранные приложения для отслеживания состояния установки</span><span class="sxs-lookup"><span data-stu-id="ea264-176">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="ea264-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea264-177">Response</span></span>
<span data-ttu-id="ea264-178">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea264-178">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea264-179">Пример</span><span class="sxs-lookup"><span data-stu-id="ea264-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea264-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea264-180">Request</span></span>
<span data-ttu-id="ea264-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea264-181">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ea264-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea264-182">Response</span></span>
<span data-ttu-id="ea264-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea264-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




