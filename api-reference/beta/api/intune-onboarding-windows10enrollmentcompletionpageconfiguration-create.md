---
title: Создание windows10EnrollmentCompletionPageConfiguration
description: Создание нового объекта windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c2edde71ba4ec8b61fe8894f05b0a6501df053c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528045"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="d1c30-103">Создание windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1c30-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="d1c30-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1c30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1c30-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1c30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1c30-106">Создание нового объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d1c30-106">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1c30-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d1c30-107">Prerequisites</span></span>
<span data-ttu-id="d1c30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1c30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1c30-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1c30-110">Permission type</span></span>|<span data-ttu-id="d1c30-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1c30-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1c30-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1c30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1c30-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1c30-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d1c30-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1c30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1c30-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1c30-115">Not supported.</span></span>|
|<span data-ttu-id="d1c30-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1c30-116">Application</span></span>|<span data-ttu-id="d1c30-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1c30-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1c30-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1c30-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d1c30-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1c30-119">Request headers</span></span>
|<span data-ttu-id="d1c30-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1c30-120">Header</span></span>|<span data-ttu-id="d1c30-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d1c30-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1c30-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1c30-122">Authorization</span></span>|<span data-ttu-id="d1c30-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1c30-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1c30-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d1c30-124">Accept</span></span>|<span data-ttu-id="d1c30-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1c30-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1c30-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1c30-126">Request body</span></span>
<span data-ttu-id="d1c30-127">В тексте запроса добавьте представление объекта windows10EnrollmentCompletionPageConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1c30-127">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="d1c30-128">В следующей таблице приведены свойства, необходимые при создании windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d1c30-128">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="d1c30-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1c30-129">Property</span></span>|<span data-ttu-id="d1c30-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d1c30-130">Type</span></span>|<span data-ttu-id="d1c30-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d1c30-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1c30-132">id</span><span class="sxs-lookup"><span data-stu-id="d1c30-132">id</span></span>|<span data-ttu-id="d1c30-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d1c30-133">String</span></span>|<span data-ttu-id="d1c30-134">Идентификатор конфигурации страницы состояния регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1c30-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1c30-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d1c30-135">displayName</span></span>|<span data-ttu-id="d1c30-136">String</span><span class="sxs-lookup"><span data-stu-id="d1c30-136">String</span></span>|<span data-ttu-id="d1c30-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1c30-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1c30-138">description</span><span class="sxs-lookup"><span data-stu-id="d1c30-138">description</span></span>|<span data-ttu-id="d1c30-139">String</span><span class="sxs-lookup"><span data-stu-id="d1c30-139">String</span></span>|<span data-ttu-id="d1c30-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1c30-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1c30-141">priority</span><span class="sxs-lookup"><span data-stu-id="d1c30-141">priority</span></span>|<span data-ttu-id="d1c30-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d1c30-142">Int32</span></span>|<span data-ttu-id="d1c30-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1c30-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1c30-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1c30-144">createdDateTime</span></span>|<span data-ttu-id="d1c30-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1c30-145">DateTimeOffset</span></span>|<span data-ttu-id="d1c30-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1c30-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1c30-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1c30-147">lastModifiedDateTime</span></span>|<span data-ttu-id="d1c30-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1c30-148">DateTimeOffset</span></span>|<span data-ttu-id="d1c30-149">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1c30-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1c30-150">version</span><span class="sxs-lookup"><span data-stu-id="d1c30-150">version</span></span>|<span data-ttu-id="d1c30-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d1c30-151">Int32</span></span>|<span data-ttu-id="d1c30-152">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1c30-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d1c30-153">Шовинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="d1c30-153">showInstallationProgress</span></span>|<span data-ttu-id="d1c30-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1c30-154">Boolean</span></span>|<span data-ttu-id="d1c30-155">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="d1c30-155">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="d1c30-156">Блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="d1c30-156">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="d1c30-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1c30-157">Boolean</span></span>|<span data-ttu-id="d1c30-158">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="d1c30-158">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="d1c30-159">Алловдевицересетонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="d1c30-159">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="d1c30-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1c30-160">Boolean</span></span>|<span data-ttu-id="d1c30-161">Разрешение или блокировка сброса устройства при сбое установки</span><span class="sxs-lookup"><span data-stu-id="d1c30-161">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="d1c30-162">Алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="d1c30-162">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="d1c30-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1c30-163">Boolean</span></span>|<span data-ttu-id="d1c30-164">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="d1c30-164">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="d1c30-165">Кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="d1c30-165">customErrorMessage</span></span>|<span data-ttu-id="d1c30-166">String</span><span class="sxs-lookup"><span data-stu-id="d1c30-166">String</span></span>|<span data-ttu-id="d1c30-167">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="d1c30-167">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="d1c30-168">Инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="d1c30-168">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="d1c30-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d1c30-169">Int32</span></span>|<span data-ttu-id="d1c30-170">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="d1c30-170">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="d1c30-171">Алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="d1c30-171">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="d1c30-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1c30-172">Boolean</span></span>|<span data-ttu-id="d1c30-173">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="d1c30-173">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="d1c30-174">Селектедмобилеаппидс</span><span class="sxs-lookup"><span data-stu-id="d1c30-174">selectedMobileAppIds</span></span>|<span data-ttu-id="d1c30-175">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d1c30-175">String collection</span></span>|<span data-ttu-id="d1c30-176">Выбранные приложения для отслеживания состояния установки</span><span class="sxs-lookup"><span data-stu-id="d1c30-176">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="d1c30-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1c30-177">Response</span></span>
<span data-ttu-id="d1c30-178">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1c30-178">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1c30-179">Пример</span><span class="sxs-lookup"><span data-stu-id="d1c30-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1c30-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1c30-180">Request</span></span>
<span data-ttu-id="d1c30-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1c30-181">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1c30-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1c30-182">Response</span></span>
<span data-ttu-id="d1c30-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1c30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





