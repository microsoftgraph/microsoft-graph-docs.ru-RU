---
title: Create windows10SecureAssessmentConfiguration
description: Создание объекта windows10SecureAssessmentConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 90098638dc2094d6d32fd2681d48d76ef5981279
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42738489"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="74ca4-103">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="74ca4-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="74ca4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74ca4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74ca4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74ca4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74ca4-106">Создание объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ca4-106">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74ca4-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="74ca4-107">Prerequisites</span></span>
<span data-ttu-id="74ca4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74ca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74ca4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74ca4-110">Permission type</span></span>|<span data-ttu-id="74ca4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74ca4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74ca4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74ca4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74ca4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74ca4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74ca4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74ca4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74ca4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74ca4-115">Not supported.</span></span>|
|<span data-ttu-id="74ca4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="74ca4-116">Application</span></span>|<span data-ttu-id="74ca4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74ca4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74ca4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74ca4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="74ca4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="74ca4-119">Request headers</span></span>
|<span data-ttu-id="74ca4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74ca4-120">Header</span></span>|<span data-ttu-id="74ca4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="74ca4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74ca4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="74ca4-122">Authorization</span></span>|<span data-ttu-id="74ca4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74ca4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74ca4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="74ca4-124">Accept</span></span>|<span data-ttu-id="74ca4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74ca4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74ca4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74ca4-126">Request body</span></span>
<span data-ttu-id="74ca4-127">В тексте запроса добавьте представление объекта windows10SecureAssessmentConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74ca4-127">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="74ca4-128">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="74ca4-128">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="74ca4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="74ca4-129">Property</span></span>|<span data-ttu-id="74ca4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="74ca4-130">Type</span></span>|<span data-ttu-id="74ca4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="74ca4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74ca4-132">id</span><span class="sxs-lookup"><span data-stu-id="74ca4-132">id</span></span>|<span data-ttu-id="74ca4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="74ca4-133">String</span></span>|<span data-ttu-id="74ca4-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="74ca4-134">Key of the entity.</span></span> <span data-ttu-id="74ca4-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ca4-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74ca4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="74ca4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74ca4-137">DateTimeOffset</span></span>|<span data-ttu-id="74ca4-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="74ca4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="74ca4-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ca4-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="74ca4-140">roleScopeTagIds</span></span>|<span data-ttu-id="74ca4-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="74ca4-141">String collection</span></span>|<span data-ttu-id="74ca4-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="74ca4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="74ca4-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ca4-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="74ca4-144">supportsScopeTags</span></span>|<span data-ttu-id="74ca4-145">Логический</span><span class="sxs-lookup"><span data-stu-id="74ca4-145">Boolean</span></span>|<span data-ttu-id="74ca4-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="74ca4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="74ca4-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="74ca4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="74ca4-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="74ca4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="74ca4-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74ca4-149">This property is read-only.</span></span> <span data-ttu-id="74ca4-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ca4-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="74ca4-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="74ca4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="74ca4-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="74ca4-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="74ca4-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="74ca4-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ca4-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="74ca4-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="74ca4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="74ca4-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="74ca4-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="74ca4-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="74ca4-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ca4-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="74ca4-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="74ca4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="74ca4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="74ca4-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="74ca4-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="74ca4-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ca4-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74ca4-163">createdDateTime</span></span>|<span data-ttu-id="74ca4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74ca4-164">DateTimeOffset</span></span>|<span data-ttu-id="74ca4-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="74ca4-165">DateTime the object was created.</span></span> <span data-ttu-id="74ca4-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ca4-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-167">description</span><span class="sxs-lookup"><span data-stu-id="74ca4-167">description</span></span>|<span data-ttu-id="74ca4-168">String</span><span class="sxs-lookup"><span data-stu-id="74ca4-168">String</span></span>|<span data-ttu-id="74ca4-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="74ca4-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="74ca4-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ca4-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-171">displayName</span><span class="sxs-lookup"><span data-stu-id="74ca4-171">displayName</span></span>|<span data-ttu-id="74ca4-172">Строка</span><span class="sxs-lookup"><span data-stu-id="74ca4-172">String</span></span>|<span data-ttu-id="74ca4-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="74ca4-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="74ca4-174">Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="74ca4-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-175">version</span><span class="sxs-lookup"><span data-stu-id="74ca4-175">version</span></span>|<span data-ttu-id="74ca4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="74ca4-176">Int32</span></span>|<span data-ttu-id="74ca4-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="74ca4-177">Version of the device configuration.</span></span> <span data-ttu-id="74ca4-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ca4-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="74ca4-179">launchUri</span><span class="sxs-lookup"><span data-stu-id="74ca4-179">launchUri</span></span>|<span data-ttu-id="74ca4-180">String</span><span class="sxs-lookup"><span data-stu-id="74ca4-180">String</span></span>|<span data-ttu-id="74ca4-181">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="74ca4-181">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="74ca4-182">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="74ca4-182">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="74ca4-183">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="74ca4-183">configurationAccount</span></span>|<span data-ttu-id="74ca4-184">String</span><span class="sxs-lookup"><span data-stu-id="74ca4-184">String</span></span>|<span data-ttu-id="74ca4-185">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="74ca4-185">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="74ca4-186">В качестве пользователя можно указать учетную запись домена (domen\polzovatel), учетную запись AAD (imya_polzovatelya@klient.com) или локальную учетную запись (имя пользователя).</span><span class="sxs-lookup"><span data-stu-id="74ca4-186">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="74ca4-187">конфигуратионаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="74ca4-187">configurationAccountType</span></span>|[<span data-ttu-id="74ca4-188">секуреассессментаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="74ca4-188">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="74ca4-189">Тип учетной записи, используемой в Конфигуратионаккаунт.</span><span class="sxs-lookup"><span data-stu-id="74ca4-189">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="74ca4-190">Возможные значения: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span><span class="sxs-lookup"><span data-stu-id="74ca4-190">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="74ca4-191">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="74ca4-191">allowPrinting</span></span>|<span data-ttu-id="74ca4-192">Логический</span><span class="sxs-lookup"><span data-stu-id="74ca4-192">Boolean</span></span>|<span data-ttu-id="74ca4-193">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="74ca4-193">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="74ca4-194">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="74ca4-194">allowScreenCapture</span></span>|<span data-ttu-id="74ca4-195">Логический</span><span class="sxs-lookup"><span data-stu-id="74ca4-195">Boolean</span></span>|<span data-ttu-id="74ca4-196">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="74ca4-196">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="74ca4-197">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="74ca4-197">allowTextSuggestion</span></span>|<span data-ttu-id="74ca4-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="74ca4-198">Boolean</span></span>|<span data-ttu-id="74ca4-199">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="74ca4-199">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="74ca4-200">локалгуестаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="74ca4-200">localGuestAccountName</span></span>|<span data-ttu-id="74ca4-201">String</span><span class="sxs-lookup"><span data-stu-id="74ca4-201">String</span></span>|<span data-ttu-id="74ca4-202">Указывает отображаемый текст для локальной гостевой учетной записи, отображаемой на экране входа.</span><span class="sxs-lookup"><span data-stu-id="74ca4-202">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="74ca4-203">Обычно это имя оценки.</span><span class="sxs-lookup"><span data-stu-id="74ca4-203">Typically is the name of an assessment.</span></span> <span data-ttu-id="74ca4-204">Когда пользователь нажимает на экране входа локальную гостевую учетную запись, запускается приложение для оценки с указанным URL-адресом оценки.</span><span class="sxs-lookup"><span data-stu-id="74ca4-204">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="74ca4-205">Для безопасной оценки можно использовать только локальную гостевую учетную запись на устройствах под управлением Windows 10 версии 1903 или более поздней.</span><span class="sxs-lookup"><span data-stu-id="74ca4-205">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="74ca4-206">Важное примечание. это свойство должно быть задано с помощью Ассессментаппусермоделид, чтобы обеспечить правильную работу локальной учетной записи гостя для обеспечения безопасной оценки.</span><span class="sxs-lookup"><span data-stu-id="74ca4-206">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="74ca4-207">ассессментаппусермоделид</span><span class="sxs-lookup"><span data-stu-id="74ca4-207">assessmentAppUserModelId</span></span>|<span data-ttu-id="74ca4-208">String</span><span class="sxs-lookup"><span data-stu-id="74ca4-208">String</span></span>|<span data-ttu-id="74ca4-209">Указывает идентификатор пользовательской модели приложения для оценки, запущенной при входе пользователя в систему для безопасной оценки с помощью локальной учетной записи гостя.</span><span class="sxs-lookup"><span data-stu-id="74ca4-209">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="74ca4-210">Важное примечание. это свойство должно быть задано с помощью Локалгуестаккаунтнаме, чтобы обеспечить правильную работу локальной учетной записи гостя для обеспечения безопасной оценки.</span><span class="sxs-lookup"><span data-stu-id="74ca4-210">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="74ca4-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="74ca4-211">Response</span></span>
<span data-ttu-id="74ca4-212">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="74ca4-212">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74ca4-213">Пример</span><span class="sxs-lookup"><span data-stu-id="74ca4-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="74ca4-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="74ca4-214">Request</span></span>
<span data-ttu-id="74ca4-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74ca4-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74ca4-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="74ca4-216">Response</span></span>
<span data-ttu-id="74ca4-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74ca4-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




