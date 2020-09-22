---
title: Create windows10SecureAssessmentConfiguration
description: Создание объекта windows10SecureAssessmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d4b32f8327c1c307d37d145974e5ab6ddc312395
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063375"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="8eb29-103">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="8eb29-103">Create windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="8eb29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eb29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8eb29-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8eb29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eb29-106">Создание объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb29-106">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8eb29-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8eb29-107">Prerequisites</span></span>
<span data-ttu-id="8eb29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eb29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eb29-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8eb29-110">Permission type</span></span>|<span data-ttu-id="8eb29-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8eb29-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8eb29-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8eb29-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8eb29-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb29-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8eb29-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8eb29-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8eb29-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eb29-115">Not supported.</span></span>|
|<span data-ttu-id="8eb29-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8eb29-116">Application</span></span>|<span data-ttu-id="8eb29-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eb29-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8eb29-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8eb29-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8eb29-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8eb29-119">Request headers</span></span>
|<span data-ttu-id="8eb29-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8eb29-120">Header</span></span>|<span data-ttu-id="8eb29-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8eb29-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8eb29-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eb29-122">Authorization</span></span>|<span data-ttu-id="8eb29-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8eb29-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8eb29-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8eb29-124">Accept</span></span>|<span data-ttu-id="8eb29-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8eb29-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eb29-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8eb29-126">Request body</span></span>
<span data-ttu-id="8eb29-127">В тексте запроса добавьте представление объекта windows10SecureAssessmentConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8eb29-127">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="8eb29-128">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8eb29-128">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="8eb29-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8eb29-129">Property</span></span>|<span data-ttu-id="8eb29-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8eb29-130">Type</span></span>|<span data-ttu-id="8eb29-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb29-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eb29-132">id</span><span class="sxs-lookup"><span data-stu-id="8eb29-132">id</span></span>|<span data-ttu-id="8eb29-133">String</span><span class="sxs-lookup"><span data-stu-id="8eb29-133">String</span></span>|<span data-ttu-id="8eb29-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8eb29-134">Key of the entity.</span></span> <span data-ttu-id="8eb29-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb29-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb29-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8eb29-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8eb29-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eb29-137">DateTimeOffset</span></span>|<span data-ttu-id="8eb29-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8eb29-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8eb29-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb29-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb29-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8eb29-140">createdDateTime</span></span>|<span data-ttu-id="8eb29-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eb29-141">DateTimeOffset</span></span>|<span data-ttu-id="8eb29-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8eb29-142">DateTime the object was created.</span></span> <span data-ttu-id="8eb29-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb29-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb29-144">description</span><span class="sxs-lookup"><span data-stu-id="8eb29-144">description</span></span>|<span data-ttu-id="8eb29-145">String</span><span class="sxs-lookup"><span data-stu-id="8eb29-145">String</span></span>|<span data-ttu-id="8eb29-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8eb29-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8eb29-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb29-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb29-148">displayName</span><span class="sxs-lookup"><span data-stu-id="8eb29-148">displayName</span></span>|<span data-ttu-id="8eb29-149">String</span><span class="sxs-lookup"><span data-stu-id="8eb29-149">String</span></span>|<span data-ttu-id="8eb29-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8eb29-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8eb29-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb29-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb29-152">version</span><span class="sxs-lookup"><span data-stu-id="8eb29-152">version</span></span>|<span data-ttu-id="8eb29-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8eb29-153">Int32</span></span>|<span data-ttu-id="8eb29-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8eb29-154">Version of the device configuration.</span></span> <span data-ttu-id="8eb29-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb29-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8eb29-156">launchUri</span><span class="sxs-lookup"><span data-stu-id="8eb29-156">launchUri</span></span>|<span data-ttu-id="8eb29-157">String</span><span class="sxs-lookup"><span data-stu-id="8eb29-157">String</span></span>|<span data-ttu-id="8eb29-158">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="8eb29-158">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="8eb29-159">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="8eb29-159">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="8eb29-160">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="8eb29-160">configurationAccount</span></span>|<span data-ttu-id="8eb29-161">String</span><span class="sxs-lookup"><span data-stu-id="8eb29-161">String</span></span>|<span data-ttu-id="8eb29-162">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="8eb29-162">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="8eb29-163">В качестве пользователя можно указать учетную запись домена (domen\polzovatel), учетную запись AAD (imya_polzovatelya@klient.com) или локальную учетную запись (имя пользователя).</span><span class="sxs-lookup"><span data-stu-id="8eb29-163">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="8eb29-164">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="8eb29-164">allowPrinting</span></span>|<span data-ttu-id="8eb29-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eb29-165">Boolean</span></span>|<span data-ttu-id="8eb29-166">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="8eb29-166">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="8eb29-167">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="8eb29-167">allowScreenCapture</span></span>|<span data-ttu-id="8eb29-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eb29-168">Boolean</span></span>|<span data-ttu-id="8eb29-169">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="8eb29-169">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="8eb29-170">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="8eb29-170">allowTextSuggestion</span></span>|<span data-ttu-id="8eb29-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="8eb29-171">Boolean</span></span>|<span data-ttu-id="8eb29-172">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="8eb29-172">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="8eb29-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="8eb29-173">Response</span></span>
<span data-ttu-id="8eb29-174">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8eb29-174">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eb29-175">Пример</span><span class="sxs-lookup"><span data-stu-id="8eb29-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="8eb29-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="8eb29-176">Request</span></span>
<span data-ttu-id="8eb29-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8eb29-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="8eb29-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="8eb29-178">Response</span></span>
<span data-ttu-id="8eb29-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8eb29-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









