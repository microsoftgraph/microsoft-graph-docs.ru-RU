---
title: Обновление объекта windows10SecureAssessmentConfiguration
description: Обновление свойств объекта windows10SecureAssessmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cdac9951877087b6abafadd16acf52ccb5d5b56e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760456"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="f2ca8-103">Обновление объекта windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2ca8-103">Update windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="f2ca8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2ca8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2ca8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2ca8-106">Обновление свойств объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2ca8-106">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2ca8-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f2ca8-107">Prerequisites</span></span>
<span data-ttu-id="f2ca8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2ca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2ca8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2ca8-110">Permission type</span></span>|<span data-ttu-id="f2ca8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2ca8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2ca8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2ca8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2ca8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2ca8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2ca8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2ca8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2ca8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-115">Not supported.</span></span>|
|<span data-ttu-id="f2ca8-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f2ca8-116">Application</span></span>|<span data-ttu-id="f2ca8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2ca8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2ca8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2ca8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f2ca8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f2ca8-119">Request headers</span></span>
|<span data-ttu-id="f2ca8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2ca8-120">Header</span></span>|<span data-ttu-id="f2ca8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f2ca8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2ca8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2ca8-122">Authorization</span></span>|<span data-ttu-id="f2ca8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2ca8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f2ca8-124">Accept</span></span>|<span data-ttu-id="f2ca8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f2ca8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2ca8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2ca8-126">Request body</span></span>
<span data-ttu-id="f2ca8-127">В теле запроса добавьте представление объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-127">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="f2ca8-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2ca8-128">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="f2ca8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2ca8-129">Property</span></span>|<span data-ttu-id="f2ca8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f2ca8-130">Type</span></span>|<span data-ttu-id="f2ca8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f2ca8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2ca8-132">id</span><span class="sxs-lookup"><span data-stu-id="f2ca8-132">id</span></span>|<span data-ttu-id="f2ca8-133">String</span><span class="sxs-lookup"><span data-stu-id="f2ca8-133">String</span></span>|<span data-ttu-id="f2ca8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-134">Key of the entity.</span></span> <span data-ttu-id="f2ca8-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2ca8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ca8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2ca8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f2ca8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2ca8-137">DateTimeOffset</span></span>|<span data-ttu-id="f2ca8-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f2ca8-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2ca8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ca8-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2ca8-140">createdDateTime</span></span>|<span data-ttu-id="f2ca8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2ca8-141">DateTimeOffset</span></span>|<span data-ttu-id="f2ca8-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-142">DateTime the object was created.</span></span> <span data-ttu-id="f2ca8-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2ca8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ca8-144">description</span><span class="sxs-lookup"><span data-stu-id="f2ca8-144">description</span></span>|<span data-ttu-id="f2ca8-145">String</span><span class="sxs-lookup"><span data-stu-id="f2ca8-145">String</span></span>|<span data-ttu-id="f2ca8-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f2ca8-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2ca8-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ca8-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f2ca8-148">displayName</span></span>|<span data-ttu-id="f2ca8-149">String</span><span class="sxs-lookup"><span data-stu-id="f2ca8-149">String</span></span>|<span data-ttu-id="f2ca8-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f2ca8-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2ca8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ca8-152">version</span><span class="sxs-lookup"><span data-stu-id="f2ca8-152">version</span></span>|<span data-ttu-id="f2ca8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f2ca8-153">Int32</span></span>|<span data-ttu-id="f2ca8-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-154">Version of the device configuration.</span></span> <span data-ttu-id="f2ca8-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2ca8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ca8-156">launchUri</span><span class="sxs-lookup"><span data-stu-id="f2ca8-156">launchUri</span></span>|<span data-ttu-id="f2ca8-157">String</span><span class="sxs-lookup"><span data-stu-id="f2ca8-157">String</span></span>|<span data-ttu-id="f2ca8-158">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-158">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="f2ca8-159">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="f2ca8-159">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="f2ca8-160">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="f2ca8-160">configurationAccount</span></span>|<span data-ttu-id="f2ca8-161">String</span><span class="sxs-lookup"><span data-stu-id="f2ca8-161">String</span></span>|<span data-ttu-id="f2ca8-162">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-162">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="f2ca8-163">В качестве пользователя можно указать учетную запись домена (domen\polzovatel), учетную запись AAD (imya_polzovatelya@klient.com) или локальную учетную запись (имя пользователя).</span><span class="sxs-lookup"><span data-stu-id="f2ca8-163">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="f2ca8-164">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="f2ca8-164">allowPrinting</span></span>|<span data-ttu-id="f2ca8-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2ca8-165">Boolean</span></span>|<span data-ttu-id="f2ca8-166">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-166">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="f2ca8-167">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="f2ca8-167">allowScreenCapture</span></span>|<span data-ttu-id="f2ca8-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2ca8-168">Boolean</span></span>|<span data-ttu-id="f2ca8-169">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-169">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="f2ca8-170">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="f2ca8-170">allowTextSuggestion</span></span>|<span data-ttu-id="f2ca8-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2ca8-171">Boolean</span></span>|<span data-ttu-id="f2ca8-172">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-172">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="f2ca8-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2ca8-173">Response</span></span>
<span data-ttu-id="f2ca8-174">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-174">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2ca8-175">Пример</span><span class="sxs-lookup"><span data-stu-id="f2ca8-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2ca8-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2ca8-176">Request</span></span>
<span data-ttu-id="f2ca8-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="f2ca8-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2ca8-178">Response</span></span>
<span data-ttu-id="f2ca8-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2ca8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```




