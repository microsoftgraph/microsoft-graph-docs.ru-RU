---
title: Обновление объекта windows10SecureAssessmentConfiguration
description: Обновление свойств объекта windows10SecureAssessmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc91366f1d7ae9e827795f10b95cd352f9d97b42
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127447"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="a8288-103">Обновление объекта windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8288-103">Update windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="a8288-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8288-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8288-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8288-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8288-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8288-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8288-107">Обновление свойств объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8288-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a8288-108">Prerequisites</span></span>
<span data-ttu-id="a8288-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8288-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8288-111">Permission type</span></span>|<span data-ttu-id="a8288-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8288-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8288-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8288-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8288-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8288-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8288-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8288-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8288-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8288-116">Not supported.</span></span>|
|<span data-ttu-id="a8288-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a8288-117">Application</span></span>|<span data-ttu-id="a8288-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8288-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8288-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8288-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a8288-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a8288-120">Request headers</span></span>
|<span data-ttu-id="a8288-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8288-121">Header</span></span>|<span data-ttu-id="a8288-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a8288-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8288-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8288-123">Authorization</span></span>|<span data-ttu-id="a8288-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8288-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8288-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8288-125">Accept</span></span>|<span data-ttu-id="a8288-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8288-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8288-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8288-127">Request body</span></span>
<span data-ttu-id="a8288-128">В теле запроса добавьте представление объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8288-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="a8288-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="a8288-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8288-130">Property</span></span>|<span data-ttu-id="a8288-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a8288-131">Type</span></span>|<span data-ttu-id="a8288-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a8288-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8288-133">id</span><span class="sxs-lookup"><span data-stu-id="a8288-133">id</span></span>|<span data-ttu-id="a8288-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a8288-134">String</span></span>|<span data-ttu-id="a8288-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a8288-135">Key of the entity.</span></span> <span data-ttu-id="a8288-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8288-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8288-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a8288-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8288-138">DateTimeOffset</span></span>|<span data-ttu-id="a8288-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a8288-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a8288-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8288-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8288-141">roleScopeTagIds</span></span>|<span data-ttu-id="a8288-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a8288-142">String collection</span></span>|<span data-ttu-id="a8288-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="a8288-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a8288-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8288-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a8288-145">supportsScopeTags</span></span>|<span data-ttu-id="a8288-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8288-146">Boolean</span></span>|<span data-ttu-id="a8288-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a8288-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a8288-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="a8288-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a8288-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a8288-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a8288-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8288-150">This property is read-only.</span></span> <span data-ttu-id="a8288-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8288-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a8288-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a8288-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a8288-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a8288-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a8288-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a8288-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8288-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a8288-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a8288-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a8288-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a8288-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a8288-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a8288-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8288-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a8288-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a8288-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a8288-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a8288-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a8288-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a8288-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8288-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8288-164">createdDateTime</span></span>|<span data-ttu-id="a8288-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8288-165">DateTimeOffset</span></span>|<span data-ttu-id="a8288-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a8288-166">DateTime the object was created.</span></span> <span data-ttu-id="a8288-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8288-168">description</span><span class="sxs-lookup"><span data-stu-id="a8288-168">description</span></span>|<span data-ttu-id="a8288-169">Строка</span><span class="sxs-lookup"><span data-stu-id="a8288-169">String</span></span>|<span data-ttu-id="a8288-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8288-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a8288-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8288-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a8288-172">displayName</span></span>|<span data-ttu-id="a8288-173">Строка</span><span class="sxs-lookup"><span data-stu-id="a8288-173">String</span></span>|<span data-ttu-id="a8288-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8288-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a8288-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8288-176">version</span><span class="sxs-lookup"><span data-stu-id="a8288-176">version</span></span>|<span data-ttu-id="a8288-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a8288-177">Int32</span></span>|<span data-ttu-id="a8288-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8288-178">Version of the device configuration.</span></span> <span data-ttu-id="a8288-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8288-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8288-180">launchUri</span><span class="sxs-lookup"><span data-stu-id="a8288-180">launchUri</span></span>|<span data-ttu-id="a8288-181">String</span><span class="sxs-lookup"><span data-stu-id="a8288-181">String</span></span>|<span data-ttu-id="a8288-182">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="a8288-182">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="a8288-183">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="a8288-183">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="a8288-184">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="a8288-184">configurationAccount</span></span>|<span data-ttu-id="a8288-185">String</span><span class="sxs-lookup"><span data-stu-id="a8288-185">String</span></span>|<span data-ttu-id="a8288-186">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="a8288-186">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="a8288-187">В качестве пользователя можно указать учетную запись домена (domen\polzovatel), учетную запись AAD (imya_polzovatelya@klient.com) или локальную учетную запись (имя пользователя).</span><span class="sxs-lookup"><span data-stu-id="a8288-187">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="a8288-188">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="a8288-188">configurationAccountType</span></span>|[<span data-ttu-id="a8288-189">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="a8288-189">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="a8288-190">Тип учетной записи, используемый в ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="a8288-190">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="a8288-191">Возможные значения: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span><span class="sxs-lookup"><span data-stu-id="a8288-191">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="a8288-192">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="a8288-192">allowPrinting</span></span>|<span data-ttu-id="a8288-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8288-193">Boolean</span></span>|<span data-ttu-id="a8288-194">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="a8288-194">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="a8288-195">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="a8288-195">allowScreenCapture</span></span>|<span data-ttu-id="a8288-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8288-196">Boolean</span></span>|<span data-ttu-id="a8288-197">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="a8288-197">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="a8288-198">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="a8288-198">allowTextSuggestion</span></span>|<span data-ttu-id="a8288-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8288-199">Boolean</span></span>|<span data-ttu-id="a8288-200">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="a8288-200">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="a8288-201">localGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="a8288-201">localGuestAccountName</span></span>|<span data-ttu-id="a8288-202">Строка</span><span class="sxs-lookup"><span data-stu-id="a8288-202">String</span></span>|<span data-ttu-id="a8288-203">Указывает текст отображения для локальной учетной записи гостей, показанной на экране входной записи.</span><span class="sxs-lookup"><span data-stu-id="a8288-203">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="a8288-204">Обычно это имя оценки.</span><span class="sxs-lookup"><span data-stu-id="a8288-204">Typically is the name of an assessment.</span></span> <span data-ttu-id="a8288-205">Когда пользователь щелкает локализованную учетную запись гостя на экране входной записи, запущено приложение оценки с указанным URL-адресом оценки.</span><span class="sxs-lookup"><span data-stu-id="a8288-205">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="a8288-206">Безопасные оценки можно настроить только с помощью местного входного окна на устройствах с Windows 10, версии 1903 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="a8288-206">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="a8288-207">Важное уведомление: это свойство должно быть задано с помощью assessmentAppUserModelID, чтобы обеспечить надежную работу местной учетной записи для безопасной оценки.</span><span class="sxs-lookup"><span data-stu-id="a8288-207">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="a8288-208">assessmentAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="a8288-208">assessmentAppUserModelId</span></span>|<span data-ttu-id="a8288-209">Строка</span><span class="sxs-lookup"><span data-stu-id="a8288-209">String</span></span>|<span data-ttu-id="a8288-210">Указывает ID модели приложения приложения-пользователя, запущенного при впуске пользователя в безопасную оценку с локальной учетной записью гостей.</span><span class="sxs-lookup"><span data-stu-id="a8288-210">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="a8288-211">Важное уведомление: это свойство должно быть заданной с помощью localGuestAccountName, чтобы обеспечить надежную работу местной учетной записи для безопасной оценки.</span><span class="sxs-lookup"><span data-stu-id="a8288-211">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="a8288-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8288-212">Response</span></span>
<span data-ttu-id="a8288-213">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a8288-213">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8288-214">Пример</span><span class="sxs-lookup"><span data-stu-id="a8288-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8288-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8288-215">Request</span></span>
<span data-ttu-id="a8288-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8288-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1403

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true,
  "localGuestAccountName": "Local Guest Account Name value",
  "assessmentAppUserModelId": "Assessment App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="a8288-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8288-217">Response</span></span>
<span data-ttu-id="a8288-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8288-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1575

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true,
  "localGuestAccountName": "Local Guest Account Name value",
  "assessmentAppUserModelId": "Assessment App User Model Id value"
}
```




