---
title: Обновление windows10EnrollmentCompletionPageConfiguration
description: Обновление свойства объекта windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9cc7d2cff8563d5e720e23c7f49bd88c42f47ec3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870085"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="b20aa-103">Обновление windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="b20aa-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="b20aa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b20aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b20aa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b20aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b20aa-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b20aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b20aa-107">Обновление свойства объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b20aa-107">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b20aa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b20aa-108">Prerequisites</span></span>
<span data-ttu-id="b20aa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b20aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b20aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b20aa-111">Permission type</span></span>|<span data-ttu-id="b20aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b20aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b20aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b20aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b20aa-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b20aa-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b20aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b20aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b20aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b20aa-116">Not supported.</span></span>|
|<span data-ttu-id="b20aa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b20aa-117">Application</span></span>|<span data-ttu-id="b20aa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b20aa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b20aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b20aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b20aa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b20aa-120">Request headers</span></span>
|<span data-ttu-id="b20aa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b20aa-121">Header</span></span>|<span data-ttu-id="b20aa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b20aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b20aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b20aa-123">Authorization</span></span>|<span data-ttu-id="b20aa-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b20aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b20aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b20aa-125">Accept</span></span>|<span data-ttu-id="b20aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b20aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b20aa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b20aa-127">Request body</span></span>
<span data-ttu-id="b20aa-128">В тексте запроса укажите представление JSON для объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b20aa-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="b20aa-129">В следующей таблице показаны свойства, которые необходимы для создания [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b20aa-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="b20aa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b20aa-130">Property</span></span>|<span data-ttu-id="b20aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b20aa-131">Type</span></span>|<span data-ttu-id="b20aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b20aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b20aa-133">id</span><span class="sxs-lookup"><span data-stu-id="b20aa-133">id</span></span>|<span data-ttu-id="b20aa-134">String</span><span class="sxs-lookup"><span data-stu-id="b20aa-134">String</span></span>|<span data-ttu-id="b20aa-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b20aa-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b20aa-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b20aa-136">displayName</span></span>|<span data-ttu-id="b20aa-137">String</span><span class="sxs-lookup"><span data-stu-id="b20aa-137">String</span></span>|<span data-ttu-id="b20aa-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b20aa-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b20aa-139">описание</span><span class="sxs-lookup"><span data-stu-id="b20aa-139">description</span></span>|<span data-ttu-id="b20aa-140">String</span><span class="sxs-lookup"><span data-stu-id="b20aa-140">String</span></span>|<span data-ttu-id="b20aa-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b20aa-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b20aa-142">priority</span><span class="sxs-lookup"><span data-stu-id="b20aa-142">priority</span></span>|<span data-ttu-id="b20aa-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b20aa-143">Int32</span></span>|<span data-ttu-id="b20aa-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b20aa-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b20aa-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b20aa-145">createdDateTime</span></span>|<span data-ttu-id="b20aa-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b20aa-146">DateTimeOffset</span></span>|<span data-ttu-id="b20aa-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b20aa-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b20aa-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b20aa-148">lastModifiedDateTime</span></span>|<span data-ttu-id="b20aa-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b20aa-149">DateTimeOffset</span></span>|<span data-ttu-id="b20aa-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b20aa-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b20aa-151">version</span><span class="sxs-lookup"><span data-stu-id="b20aa-151">version</span></span>|<span data-ttu-id="b20aa-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b20aa-152">Int32</span></span>|<span data-ttu-id="b20aa-153">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b20aa-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b20aa-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="b20aa-154">showInstallationProgress</span></span>|<span data-ttu-id="b20aa-155">Логический</span><span class="sxs-lookup"><span data-stu-id="b20aa-155">Boolean</span></span>|<span data-ttu-id="b20aa-156">Показать или скрыть выполнения установки для пользователей</span><span class="sxs-lookup"><span data-stu-id="b20aa-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="b20aa-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="b20aa-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="b20aa-158">Логический</span><span class="sxs-lookup"><span data-stu-id="b20aa-158">Boolean</span></span>|<span data-ttu-id="b20aa-159">Пользователь может повторно запустите программу установки на сбой установки</span><span class="sxs-lookup"><span data-stu-id="b20aa-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="b20aa-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="b20aa-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="b20aa-161">Логический</span><span class="sxs-lookup"><span data-stu-id="b20aa-161">Boolean</span></span>|<span data-ttu-id="b20aa-162">Разрешить или заблокировать устройство Сброс на сбой установки</span><span class="sxs-lookup"><span data-stu-id="b20aa-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="b20aa-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="b20aa-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="b20aa-164">Логический</span><span class="sxs-lookup"><span data-stu-id="b20aa-164">Boolean</span></span>|<span data-ttu-id="b20aa-165">Разрешить или заблокировать семейства журнала на сбой установки</span><span class="sxs-lookup"><span data-stu-id="b20aa-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="b20aa-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="b20aa-166">customErrorMessage</span></span>|<span data-ttu-id="b20aa-167">Строка</span><span class="sxs-lookup"><span data-stu-id="b20aa-167">String</span></span>|<span data-ttu-id="b20aa-168">Задать пользовательское сообщение об ошибке для отображения после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="b20aa-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="b20aa-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b20aa-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="b20aa-170">Int32</span><span class="sxs-lookup"><span data-stu-id="b20aa-170">Int32</span></span>|<span data-ttu-id="b20aa-171">Задать время ожидания ход выполнения установки в минутах</span><span class="sxs-lookup"><span data-stu-id="b20aa-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="b20aa-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="b20aa-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="b20aa-173">Логический</span><span class="sxs-lookup"><span data-stu-id="b20aa-173">Boolean</span></span>|<span data-ttu-id="b20aa-174">Разрешает пользователю продолжить использование устройства на сбой установки</span><span class="sxs-lookup"><span data-stu-id="b20aa-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="b20aa-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="b20aa-175">selectedMobileAppIds</span></span>|<span data-ttu-id="b20aa-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b20aa-176">String collection</span></span>|<span data-ttu-id="b20aa-177">Для отслеживания состояния установки выбранных приложений</span><span class="sxs-lookup"><span data-stu-id="b20aa-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="b20aa-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="b20aa-178">Response</span></span>
<span data-ttu-id="b20aa-179">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b20aa-179">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b20aa-180">Пример</span><span class="sxs-lookup"><span data-stu-id="b20aa-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="b20aa-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="b20aa-181">Request</span></span>
<span data-ttu-id="b20aa-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b20aa-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b20aa-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="b20aa-183">Response</span></span>
<span data-ttu-id="b20aa-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b20aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





