---
title: Создание windows10EnrollmentCompletionPageConfiguration
description: Создание нового объекта windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9751c71cee378eabe3bbbf065e2e5ba3e0cdd337
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957033"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="56702-103">Создание windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="56702-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="56702-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56702-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56702-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56702-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56702-106">Создание нового объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="56702-106">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56702-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="56702-107">Prerequisites</span></span>
<span data-ttu-id="56702-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56702-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56702-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56702-110">Permission type</span></span>|<span data-ttu-id="56702-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="56702-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56702-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56702-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56702-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56702-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="56702-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56702-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56702-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56702-115">Not supported.</span></span>|
|<span data-ttu-id="56702-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56702-116">Application</span></span>|<span data-ttu-id="56702-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56702-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56702-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56702-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="56702-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56702-119">Request headers</span></span>
|<span data-ttu-id="56702-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56702-120">Header</span></span>|<span data-ttu-id="56702-121">Значение</span><span class="sxs-lookup"><span data-stu-id="56702-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56702-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56702-122">Authorization</span></span>|<span data-ttu-id="56702-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56702-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56702-124">Accept</span><span class="sxs-lookup"><span data-stu-id="56702-124">Accept</span></span>|<span data-ttu-id="56702-125">application/json</span><span class="sxs-lookup"><span data-stu-id="56702-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56702-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56702-126">Request body</span></span>
<span data-ttu-id="56702-127">В тексте запроса добавьте представление объекта windows10EnrollmentCompletionPageConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56702-127">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="56702-128">В следующей таблице приведены свойства, необходимые при создании windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="56702-128">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="56702-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="56702-129">Property</span></span>|<span data-ttu-id="56702-130">Тип</span><span class="sxs-lookup"><span data-stu-id="56702-130">Type</span></span>|<span data-ttu-id="56702-131">Описание</span><span class="sxs-lookup"><span data-stu-id="56702-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56702-132">id</span><span class="sxs-lookup"><span data-stu-id="56702-132">id</span></span>|<span data-ttu-id="56702-133">Строка</span><span class="sxs-lookup"><span data-stu-id="56702-133">String</span></span>|<span data-ttu-id="56702-134">Идентификатор конфигурации страницы состояния регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56702-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="56702-135">displayName</span><span class="sxs-lookup"><span data-stu-id="56702-135">displayName</span></span>|<span data-ttu-id="56702-136">String</span><span class="sxs-lookup"><span data-stu-id="56702-136">String</span></span>|<span data-ttu-id="56702-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56702-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="56702-138">description</span><span class="sxs-lookup"><span data-stu-id="56702-138">description</span></span>|<span data-ttu-id="56702-139">String</span><span class="sxs-lookup"><span data-stu-id="56702-139">String</span></span>|<span data-ttu-id="56702-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56702-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="56702-141">priority</span><span class="sxs-lookup"><span data-stu-id="56702-141">priority</span></span>|<span data-ttu-id="56702-142">Int32</span><span class="sxs-lookup"><span data-stu-id="56702-142">Int32</span></span>|<span data-ttu-id="56702-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56702-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="56702-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56702-144">createdDateTime</span></span>|<span data-ttu-id="56702-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56702-145">DateTimeOffset</span></span>|<span data-ttu-id="56702-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56702-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="56702-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56702-147">lastModifiedDateTime</span></span>|<span data-ttu-id="56702-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56702-148">DateTimeOffset</span></span>|<span data-ttu-id="56702-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56702-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="56702-150">version</span><span class="sxs-lookup"><span data-stu-id="56702-150">version</span></span>|<span data-ttu-id="56702-151">Int32</span><span class="sxs-lookup"><span data-stu-id="56702-151">Int32</span></span>|<span data-ttu-id="56702-152">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56702-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="56702-153">Шовинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="56702-153">showInstallationProgress</span></span>|<span data-ttu-id="56702-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="56702-154">Boolean</span></span>|<span data-ttu-id="56702-155">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="56702-155">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="56702-156">Блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="56702-156">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="56702-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="56702-157">Boolean</span></span>|<span data-ttu-id="56702-158">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="56702-158">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="56702-159">Алловдевицересетонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="56702-159">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="56702-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="56702-160">Boolean</span></span>|<span data-ttu-id="56702-161">Разрешение или блокировка сброса устройства при сбое установки</span><span class="sxs-lookup"><span data-stu-id="56702-161">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="56702-162">Алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="56702-162">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="56702-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="56702-163">Boolean</span></span>|<span data-ttu-id="56702-164">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="56702-164">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="56702-165">Кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="56702-165">customErrorMessage</span></span>|<span data-ttu-id="56702-166">String</span><span class="sxs-lookup"><span data-stu-id="56702-166">String</span></span>|<span data-ttu-id="56702-167">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="56702-167">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="56702-168">Инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="56702-168">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="56702-169">Int32</span><span class="sxs-lookup"><span data-stu-id="56702-169">Int32</span></span>|<span data-ttu-id="56702-170">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="56702-170">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="56702-171">Алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="56702-171">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="56702-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="56702-172">Boolean</span></span>|<span data-ttu-id="56702-173">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="56702-173">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="56702-174">Селектедмобилеаппидс</span><span class="sxs-lookup"><span data-stu-id="56702-174">selectedMobileAppIds</span></span>|<span data-ttu-id="56702-175">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="56702-175">String collection</span></span>|<span data-ttu-id="56702-176">Выбранные приложения для отслеживания состояния установки</span><span class="sxs-lookup"><span data-stu-id="56702-176">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="56702-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="56702-177">Response</span></span>
<span data-ttu-id="56702-178">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56702-178">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56702-179">Пример</span><span class="sxs-lookup"><span data-stu-id="56702-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="56702-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="56702-180">Request</span></span>
<span data-ttu-id="56702-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56702-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="56702-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="56702-182">Response</span></span>
<span data-ttu-id="56702-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56702-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




