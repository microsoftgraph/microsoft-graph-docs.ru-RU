---
title: Create windows10SecureAssessmentConfiguration
description: Создание объекта windows10SecureAssessmentConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58af4dd157691184dc7cf87c1942921d8716c348
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513981"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="52fa9-103">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="52fa9-103">Create windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="52fa9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52fa9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52fa9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52fa9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52fa9-106">Создание объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52fa9-106">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52fa9-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="52fa9-107">Prerequisites</span></span>
<span data-ttu-id="52fa9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52fa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52fa9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52fa9-110">Permission type</span></span>|<span data-ttu-id="52fa9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52fa9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52fa9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52fa9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52fa9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52fa9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52fa9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52fa9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52fa9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52fa9-115">Not supported.</span></span>|
|<span data-ttu-id="52fa9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52fa9-116">Application</span></span>|<span data-ttu-id="52fa9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52fa9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52fa9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52fa9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="52fa9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="52fa9-119">Request headers</span></span>
|<span data-ttu-id="52fa9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52fa9-120">Header</span></span>|<span data-ttu-id="52fa9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="52fa9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52fa9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52fa9-122">Authorization</span></span>|<span data-ttu-id="52fa9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52fa9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52fa9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="52fa9-124">Accept</span></span>|<span data-ttu-id="52fa9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52fa9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52fa9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52fa9-126">Request body</span></span>
<span data-ttu-id="52fa9-127">В тексте запроса добавьте представление объекта windows10SecureAssessmentConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52fa9-127">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="52fa9-128">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="52fa9-128">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="52fa9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="52fa9-129">Property</span></span>|<span data-ttu-id="52fa9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="52fa9-130">Type</span></span>|<span data-ttu-id="52fa9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="52fa9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52fa9-132">id</span><span class="sxs-lookup"><span data-stu-id="52fa9-132">id</span></span>|<span data-ttu-id="52fa9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="52fa9-133">String</span></span>|<span data-ttu-id="52fa9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="52fa9-134">Key of the entity.</span></span> <span data-ttu-id="52fa9-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52fa9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52fa9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52fa9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="52fa9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52fa9-137">DateTimeOffset</span></span>|<span data-ttu-id="52fa9-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="52fa9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="52fa9-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52fa9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52fa9-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52fa9-140">createdDateTime</span></span>|<span data-ttu-id="52fa9-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52fa9-141">DateTimeOffset</span></span>|<span data-ttu-id="52fa9-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="52fa9-142">DateTime the object was created.</span></span> <span data-ttu-id="52fa9-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52fa9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52fa9-144">description</span><span class="sxs-lookup"><span data-stu-id="52fa9-144">description</span></span>|<span data-ttu-id="52fa9-145">String</span><span class="sxs-lookup"><span data-stu-id="52fa9-145">String</span></span>|<span data-ttu-id="52fa9-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="52fa9-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="52fa9-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52fa9-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52fa9-148">displayName</span><span class="sxs-lookup"><span data-stu-id="52fa9-148">displayName</span></span>|<span data-ttu-id="52fa9-149">Строка</span><span class="sxs-lookup"><span data-stu-id="52fa9-149">String</span></span>|<span data-ttu-id="52fa9-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="52fa9-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="52fa9-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52fa9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52fa9-152">version</span><span class="sxs-lookup"><span data-stu-id="52fa9-152">version</span></span>|<span data-ttu-id="52fa9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="52fa9-153">Int32</span></span>|<span data-ttu-id="52fa9-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="52fa9-154">Version of the device configuration.</span></span> <span data-ttu-id="52fa9-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52fa9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52fa9-156">launchUri</span><span class="sxs-lookup"><span data-stu-id="52fa9-156">launchUri</span></span>|<span data-ttu-id="52fa9-157">Строка</span><span class="sxs-lookup"><span data-stu-id="52fa9-157">String</span></span>|<span data-ttu-id="52fa9-158">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="52fa9-158">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="52fa9-159">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="52fa9-159">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="52fa9-160">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="52fa9-160">configurationAccount</span></span>|<span data-ttu-id="52fa9-161">String</span><span class="sxs-lookup"><span data-stu-id="52fa9-161">String</span></span>|<span data-ttu-id="52fa9-162">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="52fa9-162">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="52fa9-163">В качестве пользователя можно указать учетную запись домена (domen\polzovatel), учетную запись AAD (imya_polzovatelya@klient.com) или локальную учетную запись (имя пользователя).</span><span class="sxs-lookup"><span data-stu-id="52fa9-163">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="52fa9-164">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="52fa9-164">allowPrinting</span></span>|<span data-ttu-id="52fa9-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="52fa9-165">Boolean</span></span>|<span data-ttu-id="52fa9-166">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="52fa9-166">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="52fa9-167">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="52fa9-167">allowScreenCapture</span></span>|<span data-ttu-id="52fa9-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="52fa9-168">Boolean</span></span>|<span data-ttu-id="52fa9-169">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="52fa9-169">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="52fa9-170">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="52fa9-170">allowTextSuggestion</span></span>|<span data-ttu-id="52fa9-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="52fa9-171">Boolean</span></span>|<span data-ttu-id="52fa9-172">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="52fa9-172">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="52fa9-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="52fa9-173">Response</span></span>
<span data-ttu-id="52fa9-174">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="52fa9-174">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52fa9-175">Пример</span><span class="sxs-lookup"><span data-stu-id="52fa9-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="52fa9-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="52fa9-176">Request</span></span>
<span data-ttu-id="52fa9-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52fa9-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="52fa9-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="52fa9-178">Response</span></span>
<span data-ttu-id="52fa9-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52fa9-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




