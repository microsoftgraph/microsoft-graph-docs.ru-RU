---
title: Обновление объекта windows10SecureAssessmentConfiguration
description: Обновление свойств объекта windows10SecureAssessmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e383d3b317b762a6cc130e3c409e64ce97f77ab5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43338470"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="1c42c-103">Обновление объекта windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c42c-103">Update windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="1c42c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c42c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c42c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c42c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c42c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c42c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c42c-107">Обновление свойств объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c42c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1c42c-108">Prerequisites</span></span>
<span data-ttu-id="1c42c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c42c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c42c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c42c-111">Permission type</span></span>|<span data-ttu-id="1c42c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c42c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c42c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c42c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c42c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c42c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c42c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c42c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c42c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c42c-116">Not supported.</span></span>|
|<span data-ttu-id="1c42c-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1c42c-117">Application</span></span>|<span data-ttu-id="1c42c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c42c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c42c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c42c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1c42c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1c42c-120">Request headers</span></span>
|<span data-ttu-id="1c42c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c42c-121">Header</span></span>|<span data-ttu-id="1c42c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1c42c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c42c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c42c-123">Authorization</span></span>|<span data-ttu-id="1c42c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c42c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c42c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c42c-125">Accept</span></span>|<span data-ttu-id="1c42c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c42c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c42c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c42c-127">Request body</span></span>
<span data-ttu-id="1c42c-128">В теле запроса добавьте представление объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c42c-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="1c42c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="1c42c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c42c-130">Property</span></span>|<span data-ttu-id="1c42c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1c42c-131">Type</span></span>|<span data-ttu-id="1c42c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1c42c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c42c-133">id</span><span class="sxs-lookup"><span data-stu-id="1c42c-133">id</span></span>|<span data-ttu-id="1c42c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1c42c-134">String</span></span>|<span data-ttu-id="1c42c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1c42c-135">Key of the entity.</span></span> <span data-ttu-id="1c42c-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c42c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c42c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1c42c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c42c-138">DateTimeOffset</span></span>|<span data-ttu-id="1c42c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1c42c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1c42c-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c42c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c42c-141">roleScopeTagIds</span></span>|<span data-ttu-id="1c42c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1c42c-142">String collection</span></span>|<span data-ttu-id="1c42c-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1c42c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1c42c-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c42c-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1c42c-145">supportsScopeTags</span></span>|<span data-ttu-id="1c42c-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="1c42c-146">Boolean</span></span>|<span data-ttu-id="1c42c-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1c42c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1c42c-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1c42c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1c42c-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1c42c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1c42c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c42c-150">This property is read-only.</span></span> <span data-ttu-id="1c42c-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c42c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1c42c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1c42c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1c42c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1c42c-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1c42c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1c42c-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c42c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1c42c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1c42c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1c42c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1c42c-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1c42c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1c42c-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c42c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1c42c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1c42c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1c42c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1c42c-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1c42c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1c42c-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c42c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c42c-164">createdDateTime</span></span>|<span data-ttu-id="1c42c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c42c-165">DateTimeOffset</span></span>|<span data-ttu-id="1c42c-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1c42c-166">DateTime the object was created.</span></span> <span data-ttu-id="1c42c-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c42c-168">description</span><span class="sxs-lookup"><span data-stu-id="1c42c-168">description</span></span>|<span data-ttu-id="1c42c-169">String</span><span class="sxs-lookup"><span data-stu-id="1c42c-169">String</span></span>|<span data-ttu-id="1c42c-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c42c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1c42c-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c42c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1c42c-172">displayName</span></span>|<span data-ttu-id="1c42c-173">Строка</span><span class="sxs-lookup"><span data-stu-id="1c42c-173">String</span></span>|<span data-ttu-id="1c42c-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c42c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1c42c-175">Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c42c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c42c-176">version</span><span class="sxs-lookup"><span data-stu-id="1c42c-176">version</span></span>|<span data-ttu-id="1c42c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1c42c-177">Int32</span></span>|<span data-ttu-id="1c42c-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c42c-178">Version of the device configuration.</span></span> <span data-ttu-id="1c42c-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c42c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c42c-180">launchUri</span><span class="sxs-lookup"><span data-stu-id="1c42c-180">launchUri</span></span>|<span data-ttu-id="1c42c-181">String</span><span class="sxs-lookup"><span data-stu-id="1c42c-181">String</span></span>|<span data-ttu-id="1c42c-182">URL-адрес страницы оценки, которая автоматически загружается при запуске браузера для надежного тестирования.</span><span class="sxs-lookup"><span data-stu-id="1c42c-182">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="1c42c-183">Это должен быть допустимый URL-адрес (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="1c42c-183">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="1c42c-184">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="1c42c-184">configurationAccount</span></span>|<span data-ttu-id="1c42c-185">String</span><span class="sxs-lookup"><span data-stu-id="1c42c-185">String</span></span>|<span data-ttu-id="1c42c-186">Учетная запись, с использованием которой настраивается устройство с Windows для прохождения теста.</span><span class="sxs-lookup"><span data-stu-id="1c42c-186">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="1c42c-187">В качестве пользователя можно указать учетную запись домена (domen\polzovatel), учетную запись AAD (imya_polzovatelya@klient.com) или локальную учетную запись (имя пользователя).</span><span class="sxs-lookup"><span data-stu-id="1c42c-187">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="1c42c-188">конфигуратионаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="1c42c-188">configurationAccountType</span></span>|[<span data-ttu-id="1c42c-189">секуреассессментаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="1c42c-189">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="1c42c-190">Тип учетной записи, используемой в Конфигуратионаккаунт.</span><span class="sxs-lookup"><span data-stu-id="1c42c-190">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="1c42c-191">Возможные значения: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span><span class="sxs-lookup"><span data-stu-id="1c42c-191">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="1c42c-192">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="1c42c-192">allowPrinting</span></span>|<span data-ttu-id="1c42c-193">Логическое</span><span class="sxs-lookup"><span data-stu-id="1c42c-193">Boolean</span></span>|<span data-ttu-id="1c42c-194">Определяет, разрешается ли приложению печатать во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="1c42c-194">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="1c42c-195">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="1c42c-195">allowScreenCapture</span></span>|<span data-ttu-id="1c42c-196">Логическое</span><span class="sxs-lookup"><span data-stu-id="1c42c-196">Boolean</span></span>|<span data-ttu-id="1c42c-197">Определяет, разрешается ли создавать снимки экрана во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="1c42c-197">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="1c42c-198">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="1c42c-198">allowTextSuggestion</span></span>|<span data-ttu-id="1c42c-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c42c-199">Boolean</span></span>|<span data-ttu-id="1c42c-200">Определяет, разрешается ли использовать текстовые предложения во время выполнения теста.</span><span class="sxs-lookup"><span data-stu-id="1c42c-200">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="1c42c-201">локалгуестаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="1c42c-201">localGuestAccountName</span></span>|<span data-ttu-id="1c42c-202">String</span><span class="sxs-lookup"><span data-stu-id="1c42c-202">String</span></span>|<span data-ttu-id="1c42c-203">Указывает отображаемый текст для локальной гостевой учетной записи, отображаемой на экране входа.</span><span class="sxs-lookup"><span data-stu-id="1c42c-203">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="1c42c-204">Обычно это имя оценки.</span><span class="sxs-lookup"><span data-stu-id="1c42c-204">Typically is the name of an assessment.</span></span> <span data-ttu-id="1c42c-205">Когда пользователь нажимает на экране входа локальную гостевую учетную запись, запускается приложение для оценки с указанным URL-адресом оценки.</span><span class="sxs-lookup"><span data-stu-id="1c42c-205">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="1c42c-206">Для безопасной оценки можно использовать только локальную гостевую учетную запись на устройствах под управлением Windows 10 версии 1903 или более поздней.</span><span class="sxs-lookup"><span data-stu-id="1c42c-206">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="1c42c-207">Важное примечание. это свойство должно быть задано с помощью Ассессментаппусермоделид, чтобы обеспечить правильную работу локальной учетной записи гостя для обеспечения безопасной оценки.</span><span class="sxs-lookup"><span data-stu-id="1c42c-207">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="1c42c-208">ассессментаппусермоделид</span><span class="sxs-lookup"><span data-stu-id="1c42c-208">assessmentAppUserModelId</span></span>|<span data-ttu-id="1c42c-209">String</span><span class="sxs-lookup"><span data-stu-id="1c42c-209">String</span></span>|<span data-ttu-id="1c42c-210">Указывает идентификатор пользовательской модели приложения для оценки, запущенной при входе пользователя в систему для безопасной оценки с помощью локальной учетной записи гостя.</span><span class="sxs-lookup"><span data-stu-id="1c42c-210">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="1c42c-211">Важное примечание. это свойство должно быть задано с помощью Локалгуестаккаунтнаме, чтобы обеспечить правильную работу локальной учетной записи гостя для обеспечения безопасной оценки.</span><span class="sxs-lookup"><span data-stu-id="1c42c-211">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="1c42c-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c42c-212">Response</span></span>
<span data-ttu-id="1c42c-213">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1c42c-213">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c42c-214">Пример</span><span class="sxs-lookup"><span data-stu-id="1c42c-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c42c-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c42c-215">Request</span></span>
<span data-ttu-id="1c42c-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c42c-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1c42c-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c42c-217">Response</span></span>
<span data-ttu-id="1c42c-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c42c-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



