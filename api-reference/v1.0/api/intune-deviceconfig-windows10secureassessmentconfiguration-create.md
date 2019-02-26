---
title: Create windows10SecureAssessmentConfiguration
description: Создание объекта windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0e8b430023563ddb770b2cf7d4693814f01b4a7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252275"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="26a6d-103">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="26a6d-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="26a6d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26a6d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26a6d-105">Создание объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26a6d-105">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26a6d-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="26a6d-106">Prerequisites</span></span>
<span data-ttu-id="26a6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="26a6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="26a6d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26a6d-109">Permission type</span></span>|<span data-ttu-id="26a6d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26a6d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26a6d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26a6d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26a6d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26a6d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26a6d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26a6d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26a6d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a6d-114">Not supported.</span></span>|
|<span data-ttu-id="26a6d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26a6d-115">Application</span></span>|<span data-ttu-id="26a6d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a6d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26a6d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26a6d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="26a6d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26a6d-118">Request headers</span></span>
|<span data-ttu-id="26a6d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26a6d-119">Header</span></span>|<span data-ttu-id="26a6d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="26a6d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26a6d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="26a6d-121">Authorization</span></span>|<span data-ttu-id="26a6d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="26a6d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26a6d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="26a6d-123">Accept</span></span>|<span data-ttu-id="26a6d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="26a6d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26a6d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26a6d-125">Request body</span></span>
<span data-ttu-id="26a6d-126">В тексте запроса добавьте представление объекта windows10SecureAssessmentConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26a6d-126">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="26a6d-127">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="26a6d-127">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="26a6d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="26a6d-128">Property</span></span>|<span data-ttu-id="26a6d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="26a6d-129">Type</span></span>|<span data-ttu-id="26a6d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="26a6d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26a6d-131">id</span><span class="sxs-lookup"><span data-stu-id="26a6d-131">id</span></span>|<span data-ttu-id="26a6d-132">String</span><span class="sxs-lookup"><span data-stu-id="26a6d-132">String</span></span>|<span data-ttu-id="26a6d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="26a6d-133">Key of the entity.</span></span> <span data-ttu-id="26a6d-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26a6d-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a6d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26a6d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="26a6d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26a6d-136">DateTimeOffset</span></span>|<span data-ttu-id="26a6d-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="26a6d-137">DateTime the object was last modified.</span></span> <span data-ttu-id="26a6d-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26a6d-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a6d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26a6d-139">createdDateTime</span></span>|<span data-ttu-id="26a6d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26a6d-140">DateTimeOffset</span></span>|<span data-ttu-id="26a6d-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="26a6d-141">DateTime the object was created.</span></span> <span data-ttu-id="26a6d-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26a6d-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a6d-143">description</span><span class="sxs-lookup"><span data-stu-id="26a6d-143">description</span></span>|<span data-ttu-id="26a6d-144">Строка</span><span class="sxs-lookup"><span data-stu-id="26a6d-144">String</span></span>|<span data-ttu-id="26a6d-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="26a6d-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="26a6d-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26a6d-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a6d-147">displayName</span><span class="sxs-lookup"><span data-stu-id="26a6d-147">displayName</span></span>|<span data-ttu-id="26a6d-148">Строка</span><span class="sxs-lookup"><span data-stu-id="26a6d-148">String</span></span>|<span data-ttu-id="26a6d-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="26a6d-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="26a6d-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26a6d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a6d-151">version</span><span class="sxs-lookup"><span data-stu-id="26a6d-151">version</span></span>|<span data-ttu-id="26a6d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="26a6d-152">Int32</span></span>|<span data-ttu-id="26a6d-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="26a6d-153">Version of the device configuration.</span></span> <span data-ttu-id="26a6d-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26a6d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26a6d-155">launchUri</span><span class="sxs-lookup"><span data-stu-id="26a6d-155">launchUri</span></span>|<span data-ttu-id="26a6d-156">String</span><span class="sxs-lookup"><span data-stu-id="26a6d-156">String</span></span>|<span data-ttu-id="26a6d-157">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="26a6d-157">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="26a6d-158">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="26a6d-158">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="26a6d-159">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="26a6d-159">configurationAccount</span></span>|<span data-ttu-id="26a6d-160">String</span><span class="sxs-lookup"><span data-stu-id="26a6d-160">String</span></span>|<span data-ttu-id="26a6d-161">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="26a6d-161">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="26a6d-162">В качестве пользователя можно указать учетную запись домена (домен\пользователь), учетную запись AAD (имя_пользователя@клиент.com) или локальную учетную запись (имя_пользователя).</span><span class="sxs-lookup"><span data-stu-id="26a6d-162">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="26a6d-163">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="26a6d-163">allowPrinting</span></span>|<span data-ttu-id="26a6d-164">Логический</span><span class="sxs-lookup"><span data-stu-id="26a6d-164">Boolean</span></span>|<span data-ttu-id="26a6d-165">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="26a6d-165">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="26a6d-166">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="26a6d-166">allowScreenCapture</span></span>|<span data-ttu-id="26a6d-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a6d-167">Boolean</span></span>|<span data-ttu-id="26a6d-168">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="26a6d-168">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="26a6d-169">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="26a6d-169">allowTextSuggestion</span></span>|<span data-ttu-id="26a6d-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a6d-170">Boolean</span></span>|<span data-ttu-id="26a6d-171">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="26a6d-171">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="26a6d-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="26a6d-172">Response</span></span>
<span data-ttu-id="26a6d-173">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="26a6d-173">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26a6d-174">Пример</span><span class="sxs-lookup"><span data-stu-id="26a6d-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="26a6d-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="26a6d-175">Request</span></span>
<span data-ttu-id="26a6d-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26a6d-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26a6d-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="26a6d-177">Response</span></span>
<span data-ttu-id="26a6d-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="26a6d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



