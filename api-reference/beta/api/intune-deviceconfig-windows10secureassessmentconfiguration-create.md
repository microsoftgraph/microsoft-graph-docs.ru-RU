---
title: Create windows10SecureAssessmentConfiguration
description: Создание объекта windows10SecureAssessmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c48e4c2ffdbc6f09bdca1d9f4563261288cbf1c9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127482"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="fbd5d-103">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="fbd5d-103">Create windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="fbd5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbd5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbd5d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbd5d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbd5d-107">Создание объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-107">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbd5d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fbd5d-108">Prerequisites</span></span>
<span data-ttu-id="fbd5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbd5d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbd5d-111">Permission type</span></span>|<span data-ttu-id="fbd5d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbd5d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbd5d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbd5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbd5d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbd5d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fbd5d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbd5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbd5d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-116">Not supported.</span></span>|
|<span data-ttu-id="fbd5d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fbd5d-117">Application</span></span>|<span data-ttu-id="fbd5d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbd5d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbd5d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbd5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fbd5d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fbd5d-120">Request headers</span></span>
|<span data-ttu-id="fbd5d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbd5d-121">Header</span></span>|<span data-ttu-id="fbd5d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fbd5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbd5d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbd5d-123">Authorization</span></span>|<span data-ttu-id="fbd5d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbd5d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fbd5d-125">Accept</span></span>|<span data-ttu-id="fbd5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbd5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbd5d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbd5d-127">Request body</span></span>
<span data-ttu-id="fbd5d-128">В тексте запроса добавьте представление объекта windows10SecureAssessmentConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-128">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="fbd5d-129">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-129">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="fbd5d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbd5d-130">Property</span></span>|<span data-ttu-id="fbd5d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fbd5d-131">Type</span></span>|<span data-ttu-id="fbd5d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fbd5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbd5d-133">id</span><span class="sxs-lookup"><span data-stu-id="fbd5d-133">id</span></span>|<span data-ttu-id="fbd5d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fbd5d-134">String</span></span>|<span data-ttu-id="fbd5d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-135">Key of the entity.</span></span> <span data-ttu-id="fbd5d-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbd5d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbd5d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fbd5d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbd5d-138">DateTimeOffset</span></span>|<span data-ttu-id="fbd5d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fbd5d-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbd5d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fbd5d-141">roleScopeTagIds</span></span>|<span data-ttu-id="fbd5d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fbd5d-142">String collection</span></span>|<span data-ttu-id="fbd5d-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fbd5d-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbd5d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fbd5d-145">supportsScopeTags</span></span>|<span data-ttu-id="fbd5d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbd5d-146">Boolean</span></span>|<span data-ttu-id="fbd5d-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fbd5d-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fbd5d-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fbd5d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-150">This property is read-only.</span></span> <span data-ttu-id="fbd5d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbd5d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fbd5d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fbd5d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fbd5d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fbd5d-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fbd5d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbd5d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fbd5d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fbd5d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fbd5d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fbd5d-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fbd5d-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbd5d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fbd5d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fbd5d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fbd5d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fbd5d-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fbd5d-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbd5d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbd5d-164">createdDateTime</span></span>|<span data-ttu-id="fbd5d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbd5d-165">DateTimeOffset</span></span>|<span data-ttu-id="fbd5d-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-166">DateTime the object was created.</span></span> <span data-ttu-id="fbd5d-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbd5d-168">description</span><span class="sxs-lookup"><span data-stu-id="fbd5d-168">description</span></span>|<span data-ttu-id="fbd5d-169">Строка</span><span class="sxs-lookup"><span data-stu-id="fbd5d-169">String</span></span>|<span data-ttu-id="fbd5d-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fbd5d-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbd5d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fbd5d-172">displayName</span></span>|<span data-ttu-id="fbd5d-173">Строка</span><span class="sxs-lookup"><span data-stu-id="fbd5d-173">String</span></span>|<span data-ttu-id="fbd5d-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fbd5d-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbd5d-176">version</span><span class="sxs-lookup"><span data-stu-id="fbd5d-176">version</span></span>|<span data-ttu-id="fbd5d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fbd5d-177">Int32</span></span>|<span data-ttu-id="fbd5d-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-178">Version of the device configuration.</span></span> <span data-ttu-id="fbd5d-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbd5d-180">launchUri</span><span class="sxs-lookup"><span data-stu-id="fbd5d-180">launchUri</span></span>|<span data-ttu-id="fbd5d-181">String</span><span class="sxs-lookup"><span data-stu-id="fbd5d-181">String</span></span>|<span data-ttu-id="fbd5d-182">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-182">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="fbd5d-183">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-183">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="fbd5d-184">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="fbd5d-184">configurationAccount</span></span>|<span data-ttu-id="fbd5d-185">String</span><span class="sxs-lookup"><span data-stu-id="fbd5d-185">String</span></span>|<span data-ttu-id="fbd5d-186">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-186">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="fbd5d-187">В качестве пользователя можно указать учетную запись домена (domen\polzovatel), учетную запись AAD (imya_polzovatelya@klient.com) или локальную учетную запись (имя пользователя).</span><span class="sxs-lookup"><span data-stu-id="fbd5d-187">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="fbd5d-188">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="fbd5d-188">configurationAccountType</span></span>|[<span data-ttu-id="fbd5d-189">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="fbd5d-189">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="fbd5d-190">Тип учетной записи, используемый в ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-190">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="fbd5d-191">Возможные значения: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-191">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="fbd5d-192">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="fbd5d-192">allowPrinting</span></span>|<span data-ttu-id="fbd5d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbd5d-193">Boolean</span></span>|<span data-ttu-id="fbd5d-194">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-194">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="fbd5d-195">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="fbd5d-195">allowScreenCapture</span></span>|<span data-ttu-id="fbd5d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbd5d-196">Boolean</span></span>|<span data-ttu-id="fbd5d-197">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-197">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="fbd5d-198">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="fbd5d-198">allowTextSuggestion</span></span>|<span data-ttu-id="fbd5d-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbd5d-199">Boolean</span></span>|<span data-ttu-id="fbd5d-200">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-200">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="fbd5d-201">localGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="fbd5d-201">localGuestAccountName</span></span>|<span data-ttu-id="fbd5d-202">Строка</span><span class="sxs-lookup"><span data-stu-id="fbd5d-202">String</span></span>|<span data-ttu-id="fbd5d-203">Указывает текст отображения для локальной учетной записи гостей, показанной на экране входной записи.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-203">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="fbd5d-204">Обычно это имя оценки.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-204">Typically is the name of an assessment.</span></span> <span data-ttu-id="fbd5d-205">Когда пользователь щелкает локализованную учетную запись гостя на экране входной записи, запущено приложение оценки с указанным URL-адресом оценки.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-205">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="fbd5d-206">Безопасные оценки можно настроить только с помощью местного входного окна на устройствах с Windows 10, версии 1903 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-206">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="fbd5d-207">Важное уведомление: это свойство должно быть задано с помощью assessmentAppUserModelID, чтобы обеспечить надежную работу местной учетной записи для безопасной оценки.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-207">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="fbd5d-208">assessmentAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="fbd5d-208">assessmentAppUserModelId</span></span>|<span data-ttu-id="fbd5d-209">Строка</span><span class="sxs-lookup"><span data-stu-id="fbd5d-209">String</span></span>|<span data-ttu-id="fbd5d-210">Указывает ID модели приложения приложения-пользователя, запущенного при впуске пользователя в безопасную оценку с локальной учетной записью гостей.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-210">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="fbd5d-211">Важное уведомление: это свойство должно быть заданной с помощью localGuestAccountName, чтобы обеспечить надежную работу местной учетной записи для безопасной оценки.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-211">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="fbd5d-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbd5d-212">Response</span></span>
<span data-ttu-id="fbd5d-213">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-213">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbd5d-214">Пример</span><span class="sxs-lookup"><span data-stu-id="fbd5d-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbd5d-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbd5d-215">Request</span></span>
<span data-ttu-id="fbd5d-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="fbd5d-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbd5d-217">Response</span></span>
<span data-ttu-id="fbd5d-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbd5d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




