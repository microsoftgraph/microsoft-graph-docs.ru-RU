---
title: Обновление объекта windows10SecureAssessmentConfiguration
description: Обновление свойств объекта windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ebff2b3c12e605727fd0eeff5f953713d5303b8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984466"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="16bac-103">Обновление объекта windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="16bac-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="16bac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16bac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16bac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16bac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16bac-106">Обновление свойств объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16bac-106">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16bac-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="16bac-107">Prerequisites</span></span>
<span data-ttu-id="16bac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16bac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16bac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16bac-110">Permission type</span></span>|<span data-ttu-id="16bac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16bac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16bac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16bac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16bac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16bac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16bac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16bac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16bac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16bac-115">Not supported.</span></span>|
|<span data-ttu-id="16bac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16bac-116">Application</span></span>|<span data-ttu-id="16bac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16bac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16bac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16bac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="16bac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16bac-119">Request headers</span></span>
|<span data-ttu-id="16bac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16bac-120">Header</span></span>|<span data-ttu-id="16bac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="16bac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16bac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16bac-122">Authorization</span></span>|<span data-ttu-id="16bac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16bac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16bac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="16bac-124">Accept</span></span>|<span data-ttu-id="16bac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16bac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16bac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16bac-126">Request body</span></span>
<span data-ttu-id="16bac-127">В теле запроса добавьте представление объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16bac-127">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="16bac-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16bac-128">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="16bac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="16bac-129">Property</span></span>|<span data-ttu-id="16bac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="16bac-130">Type</span></span>|<span data-ttu-id="16bac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="16bac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16bac-132">id</span><span class="sxs-lookup"><span data-stu-id="16bac-132">id</span></span>|<span data-ttu-id="16bac-133">Строка</span><span class="sxs-lookup"><span data-stu-id="16bac-133">String</span></span>|<span data-ttu-id="16bac-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="16bac-134">Key of the entity.</span></span> <span data-ttu-id="16bac-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16bac-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16bac-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16bac-136">lastModifiedDateTime</span></span>|<span data-ttu-id="16bac-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16bac-137">DateTimeOffset</span></span>|<span data-ttu-id="16bac-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="16bac-138">DateTime the object was last modified.</span></span> <span data-ttu-id="16bac-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16bac-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16bac-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16bac-140">roleScopeTagIds</span></span>|<span data-ttu-id="16bac-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="16bac-141">String collection</span></span>|<span data-ttu-id="16bac-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="16bac-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="16bac-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16bac-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16bac-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="16bac-144">supportsScopeTags</span></span>|<span data-ttu-id="16bac-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="16bac-145">Boolean</span></span>|<span data-ttu-id="16bac-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="16bac-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="16bac-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="16bac-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="16bac-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="16bac-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="16bac-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16bac-149">This property is read-only.</span></span> <span data-ttu-id="16bac-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16bac-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16bac-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16bac-151">createdDateTime</span></span>|<span data-ttu-id="16bac-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16bac-152">DateTimeOffset</span></span>|<span data-ttu-id="16bac-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="16bac-153">DateTime the object was created.</span></span> <span data-ttu-id="16bac-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16bac-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16bac-155">description</span><span class="sxs-lookup"><span data-stu-id="16bac-155">description</span></span>|<span data-ttu-id="16bac-156">String</span><span class="sxs-lookup"><span data-stu-id="16bac-156">String</span></span>|<span data-ttu-id="16bac-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="16bac-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="16bac-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16bac-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16bac-159">displayName</span><span class="sxs-lookup"><span data-stu-id="16bac-159">displayName</span></span>|<span data-ttu-id="16bac-160">Строка</span><span class="sxs-lookup"><span data-stu-id="16bac-160">String</span></span>|<span data-ttu-id="16bac-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="16bac-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="16bac-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16bac-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16bac-163">version</span><span class="sxs-lookup"><span data-stu-id="16bac-163">version</span></span>|<span data-ttu-id="16bac-164">Int32</span><span class="sxs-lookup"><span data-stu-id="16bac-164">Int32</span></span>|<span data-ttu-id="16bac-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="16bac-165">Version of the device configuration.</span></span> <span data-ttu-id="16bac-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16bac-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16bac-167">launchUri</span><span class="sxs-lookup"><span data-stu-id="16bac-167">launchUri</span></span>|<span data-ttu-id="16bac-168">String</span><span class="sxs-lookup"><span data-stu-id="16bac-168">String</span></span>|<span data-ttu-id="16bac-169">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="16bac-169">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="16bac-170">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="16bac-170">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="16bac-171">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="16bac-171">configurationAccount</span></span>|<span data-ttu-id="16bac-172">String</span><span class="sxs-lookup"><span data-stu-id="16bac-172">String</span></span>|<span data-ttu-id="16bac-173">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="16bac-173">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="16bac-174">В качестве пользователя можно указать учетную запись домена (domen\polzovatel), учетную запись AAD (imya_polzovatelya@klient.com) или локальную учетную запись (имя пользователя).</span><span class="sxs-lookup"><span data-stu-id="16bac-174">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="16bac-175">Конфигуратионаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="16bac-175">configurationAccountType</span></span>|[<span data-ttu-id="16bac-176">Секуреассессментаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="16bac-176">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="16bac-177">Тип учетной записи, используемой в Конфигуратионаккаунт.</span><span class="sxs-lookup"><span data-stu-id="16bac-177">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="16bac-178">Возможные значения: `azureADAccount`, `domainAccount`, `localAccount`.</span><span class="sxs-lookup"><span data-stu-id="16bac-178">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="16bac-179">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="16bac-179">allowPrinting</span></span>|<span data-ttu-id="16bac-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="16bac-180">Boolean</span></span>|<span data-ttu-id="16bac-181">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="16bac-181">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="16bac-182">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="16bac-182">allowScreenCapture</span></span>|<span data-ttu-id="16bac-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="16bac-183">Boolean</span></span>|<span data-ttu-id="16bac-184">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="16bac-184">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="16bac-185">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="16bac-185">allowTextSuggestion</span></span>|<span data-ttu-id="16bac-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="16bac-186">Boolean</span></span>|<span data-ttu-id="16bac-187">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="16bac-187">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="16bac-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="16bac-188">Response</span></span>
<span data-ttu-id="16bac-189">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="16bac-189">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16bac-190">Пример</span><span class="sxs-lookup"><span data-stu-id="16bac-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="16bac-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="16bac-191">Request</span></span>
<span data-ttu-id="16bac-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16bac-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="16bac-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="16bac-193">Response</span></span>
<span data-ttu-id="16bac-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16bac-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




