---
title: Обновление windows10EnrollmentCompletionPageConfiguration
description: Обновление свойства объекта windows10EnrollmentCompletionPageConfiguration.
ms.openlocfilehash: b3566d7b476c17557bdfc15f8ff9d86763123ab2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080898"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="4bb48-103">Обновление windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="4bb48-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="4bb48-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4bb48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bb48-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4bb48-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4bb48-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bb48-107">Обновление свойства объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4bb48-107">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4bb48-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4bb48-108">Prerequisites</span></span>
<span data-ttu-id="4bb48-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bb48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bb48-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bb48-111">Permission type</span></span>|<span data-ttu-id="4bb48-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bb48-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bb48-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bb48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4bb48-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bb48-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4bb48-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bb48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bb48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb48-116">Not supported.</span></span>|
|<span data-ttu-id="4bb48-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bb48-117">Application</span></span>|<span data-ttu-id="4bb48-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb48-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bb48-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bb48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4bb48-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bb48-120">Request headers</span></span>
|<span data-ttu-id="4bb48-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bb48-121">Header</span></span>|<span data-ttu-id="4bb48-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4bb48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bb48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bb48-123">Authorization</span></span>|<span data-ttu-id="4bb48-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4bb48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bb48-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4bb48-125">Accept</span></span>|<span data-ttu-id="4bb48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4bb48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bb48-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bb48-127">Request body</span></span>
<span data-ttu-id="4bb48-128">В тексте запроса укажите представление JSON для объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4bb48-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="4bb48-129">В следующей таблице показаны свойства, которые необходимы для создания [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bb48-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="4bb48-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bb48-130">Property</span></span>|<span data-ttu-id="4bb48-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4bb48-131">Type</span></span>|<span data-ttu-id="4bb48-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb48-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bb48-133">id</span><span class="sxs-lookup"><span data-stu-id="4bb48-133">id</span></span>|<span data-ttu-id="4bb48-134">String</span><span class="sxs-lookup"><span data-stu-id="4bb48-134">String</span></span>|<span data-ttu-id="4bb48-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bb48-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4bb48-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4bb48-136">displayName</span></span>|<span data-ttu-id="4bb48-137">String</span><span class="sxs-lookup"><span data-stu-id="4bb48-137">String</span></span>|<span data-ttu-id="4bb48-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bb48-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4bb48-139">описание</span><span class="sxs-lookup"><span data-stu-id="4bb48-139">description</span></span>|<span data-ttu-id="4bb48-140">String</span><span class="sxs-lookup"><span data-stu-id="4bb48-140">String</span></span>|<span data-ttu-id="4bb48-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bb48-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4bb48-142">priority</span><span class="sxs-lookup"><span data-stu-id="4bb48-142">priority</span></span>|<span data-ttu-id="4bb48-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4bb48-143">Int32</span></span>|<span data-ttu-id="4bb48-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bb48-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4bb48-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4bb48-145">createdDateTime</span></span>|<span data-ttu-id="4bb48-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bb48-146">DateTimeOffset</span></span>|<span data-ttu-id="4bb48-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bb48-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4bb48-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4bb48-148">lastModifiedDateTime</span></span>|<span data-ttu-id="4bb48-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bb48-149">DateTimeOffset</span></span>|<span data-ttu-id="4bb48-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bb48-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4bb48-151">version</span><span class="sxs-lookup"><span data-stu-id="4bb48-151">version</span></span>|<span data-ttu-id="4bb48-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4bb48-152">Int32</span></span>|<span data-ttu-id="4bb48-153">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4bb48-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4bb48-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="4bb48-154">showInstallationProgress</span></span>|<span data-ttu-id="4bb48-155">Логический</span><span class="sxs-lookup"><span data-stu-id="4bb48-155">Boolean</span></span>|<span data-ttu-id="4bb48-156">Показать или скрыть выполнения установки для пользователей</span><span class="sxs-lookup"><span data-stu-id="4bb48-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="4bb48-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="4bb48-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="4bb48-158">Логический</span><span class="sxs-lookup"><span data-stu-id="4bb48-158">Boolean</span></span>|<span data-ttu-id="4bb48-159">Пользователь может повторно запустите программу установки на сбой установки</span><span class="sxs-lookup"><span data-stu-id="4bb48-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="4bb48-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="4bb48-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="4bb48-161">Логический</span><span class="sxs-lookup"><span data-stu-id="4bb48-161">Boolean</span></span>|<span data-ttu-id="4bb48-162">Разрешить или заблокировать устройство Сброс на сбой установки</span><span class="sxs-lookup"><span data-stu-id="4bb48-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="4bb48-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="4bb48-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="4bb48-164">Логический</span><span class="sxs-lookup"><span data-stu-id="4bb48-164">Boolean</span></span>|<span data-ttu-id="4bb48-165">Разрешить или заблокировать семейства журнала на сбой установки</span><span class="sxs-lookup"><span data-stu-id="4bb48-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="4bb48-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="4bb48-166">customErrorMessage</span></span>|<span data-ttu-id="4bb48-167">String</span><span class="sxs-lookup"><span data-stu-id="4bb48-167">String</span></span>|<span data-ttu-id="4bb48-168">Задать пользовательское сообщение об ошибке для отображения после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="4bb48-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="4bb48-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="4bb48-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="4bb48-170">Int32</span><span class="sxs-lookup"><span data-stu-id="4bb48-170">Int32</span></span>|<span data-ttu-id="4bb48-171">Задать время ожидания ход выполнения установки в минутах</span><span class="sxs-lookup"><span data-stu-id="4bb48-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="4bb48-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="4bb48-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="4bb48-173">Логический</span><span class="sxs-lookup"><span data-stu-id="4bb48-173">Boolean</span></span>|<span data-ttu-id="4bb48-174">Разрешает пользователю продолжить использование устройства на сбой установки</span><span class="sxs-lookup"><span data-stu-id="4bb48-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="4bb48-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="4bb48-175">selectedMobileAppIds</span></span>|<span data-ttu-id="4bb48-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4bb48-176">String collection</span></span>|<span data-ttu-id="4bb48-177">Для отслеживания состояния установки выбранных приложений</span><span class="sxs-lookup"><span data-stu-id="4bb48-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="4bb48-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bb48-178">Response</span></span>
<span data-ttu-id="4bb48-179">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4bb48-179">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bb48-180">Пример</span><span class="sxs-lookup"><span data-stu-id="4bb48-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="4bb48-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bb48-181">Request</span></span>
<span data-ttu-id="4bb48-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bb48-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 562

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="4bb48-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bb48-183">Response</span></span>
<span data-ttu-id="4bb48-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4bb48-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





