---
title: Обновление объекта windows10SecureAssessmentConfiguration
description: Обновление свойств объекта windows10SecureAssessmentConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c2271163181b6be26d57cfe0cbf4443bd14ff829
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976805"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="631ce-103">Обновление объекта windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="631ce-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="631ce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="631ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="631ce-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="631ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="631ce-106">Обновление свойств объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-106">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="631ce-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="631ce-107">Prerequisites</span></span>
<span data-ttu-id="631ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="631ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="631ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="631ce-110">Permission type</span></span>|<span data-ttu-id="631ce-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="631ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="631ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="631ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="631ce-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="631ce-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="631ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="631ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="631ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="631ce-115">Not supported.</span></span>|
|<span data-ttu-id="631ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="631ce-116">Application</span></span>|<span data-ttu-id="631ce-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="631ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="631ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="631ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="631ce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="631ce-119">Request headers</span></span>
|<span data-ttu-id="631ce-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="631ce-120">Header</span></span>|<span data-ttu-id="631ce-121">Значение</span><span class="sxs-lookup"><span data-stu-id="631ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="631ce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="631ce-122">Authorization</span></span>|<span data-ttu-id="631ce-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="631ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="631ce-124">Accept</span><span class="sxs-lookup"><span data-stu-id="631ce-124">Accept</span></span>|<span data-ttu-id="631ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="631ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="631ce-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="631ce-126">Request body</span></span>
<span data-ttu-id="631ce-127">В теле запроса добавьте представление объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="631ce-127">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="631ce-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-128">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="631ce-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="631ce-129">Property</span></span>|<span data-ttu-id="631ce-130">Тип</span><span class="sxs-lookup"><span data-stu-id="631ce-130">Type</span></span>|<span data-ttu-id="631ce-131">Описание</span><span class="sxs-lookup"><span data-stu-id="631ce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="631ce-132">id</span><span class="sxs-lookup"><span data-stu-id="631ce-132">id</span></span>|<span data-ttu-id="631ce-133">Строка</span><span class="sxs-lookup"><span data-stu-id="631ce-133">String</span></span>|<span data-ttu-id="631ce-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="631ce-134">Key of the entity.</span></span> <span data-ttu-id="631ce-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631ce-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="631ce-136">lastModifiedDateTime</span></span>|<span data-ttu-id="631ce-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="631ce-137">DateTimeOffset</span></span>|<span data-ttu-id="631ce-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="631ce-138">DateTime the object was last modified.</span></span> <span data-ttu-id="631ce-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631ce-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="631ce-140">roleScopeTagIds</span></span>|<span data-ttu-id="631ce-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="631ce-141">String collection</span></span>|<span data-ttu-id="631ce-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="631ce-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="631ce-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631ce-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="631ce-144">supportsScopeTags</span></span>|<span data-ttu-id="631ce-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="631ce-145">Boolean</span></span>|<span data-ttu-id="631ce-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="631ce-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="631ce-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="631ce-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="631ce-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="631ce-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="631ce-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="631ce-149">This property is read-only.</span></span> <span data-ttu-id="631ce-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631ce-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="631ce-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="631ce-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="631ce-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="631ce-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="631ce-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="631ce-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631ce-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="631ce-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="631ce-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="631ce-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="631ce-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="631ce-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="631ce-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631ce-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="631ce-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="631ce-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="631ce-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="631ce-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="631ce-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="631ce-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631ce-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="631ce-163">createdDateTime</span></span>|<span data-ttu-id="631ce-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="631ce-164">DateTimeOffset</span></span>|<span data-ttu-id="631ce-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="631ce-165">DateTime the object was created.</span></span> <span data-ttu-id="631ce-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631ce-167">description</span><span class="sxs-lookup"><span data-stu-id="631ce-167">description</span></span>|<span data-ttu-id="631ce-168">String</span><span class="sxs-lookup"><span data-stu-id="631ce-168">String</span></span>|<span data-ttu-id="631ce-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="631ce-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="631ce-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631ce-171">displayName</span><span class="sxs-lookup"><span data-stu-id="631ce-171">displayName</span></span>|<span data-ttu-id="631ce-172">Строка</span><span class="sxs-lookup"><span data-stu-id="631ce-172">String</span></span>|<span data-ttu-id="631ce-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="631ce-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="631ce-174">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="631ce-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631ce-175">version</span><span class="sxs-lookup"><span data-stu-id="631ce-175">version</span></span>|<span data-ttu-id="631ce-176">Int32</span><span class="sxs-lookup"><span data-stu-id="631ce-176">Int32</span></span>|<span data-ttu-id="631ce-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="631ce-177">Version of the device configuration.</span></span> <span data-ttu-id="631ce-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="631ce-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="631ce-179">launchUri</span><span class="sxs-lookup"><span data-stu-id="631ce-179">launchUri</span></span>|<span data-ttu-id="631ce-180">String</span><span class="sxs-lookup"><span data-stu-id="631ce-180">String</span></span>|<span data-ttu-id="631ce-181">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="631ce-181">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="631ce-182">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="631ce-182">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="631ce-183">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="631ce-183">configurationAccount</span></span>|<span data-ttu-id="631ce-184">String</span><span class="sxs-lookup"><span data-stu-id="631ce-184">String</span></span>|<span data-ttu-id="631ce-185">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="631ce-185">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="631ce-186">В качестве пользователя можно указать учетную запись домена (domen\polzovatel), учетную запись AAD (imya_polzovatelya@klient.com) или локальную учетную запись (имя пользователя).</span><span class="sxs-lookup"><span data-stu-id="631ce-186">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="631ce-187">Конфигуратионаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="631ce-187">configurationAccountType</span></span>|[<span data-ttu-id="631ce-188">Секуреассессментаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="631ce-188">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="631ce-189">Тип учетной записи, используемой в Конфигуратионаккаунт.</span><span class="sxs-lookup"><span data-stu-id="631ce-189">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="631ce-190">Возможные значения: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span><span class="sxs-lookup"><span data-stu-id="631ce-190">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="631ce-191">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="631ce-191">allowPrinting</span></span>|<span data-ttu-id="631ce-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="631ce-192">Boolean</span></span>|<span data-ttu-id="631ce-193">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="631ce-193">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="631ce-194">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="631ce-194">allowScreenCapture</span></span>|<span data-ttu-id="631ce-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="631ce-195">Boolean</span></span>|<span data-ttu-id="631ce-196">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="631ce-196">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="631ce-197">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="631ce-197">allowTextSuggestion</span></span>|<span data-ttu-id="631ce-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="631ce-198">Boolean</span></span>|<span data-ttu-id="631ce-199">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="631ce-199">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="631ce-200">Локалгуестаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="631ce-200">localGuestAccountName</span></span>|<span data-ttu-id="631ce-201">String</span><span class="sxs-lookup"><span data-stu-id="631ce-201">String</span></span>|<span data-ttu-id="631ce-202">Указывает отображаемый текст для локальной гостевой учетной записи, отображаемой на экране входа.</span><span class="sxs-lookup"><span data-stu-id="631ce-202">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="631ce-203">Обычно это имя оценки.</span><span class="sxs-lookup"><span data-stu-id="631ce-203">Typically is the name of an assessment.</span></span> <span data-ttu-id="631ce-204">Когда пользователь нажимает на экране входа локальную гостевую учетную запись, запускается приложение для оценки с указанным URL-адресом оценки.</span><span class="sxs-lookup"><span data-stu-id="631ce-204">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="631ce-205">Для безопасной оценки можно использовать только локальную гостевую учетную запись на устройствах под управлением Windows 10 версии 1903 или более поздней.</span><span class="sxs-lookup"><span data-stu-id="631ce-205">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="631ce-206">Важное примечание. это свойство должно быть задано с помощью Ассессментаппусермоделид, чтобы обеспечить правильную работу локальной учетной записи гостя для обеспечения безопасной оценки.</span><span class="sxs-lookup"><span data-stu-id="631ce-206">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="631ce-207">Ассессментаппусермоделид</span><span class="sxs-lookup"><span data-stu-id="631ce-207">assessmentAppUserModelId</span></span>|<span data-ttu-id="631ce-208">String</span><span class="sxs-lookup"><span data-stu-id="631ce-208">String</span></span>|<span data-ttu-id="631ce-209">Указывает идентификатор пользовательской модели приложения для оценки, запущенной при входе пользователя в систему для безопасной оценки с помощью локальной учетной записи гостя.</span><span class="sxs-lookup"><span data-stu-id="631ce-209">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="631ce-210">Важное примечание. это свойство должно быть задано с помощью Локалгуестаккаунтнаме, чтобы обеспечить правильную работу локальной учетной записи гостя для обеспечения безопасной оценки.</span><span class="sxs-lookup"><span data-stu-id="631ce-210">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="631ce-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="631ce-211">Response</span></span>
<span data-ttu-id="631ce-212">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="631ce-212">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="631ce-213">Пример</span><span class="sxs-lookup"><span data-stu-id="631ce-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="631ce-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="631ce-214">Request</span></span>
<span data-ttu-id="631ce-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="631ce-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="631ce-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="631ce-216">Response</span></span>
<span data-ttu-id="631ce-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="631ce-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





