---
title: Создание windows10EnrollmentCompletionPageConfiguration
description: Создание нового объекта windows10EnrollmentCompletionPageConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d64ca5e5df475368e9b4848f57141884df5dd86
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984496"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="34f0e-103">Создание windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="34f0e-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="34f0e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34f0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34f0e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34f0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34f0e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="34f0e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34f0e-107">Создание нового объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="34f0e-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34f0e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="34f0e-108">Prerequisites</span></span>
<span data-ttu-id="34f0e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34f0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34f0e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34f0e-111">Permission type</span></span>|<span data-ttu-id="34f0e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34f0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34f0e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34f0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34f0e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34f0e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="34f0e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34f0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34f0e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34f0e-116">Not supported.</span></span>|
|<span data-ttu-id="34f0e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34f0e-117">Application</span></span>|<span data-ttu-id="34f0e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34f0e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34f0e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34f0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="34f0e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34f0e-120">Request headers</span></span>
|<span data-ttu-id="34f0e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34f0e-121">Header</span></span>|<span data-ttu-id="34f0e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="34f0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34f0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34f0e-123">Authorization</span></span>|<span data-ttu-id="34f0e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="34f0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34f0e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="34f0e-125">Accept</span></span>|<span data-ttu-id="34f0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34f0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34f0e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="34f0e-127">Request body</span></span>
<span data-ttu-id="34f0e-128">В тексте запроса укажите представление JSON для объекта windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="34f0e-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="34f0e-129">В следующей таблице показаны свойства, которые необходимы для создания windows10EnrollmentCompletionPageConfiguration.</span><span class="sxs-lookup"><span data-stu-id="34f0e-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="34f0e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="34f0e-130">Property</span></span>|<span data-ttu-id="34f0e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="34f0e-131">Type</span></span>|<span data-ttu-id="34f0e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="34f0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34f0e-133">id</span><span class="sxs-lookup"><span data-stu-id="34f0e-133">id</span></span>|<span data-ttu-id="34f0e-134">String</span><span class="sxs-lookup"><span data-stu-id="34f0e-134">String</span></span>|<span data-ttu-id="34f0e-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34f0e-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="34f0e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="34f0e-136">displayName</span></span>|<span data-ttu-id="34f0e-137">String</span><span class="sxs-lookup"><span data-stu-id="34f0e-137">String</span></span>|<span data-ttu-id="34f0e-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34f0e-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="34f0e-139">описание</span><span class="sxs-lookup"><span data-stu-id="34f0e-139">description</span></span>|<span data-ttu-id="34f0e-140">String</span><span class="sxs-lookup"><span data-stu-id="34f0e-140">String</span></span>|<span data-ttu-id="34f0e-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34f0e-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="34f0e-142">priority</span><span class="sxs-lookup"><span data-stu-id="34f0e-142">priority</span></span>|<span data-ttu-id="34f0e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="34f0e-143">Int32</span></span>|<span data-ttu-id="34f0e-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34f0e-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="34f0e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34f0e-145">createdDateTime</span></span>|<span data-ttu-id="34f0e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34f0e-146">DateTimeOffset</span></span>|<span data-ttu-id="34f0e-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34f0e-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="34f0e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34f0e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="34f0e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34f0e-149">DateTimeOffset</span></span>|<span data-ttu-id="34f0e-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34f0e-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="34f0e-151">version</span><span class="sxs-lookup"><span data-stu-id="34f0e-151">version</span></span>|<span data-ttu-id="34f0e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="34f0e-152">Int32</span></span>|<span data-ttu-id="34f0e-153">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34f0e-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="34f0e-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="34f0e-154">showInstallationProgress</span></span>|<span data-ttu-id="34f0e-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="34f0e-155">Boolean</span></span>|<span data-ttu-id="34f0e-156">Показать или скрыть выполнения установки для пользователей</span><span class="sxs-lookup"><span data-stu-id="34f0e-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="34f0e-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="34f0e-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="34f0e-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="34f0e-158">Boolean</span></span>|<span data-ttu-id="34f0e-159">Пользователь может повторно запустите программу установки на сбой установки</span><span class="sxs-lookup"><span data-stu-id="34f0e-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="34f0e-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="34f0e-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="34f0e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="34f0e-161">Boolean</span></span>|<span data-ttu-id="34f0e-162">Разрешить или заблокировать устройство Сброс на сбой установки</span><span class="sxs-lookup"><span data-stu-id="34f0e-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="34f0e-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="34f0e-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="34f0e-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="34f0e-164">Boolean</span></span>|<span data-ttu-id="34f0e-165">Разрешить или заблокировать семейства журнала на сбой установки</span><span class="sxs-lookup"><span data-stu-id="34f0e-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="34f0e-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="34f0e-166">customErrorMessage</span></span>|<span data-ttu-id="34f0e-167">String</span><span class="sxs-lookup"><span data-stu-id="34f0e-167">String</span></span>|<span data-ttu-id="34f0e-168">Задать пользовательское сообщение об ошибке для отображения после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="34f0e-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="34f0e-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="34f0e-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="34f0e-170">Int32</span><span class="sxs-lookup"><span data-stu-id="34f0e-170">Int32</span></span>|<span data-ttu-id="34f0e-171">Задать время ожидания ход выполнения установки в минутах</span><span class="sxs-lookup"><span data-stu-id="34f0e-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="34f0e-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="34f0e-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="34f0e-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="34f0e-173">Boolean</span></span>|<span data-ttu-id="34f0e-174">Разрешает пользователю продолжить использование устройства на сбой установки</span><span class="sxs-lookup"><span data-stu-id="34f0e-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="34f0e-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="34f0e-175">selectedMobileAppIds</span></span>|<span data-ttu-id="34f0e-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="34f0e-176">String collection</span></span>|<span data-ttu-id="34f0e-177">Для отслеживания состояния установки выбранных приложений</span><span class="sxs-lookup"><span data-stu-id="34f0e-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="34f0e-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="34f0e-178">Response</span></span>
<span data-ttu-id="34f0e-179">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="34f0e-179">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34f0e-180">Пример</span><span class="sxs-lookup"><span data-stu-id="34f0e-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="34f0e-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="34f0e-181">Request</span></span>
<span data-ttu-id="34f0e-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34f0e-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 647

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
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

### <a name="response"></a><span data-ttu-id="34f0e-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="34f0e-183">Response</span></span>
<span data-ttu-id="34f0e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="34f0e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





