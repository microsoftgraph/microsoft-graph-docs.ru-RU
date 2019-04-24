---
title: Create windows10SecureAssessmentConfiguration
description: Создание объекта windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6864f7034d1009e5ddb1707d3f84dc463b15080b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32515822"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="344e7-103">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="344e7-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="344e7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="344e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="344e7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="344e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="344e7-106">Создание объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="344e7-106">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="344e7-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="344e7-107">Prerequisites</span></span>
<span data-ttu-id="344e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="344e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="344e7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="344e7-110">Permission type</span></span>|<span data-ttu-id="344e7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="344e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="344e7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="344e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="344e7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="344e7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="344e7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="344e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="344e7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="344e7-115">Not supported.</span></span>|
|<span data-ttu-id="344e7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="344e7-116">Application</span></span>|<span data-ttu-id="344e7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="344e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="344e7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="344e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="344e7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="344e7-119">Request headers</span></span>
|<span data-ttu-id="344e7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="344e7-120">Header</span></span>|<span data-ttu-id="344e7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="344e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="344e7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="344e7-122">Authorization</span></span>|<span data-ttu-id="344e7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="344e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="344e7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="344e7-124">Accept</span></span>|<span data-ttu-id="344e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="344e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="344e7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="344e7-126">Request body</span></span>
<span data-ttu-id="344e7-127">В тексте запроса добавьте представление объекта windows10SecureAssessmentConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="344e7-127">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="344e7-128">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="344e7-128">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="344e7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="344e7-129">Property</span></span>|<span data-ttu-id="344e7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="344e7-130">Type</span></span>|<span data-ttu-id="344e7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="344e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="344e7-132">id</span><span class="sxs-lookup"><span data-stu-id="344e7-132">id</span></span>|<span data-ttu-id="344e7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="344e7-133">String</span></span>|<span data-ttu-id="344e7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="344e7-134">Key of the entity.</span></span> <span data-ttu-id="344e7-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="344e7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="344e7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="344e7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="344e7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="344e7-137">DateTimeOffset</span></span>|<span data-ttu-id="344e7-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="344e7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="344e7-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="344e7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="344e7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="344e7-140">roleScopeTagIds</span></span>|<span data-ttu-id="344e7-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="344e7-141">String collection</span></span>|<span data-ttu-id="344e7-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="344e7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="344e7-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="344e7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="344e7-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="344e7-144">supportsScopeTags</span></span>|<span data-ttu-id="344e7-145">Логический</span><span class="sxs-lookup"><span data-stu-id="344e7-145">Boolean</span></span>|<span data-ttu-id="344e7-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="344e7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="344e7-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="344e7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="344e7-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="344e7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="344e7-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="344e7-149">This property is read-only.</span></span> <span data-ttu-id="344e7-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="344e7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="344e7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="344e7-151">createdDateTime</span></span>|<span data-ttu-id="344e7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="344e7-152">DateTimeOffset</span></span>|<span data-ttu-id="344e7-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="344e7-153">DateTime the object was created.</span></span> <span data-ttu-id="344e7-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="344e7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="344e7-155">description</span><span class="sxs-lookup"><span data-stu-id="344e7-155">description</span></span>|<span data-ttu-id="344e7-156">String</span><span class="sxs-lookup"><span data-stu-id="344e7-156">String</span></span>|<span data-ttu-id="344e7-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="344e7-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="344e7-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="344e7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="344e7-159">displayName</span><span class="sxs-lookup"><span data-stu-id="344e7-159">displayName</span></span>|<span data-ttu-id="344e7-160">Строка</span><span class="sxs-lookup"><span data-stu-id="344e7-160">String</span></span>|<span data-ttu-id="344e7-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="344e7-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="344e7-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="344e7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="344e7-163">version</span><span class="sxs-lookup"><span data-stu-id="344e7-163">version</span></span>|<span data-ttu-id="344e7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="344e7-164">Int32</span></span>|<span data-ttu-id="344e7-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="344e7-165">Version of the device configuration.</span></span> <span data-ttu-id="344e7-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="344e7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="344e7-167">launchUri</span><span class="sxs-lookup"><span data-stu-id="344e7-167">launchUri</span></span>|<span data-ttu-id="344e7-168">String</span><span class="sxs-lookup"><span data-stu-id="344e7-168">String</span></span>|<span data-ttu-id="344e7-169">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="344e7-169">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="344e7-170">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="344e7-170">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="344e7-171">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="344e7-171">configurationAccount</span></span>|<span data-ttu-id="344e7-172">String</span><span class="sxs-lookup"><span data-stu-id="344e7-172">String</span></span>|<span data-ttu-id="344e7-173">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="344e7-173">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="344e7-174">В качестве пользователя можно указать учетную запись домена (domen\polzovatel), учетную запись AAD (imya_polzovatelya@klient.com) или локальную учетную запись (имя пользователя).</span><span class="sxs-lookup"><span data-stu-id="344e7-174">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="344e7-175">Конфигуратионаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="344e7-175">configurationAccountType</span></span>|[<span data-ttu-id="344e7-176">Секуреассессментаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="344e7-176">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="344e7-177">Тип учетной записи, используемой в Конфигуратионаккаунт.</span><span class="sxs-lookup"><span data-stu-id="344e7-177">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="344e7-178">Возможные значения: `azureADAccount`, `domainAccount`, `localAccount`.</span><span class="sxs-lookup"><span data-stu-id="344e7-178">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="344e7-179">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="344e7-179">allowPrinting</span></span>|<span data-ttu-id="344e7-180">Логический</span><span class="sxs-lookup"><span data-stu-id="344e7-180">Boolean</span></span>|<span data-ttu-id="344e7-181">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="344e7-181">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="344e7-182">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="344e7-182">allowScreenCapture</span></span>|<span data-ttu-id="344e7-183">Логический</span><span class="sxs-lookup"><span data-stu-id="344e7-183">Boolean</span></span>|<span data-ttu-id="344e7-184">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="344e7-184">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="344e7-185">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="344e7-185">allowTextSuggestion</span></span>|<span data-ttu-id="344e7-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="344e7-186">Boolean</span></span>|<span data-ttu-id="344e7-187">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="344e7-187">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="344e7-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="344e7-188">Response</span></span>
<span data-ttu-id="344e7-189">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="344e7-189">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="344e7-190">Пример</span><span class="sxs-lookup"><span data-stu-id="344e7-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="344e7-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="344e7-191">Request</span></span>
<span data-ttu-id="344e7-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="344e7-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 499

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="344e7-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="344e7-193">Response</span></span>
<span data-ttu-id="344e7-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="344e7-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```





