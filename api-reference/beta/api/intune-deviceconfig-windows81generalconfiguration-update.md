---
title: Update windows81GeneralConfiguration
description: Обновление свойств объекта windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 109f111cdf0042fd50cd5107d1b04833f7f4ec4c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147345"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="55230-103">Update windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="55230-103">Update windows81GeneralConfiguration</span></span>

<span data-ttu-id="55230-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55230-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55230-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55230-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55230-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55230-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55230-107">Обновление свойств объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-107">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55230-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="55230-108">Prerequisites</span></span>
<span data-ttu-id="55230-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55230-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55230-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55230-111">Permission type</span></span>|<span data-ttu-id="55230-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55230-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55230-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55230-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55230-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55230-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55230-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55230-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55230-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55230-116">Not supported.</span></span>|
|<span data-ttu-id="55230-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="55230-117">Application</span></span>|<span data-ttu-id="55230-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55230-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55230-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55230-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="55230-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="55230-120">Request headers</span></span>
|<span data-ttu-id="55230-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55230-121">Header</span></span>|<span data-ttu-id="55230-122">Значение</span><span class="sxs-lookup"><span data-stu-id="55230-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55230-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55230-123">Authorization</span></span>|<span data-ttu-id="55230-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55230-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55230-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55230-125">Accept</span></span>|<span data-ttu-id="55230-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55230-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55230-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55230-127">Request body</span></span>
<span data-ttu-id="55230-128">В тексте запроса добавьте представление объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55230-128">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="55230-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-129">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="55230-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="55230-130">Property</span></span>|<span data-ttu-id="55230-131">Тип</span><span class="sxs-lookup"><span data-stu-id="55230-131">Type</span></span>|<span data-ttu-id="55230-132">Описание</span><span class="sxs-lookup"><span data-stu-id="55230-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55230-133">id</span><span class="sxs-lookup"><span data-stu-id="55230-133">id</span></span>|<span data-ttu-id="55230-134">Строка</span><span class="sxs-lookup"><span data-stu-id="55230-134">String</span></span>|<span data-ttu-id="55230-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="55230-135">Key of the entity.</span></span> <span data-ttu-id="55230-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55230-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55230-137">lastModifiedDateTime</span></span>|<span data-ttu-id="55230-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55230-138">DateTimeOffset</span></span>|<span data-ttu-id="55230-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="55230-139">DateTime the object was last modified.</span></span> <span data-ttu-id="55230-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55230-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="55230-141">roleScopeTagIds</span></span>|<span data-ttu-id="55230-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="55230-142">String collection</span></span>|<span data-ttu-id="55230-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="55230-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="55230-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55230-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="55230-145">supportsScopeTags</span></span>|<span data-ttu-id="55230-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-146">Boolean</span></span>|<span data-ttu-id="55230-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="55230-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="55230-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="55230-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="55230-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="55230-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="55230-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55230-150">This property is read-only.</span></span> <span data-ttu-id="55230-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55230-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="55230-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="55230-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="55230-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="55230-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="55230-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="55230-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55230-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="55230-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="55230-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="55230-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="55230-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="55230-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="55230-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55230-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="55230-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="55230-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="55230-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="55230-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="55230-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="55230-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55230-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55230-164">createdDateTime</span></span>|<span data-ttu-id="55230-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55230-165">DateTimeOffset</span></span>|<span data-ttu-id="55230-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="55230-166">DateTime the object was created.</span></span> <span data-ttu-id="55230-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55230-168">description</span><span class="sxs-lookup"><span data-stu-id="55230-168">description</span></span>|<span data-ttu-id="55230-169">Строка</span><span class="sxs-lookup"><span data-stu-id="55230-169">String</span></span>|<span data-ttu-id="55230-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="55230-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="55230-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55230-172">displayName</span><span class="sxs-lookup"><span data-stu-id="55230-172">displayName</span></span>|<span data-ttu-id="55230-173">Строка</span><span class="sxs-lookup"><span data-stu-id="55230-173">String</span></span>|<span data-ttu-id="55230-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="55230-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="55230-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="55230-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55230-176">version</span><span class="sxs-lookup"><span data-stu-id="55230-176">version</span></span>|<span data-ttu-id="55230-177">Int32</span><span class="sxs-lookup"><span data-stu-id="55230-177">Int32</span></span>|<span data-ttu-id="55230-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="55230-178">Version of the device configuration.</span></span> <span data-ttu-id="55230-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="55230-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="55230-180">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="55230-180">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="55230-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-181">Boolean</span></span>|<span data-ttu-id="55230-182">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="55230-182">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="55230-183">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="55230-183">applyOnlyToWindows81</span></span>|<span data-ttu-id="55230-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-184">Boolean</span></span>|<span data-ttu-id="55230-185">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="55230-185">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="55230-186">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55230-186">This property is read-only.</span></span>|
|<span data-ttu-id="55230-187">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="55230-187">browserBlockAutofill</span></span>|<span data-ttu-id="55230-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-188">Boolean</span></span>|<span data-ttu-id="55230-189">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="55230-189">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="55230-190">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="55230-190">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="55230-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-191">Boolean</span></span>|<span data-ttu-id="55230-192">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="55230-192">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="55230-193">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="55230-193">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="55230-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-194">Boolean</span></span>|<span data-ttu-id="55230-195">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="55230-195">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="55230-196">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="55230-196">browserBlockJavaScript</span></span>|<span data-ttu-id="55230-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-197">Boolean</span></span>|<span data-ttu-id="55230-198">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="55230-198">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="55230-199">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="55230-199">browserBlockPlugins</span></span>|<span data-ttu-id="55230-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-200">Boolean</span></span>|<span data-ttu-id="55230-201">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="55230-201">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="55230-202">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="55230-202">browserBlockPopups</span></span>|<span data-ttu-id="55230-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-203">Boolean</span></span>|<span data-ttu-id="55230-204">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="55230-204">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="55230-205">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="55230-205">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="55230-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-206">Boolean</span></span>|<span data-ttu-id="55230-207">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="55230-207">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="55230-208">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="55230-208">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="55230-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-209">Boolean</span></span>|<span data-ttu-id="55230-210">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="55230-210">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="55230-211">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="55230-211">browserRequireSmartScreen</span></span>|<span data-ttu-id="55230-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-212">Boolean</span></span>|<span data-ttu-id="55230-213">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="55230-213">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="55230-214">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="55230-214">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="55230-215">String</span><span class="sxs-lookup"><span data-stu-id="55230-215">String</span></span>|<span data-ttu-id="55230-216">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="55230-216">The enterprise mode site list location.</span></span> <span data-ttu-id="55230-217">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="55230-217">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="55230-218">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55230-218">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="55230-219">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55230-219">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="55230-220">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="55230-220">The internet security level.</span></span> <span data-ttu-id="55230-221">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="55230-221">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="55230-222">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55230-222">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="55230-223">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55230-223">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="55230-224">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="55230-224">The Intranet security level.</span></span> <span data-ttu-id="55230-225">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="55230-225">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="55230-226">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="55230-226">browserLoggingReportLocation</span></span>|<span data-ttu-id="55230-227">String</span><span class="sxs-lookup"><span data-stu-id="55230-227">String</span></span>|<span data-ttu-id="55230-228">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="55230-228">The logging report location.</span></span>|
|<span data-ttu-id="55230-229">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="55230-229">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="55230-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-230">Boolean</span></span>|<span data-ttu-id="55230-231">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="55230-231">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="55230-232">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="55230-232">browserRequireFirewall</span></span>|<span data-ttu-id="55230-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-233">Boolean</span></span>|<span data-ttu-id="55230-234">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="55230-234">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="55230-235">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="55230-235">browserRequireFraudWarning</span></span>|<span data-ttu-id="55230-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-236">Boolean</span></span>|<span data-ttu-id="55230-237">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="55230-237">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="55230-238">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55230-238">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="55230-239">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55230-239">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="55230-240">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="55230-240">The trusted sites security level.</span></span> <span data-ttu-id="55230-241">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="55230-241">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="55230-242">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="55230-242">cellularBlockDataRoaming</span></span>|<span data-ttu-id="55230-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-243">Boolean</span></span>|<span data-ttu-id="55230-244">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="55230-244">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="55230-245">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="55230-245">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="55230-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-246">Boolean</span></span>|<span data-ttu-id="55230-247">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="55230-247">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="55230-248">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="55230-248">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="55230-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-249">Boolean</span></span>|<span data-ttu-id="55230-250">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="55230-250">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="55230-251">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="55230-251">passwordExpirationDays</span></span>|<span data-ttu-id="55230-252">Int32</span><span class="sxs-lookup"><span data-stu-id="55230-252">Int32</span></span>|<span data-ttu-id="55230-253">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="55230-253">Password expiration in days.</span></span>|
|<span data-ttu-id="55230-254">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="55230-254">passwordMinimumLength</span></span>|<span data-ttu-id="55230-255">Int32</span><span class="sxs-lookup"><span data-stu-id="55230-255">Int32</span></span>|<span data-ttu-id="55230-256">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="55230-256">The minimum password length.</span></span>|
|<span data-ttu-id="55230-257">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="55230-257">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="55230-258">Int32</span><span class="sxs-lookup"><span data-stu-id="55230-258">Int32</span></span>|<span data-ttu-id="55230-259">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="55230-259">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="55230-260">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="55230-260">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="55230-261">Int32</span><span class="sxs-lookup"><span data-stu-id="55230-261">Int32</span></span>|<span data-ttu-id="55230-262">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="55230-262">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="55230-263">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="55230-263">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="55230-264">Int32</span><span class="sxs-lookup"><span data-stu-id="55230-264">Int32</span></span>|<span data-ttu-id="55230-265">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="55230-265">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="55230-266">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="55230-266">Valid values 0 to 24</span></span>|
|<span data-ttu-id="55230-267">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="55230-267">passwordRequiredType</span></span>|[<span data-ttu-id="55230-268">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="55230-268">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="55230-269">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="55230-269">The required password type.</span></span> <span data-ttu-id="55230-270">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="55230-270">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="55230-271">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="55230-271">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="55230-272">Int32</span><span class="sxs-lookup"><span data-stu-id="55230-272">Int32</span></span>|<span data-ttu-id="55230-273">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="55230-273">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="55230-274">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="55230-274">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="55230-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-275">Boolean</span></span>|<span data-ttu-id="55230-276">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="55230-276">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="55230-277">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="55230-277">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="55230-278">updateClassification</span><span class="sxs-lookup"><span data-stu-id="55230-278">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="55230-279">Минимальная классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="55230-279">The minimum update classification to install automatically.</span></span> <span data-ttu-id="55230-280">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="55230-280">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="55230-281">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="55230-281">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="55230-282">updateClassification</span><span class="sxs-lookup"><span data-stu-id="55230-282">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="55230-283">Минимальная классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="55230-283">The minimum update classification to install automatically.</span></span> <span data-ttu-id="55230-284">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="55230-284">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="55230-285">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="55230-285">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="55230-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="55230-286">Boolean</span></span>|<span data-ttu-id="55230-287">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="55230-287">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="55230-288">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="55230-288">userAccountControlSettings</span></span>|[<span data-ttu-id="55230-289">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="55230-289">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="55230-290">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="55230-290">The user account control settings.</span></span> <span data-ttu-id="55230-291">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="55230-291">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="55230-292">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="55230-292">workFoldersUrl</span></span>|<span data-ttu-id="55230-293">String</span><span class="sxs-lookup"><span data-stu-id="55230-293">String</span></span>|<span data-ttu-id="55230-294">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="55230-294">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="55230-295">Ответ</span><span class="sxs-lookup"><span data-stu-id="55230-295">Response</span></span>
<span data-ttu-id="55230-296">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="55230-296">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55230-297">Пример</span><span class="sxs-lookup"><span data-stu-id="55230-297">Example</span></span>

### <a name="request"></a><span data-ttu-id="55230-298">Запрос</span><span class="sxs-lookup"><span data-stu-id="55230-298">Request</span></span>
<span data-ttu-id="55230-299">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55230-299">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2697

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
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
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="55230-300">Отклик</span><span class="sxs-lookup"><span data-stu-id="55230-300">Response</span></span>
<span data-ttu-id="55230-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55230-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2869

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
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
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```




