---
title: Создание windows10EnrollmentCompletionPageConfiguration
description: Создание нового объекта windows10EnrollmentCompletionPageConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4e7797ac1cd3ca46724c046e43bfa1fa1649ebb7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411360"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="23673-103">Создание windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="23673-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="23673-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23673-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23673-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23673-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23673-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23673-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23673-107">Создание нового объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="23673-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23673-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="23673-108">Prerequisites</span></span>
<span data-ttu-id="23673-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="23673-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="23673-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23673-111">Permission type</span></span>|<span data-ttu-id="23673-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="23673-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23673-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23673-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23673-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23673-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="23673-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23673-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23673-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23673-116">Not supported.</span></span>|
|<span data-ttu-id="23673-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23673-117">Application</span></span>|<span data-ttu-id="23673-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23673-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23673-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23673-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="23673-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23673-120">Request headers</span></span>
|<span data-ttu-id="23673-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23673-121">Header</span></span>|<span data-ttu-id="23673-122">Значение</span><span class="sxs-lookup"><span data-stu-id="23673-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23673-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23673-123">Authorization</span></span>|<span data-ttu-id="23673-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="23673-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23673-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23673-125">Accept</span></span>|<span data-ttu-id="23673-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23673-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23673-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23673-127">Request body</span></span>
<span data-ttu-id="23673-128">В тексте запроса укажите представление JSON для объекта windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="23673-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="23673-129">В следующей таблице показаны свойства, которые необходимы для создания windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="23673-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="23673-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="23673-130">Property</span></span>|<span data-ttu-id="23673-131">Тип</span><span class="sxs-lookup"><span data-stu-id="23673-131">Type</span></span>|<span data-ttu-id="23673-132">Описание</span><span class="sxs-lookup"><span data-stu-id="23673-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23673-133">id</span><span class="sxs-lookup"><span data-stu-id="23673-133">id</span></span>|<span data-ttu-id="23673-134">String</span><span class="sxs-lookup"><span data-stu-id="23673-134">String</span></span>|<span data-ttu-id="23673-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23673-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="23673-136">displayName</span><span class="sxs-lookup"><span data-stu-id="23673-136">displayName</span></span>|<span data-ttu-id="23673-137">String</span><span class="sxs-lookup"><span data-stu-id="23673-137">String</span></span>|<span data-ttu-id="23673-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23673-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="23673-139">description</span><span class="sxs-lookup"><span data-stu-id="23673-139">description</span></span>|<span data-ttu-id="23673-140">String</span><span class="sxs-lookup"><span data-stu-id="23673-140">String</span></span>|<span data-ttu-id="23673-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23673-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="23673-142">priority</span><span class="sxs-lookup"><span data-stu-id="23673-142">priority</span></span>|<span data-ttu-id="23673-143">Int32</span><span class="sxs-lookup"><span data-stu-id="23673-143">Int32</span></span>|<span data-ttu-id="23673-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23673-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="23673-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23673-145">createdDateTime</span></span>|<span data-ttu-id="23673-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23673-146">DateTimeOffset</span></span>|<span data-ttu-id="23673-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23673-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="23673-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23673-148">lastModifiedDateTime</span></span>|<span data-ttu-id="23673-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23673-149">DateTimeOffset</span></span>|<span data-ttu-id="23673-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23673-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="23673-151">version</span><span class="sxs-lookup"><span data-stu-id="23673-151">version</span></span>|<span data-ttu-id="23673-152">Int32</span><span class="sxs-lookup"><span data-stu-id="23673-152">Int32</span></span>|<span data-ttu-id="23673-153">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23673-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="23673-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="23673-154">showInstallationProgress</span></span>|<span data-ttu-id="23673-155">Логический</span><span class="sxs-lookup"><span data-stu-id="23673-155">Boolean</span></span>|<span data-ttu-id="23673-156">Показать или скрыть выполнения установки для пользователей</span><span class="sxs-lookup"><span data-stu-id="23673-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="23673-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="23673-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="23673-158">Логический</span><span class="sxs-lookup"><span data-stu-id="23673-158">Boolean</span></span>|<span data-ttu-id="23673-159">Пользователь может повторно запустите программу установки на сбой установки</span><span class="sxs-lookup"><span data-stu-id="23673-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="23673-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="23673-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="23673-161">Логический</span><span class="sxs-lookup"><span data-stu-id="23673-161">Boolean</span></span>|<span data-ttu-id="23673-162">Разрешить или заблокировать устройство Сброс на сбой установки</span><span class="sxs-lookup"><span data-stu-id="23673-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="23673-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="23673-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="23673-164">Логический</span><span class="sxs-lookup"><span data-stu-id="23673-164">Boolean</span></span>|<span data-ttu-id="23673-165">Разрешить или заблокировать семейства журнала на сбой установки</span><span class="sxs-lookup"><span data-stu-id="23673-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="23673-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="23673-166">customErrorMessage</span></span>|<span data-ttu-id="23673-167">String</span><span class="sxs-lookup"><span data-stu-id="23673-167">String</span></span>|<span data-ttu-id="23673-168">Задать пользовательское сообщение об ошибке для отображения после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="23673-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="23673-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="23673-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="23673-170">Int32</span><span class="sxs-lookup"><span data-stu-id="23673-170">Int32</span></span>|<span data-ttu-id="23673-171">Задать время ожидания ход выполнения установки в минутах</span><span class="sxs-lookup"><span data-stu-id="23673-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="23673-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="23673-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="23673-173">Логический</span><span class="sxs-lookup"><span data-stu-id="23673-173">Boolean</span></span>|<span data-ttu-id="23673-174">Разрешает пользователю продолжить использование устройства на сбой установки</span><span class="sxs-lookup"><span data-stu-id="23673-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="23673-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="23673-175">selectedMobileAppIds</span></span>|<span data-ttu-id="23673-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="23673-176">String collection</span></span>|<span data-ttu-id="23673-177">Для отслеживания состояния установки выбранных приложений</span><span class="sxs-lookup"><span data-stu-id="23673-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="23673-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="23673-178">Response</span></span>
<span data-ttu-id="23673-179">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="23673-179">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23673-180">Пример</span><span class="sxs-lookup"><span data-stu-id="23673-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="23673-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="23673-181">Request</span></span>
<span data-ttu-id="23673-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23673-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="23673-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="23673-183">Response</span></span>
<span data-ttu-id="23673-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="23673-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




