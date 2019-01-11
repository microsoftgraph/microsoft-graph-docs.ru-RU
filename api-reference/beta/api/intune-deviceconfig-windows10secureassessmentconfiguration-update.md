---
title: Обновление объекта windows10SecureAssessmentConfiguration
description: Обновление свойств объекта windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ae56b06f333b4d172a024f745258afb5ff710011
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817096"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="2b908-103">Обновление объекта windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b908-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="2b908-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2b908-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b908-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b908-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b908-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2b908-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b908-107">Обновление свойств объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b908-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b908-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2b908-108">Prerequisites</span></span>
<span data-ttu-id="2b908-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b908-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b908-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b908-111">Permission type</span></span>|<span data-ttu-id="2b908-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b908-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b908-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b908-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b908-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b908-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b908-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b908-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b908-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b908-116">Not supported.</span></span>|
|<span data-ttu-id="2b908-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b908-117">Application</span></span>|<span data-ttu-id="2b908-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b908-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b908-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b908-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2b908-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b908-120">Request headers</span></span>
|<span data-ttu-id="2b908-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b908-121">Header</span></span>|<span data-ttu-id="2b908-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b908-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b908-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b908-123">Authorization</span></span>|<span data-ttu-id="2b908-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2b908-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b908-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b908-125">Accept</span></span>|<span data-ttu-id="2b908-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b908-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b908-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b908-127">Request body</span></span>
<span data-ttu-id="2b908-128">В теле запроса добавьте представление объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b908-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="2b908-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b908-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="2b908-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b908-130">Property</span></span>|<span data-ttu-id="2b908-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b908-131">Type</span></span>|<span data-ttu-id="2b908-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b908-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b908-133">id</span><span class="sxs-lookup"><span data-stu-id="2b908-133">id</span></span>|<span data-ttu-id="2b908-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2b908-134">String</span></span>|<span data-ttu-id="2b908-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2b908-135">Key of the entity.</span></span> <span data-ttu-id="2b908-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b908-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b908-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b908-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2b908-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b908-138">DateTimeOffset</span></span>|<span data-ttu-id="2b908-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2b908-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2b908-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b908-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b908-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b908-141">roleScopeTagIds</span></span>|<span data-ttu-id="2b908-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2b908-142">String collection</span></span>|<span data-ttu-id="2b908-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2b908-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2b908-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b908-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b908-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2b908-145">supportsScopeTags</span></span>|<span data-ttu-id="2b908-146">Логический</span><span class="sxs-lookup"><span data-stu-id="2b908-146">Boolean</span></span>|<span data-ttu-id="2b908-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="2b908-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2b908-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="2b908-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2b908-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2b908-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2b908-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b908-150">This property is read-only.</span></span> <span data-ttu-id="2b908-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b908-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b908-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b908-152">createdDateTime</span></span>|<span data-ttu-id="2b908-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b908-153">DateTimeOffset</span></span>|<span data-ttu-id="2b908-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2b908-154">DateTime the object was created.</span></span> <span data-ttu-id="2b908-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b908-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b908-156">описание</span><span class="sxs-lookup"><span data-stu-id="2b908-156">description</span></span>|<span data-ttu-id="2b908-157">Строка</span><span class="sxs-lookup"><span data-stu-id="2b908-157">String</span></span>|<span data-ttu-id="2b908-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b908-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2b908-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b908-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b908-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2b908-160">displayName</span></span>|<span data-ttu-id="2b908-161">Строка</span><span class="sxs-lookup"><span data-stu-id="2b908-161">String</span></span>|<span data-ttu-id="2b908-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b908-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2b908-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b908-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b908-164">version</span><span class="sxs-lookup"><span data-stu-id="2b908-164">version</span></span>|<span data-ttu-id="2b908-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2b908-165">Int32</span></span>|<span data-ttu-id="2b908-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b908-166">Version of the device configuration.</span></span> <span data-ttu-id="2b908-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b908-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b908-168">launchUri</span><span class="sxs-lookup"><span data-stu-id="2b908-168">launchUri</span></span>|<span data-ttu-id="2b908-169">String</span><span class="sxs-lookup"><span data-stu-id="2b908-169">String</span></span>|<span data-ttu-id="2b908-170">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="2b908-170">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="2b908-171">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="2b908-171">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="2b908-172">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="2b908-172">configurationAccount</span></span>|<span data-ttu-id="2b908-173">String</span><span class="sxs-lookup"><span data-stu-id="2b908-173">String</span></span>|<span data-ttu-id="2b908-174">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="2b908-174">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="2b908-175">В качестве пользователя можно указать учетную запись домена (домен\пользователь), учетную запись AAD (имя_пользователя@клиент.com) или локальную учетную запись (имя_пользователя).</span><span class="sxs-lookup"><span data-stu-id="2b908-175">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="2b908-176">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="2b908-176">configurationAccountType</span></span>|[<span data-ttu-id="2b908-177">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="2b908-177">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="2b908-178">Тип учетной записи, используемые ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="2b908-178">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="2b908-179">Возможные значения: `azureADAccount`, `domainAccount`, `localAccount`.</span><span class="sxs-lookup"><span data-stu-id="2b908-179">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="2b908-180">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="2b908-180">allowPrinting</span></span>|<span data-ttu-id="2b908-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b908-181">Boolean</span></span>|<span data-ttu-id="2b908-182">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="2b908-182">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="2b908-183">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="2b908-183">allowScreenCapture</span></span>|<span data-ttu-id="2b908-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b908-184">Boolean</span></span>|<span data-ttu-id="2b908-185">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="2b908-185">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="2b908-186">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="2b908-186">allowTextSuggestion</span></span>|<span data-ttu-id="2b908-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b908-187">Boolean</span></span>|<span data-ttu-id="2b908-188">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="2b908-188">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="2b908-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b908-189">Response</span></span>
<span data-ttu-id="2b908-190">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b908-190">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b908-191">Пример</span><span class="sxs-lookup"><span data-stu-id="2b908-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b908-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b908-192">Request</span></span>
<span data-ttu-id="2b908-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b908-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 486

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="2b908-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b908-194">Response</span></span>
<span data-ttu-id="2b908-p114">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2b908-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





