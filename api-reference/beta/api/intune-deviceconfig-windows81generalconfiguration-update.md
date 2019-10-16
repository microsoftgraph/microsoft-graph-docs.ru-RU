---
title: Update windows81GeneralConfiguration
description: Обновление свойств объекта windows81GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 781b85b26f1758b1eb39bedb59da4f20b3471c2e
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37532955"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="85392-103">Update windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="85392-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="85392-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85392-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85392-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85392-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85392-106">Обновление свойств объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-106">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85392-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="85392-107">Prerequisites</span></span>
<span data-ttu-id="85392-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85392-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85392-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85392-110">Permission type</span></span>|<span data-ttu-id="85392-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85392-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85392-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85392-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85392-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85392-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85392-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85392-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85392-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85392-115">Not supported.</span></span>|
|<span data-ttu-id="85392-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="85392-116">Application</span></span>|<span data-ttu-id="85392-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85392-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85392-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85392-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="85392-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85392-119">Request headers</span></span>
|<span data-ttu-id="85392-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85392-120">Header</span></span>|<span data-ttu-id="85392-121">Значение</span><span class="sxs-lookup"><span data-stu-id="85392-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85392-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85392-122">Authorization</span></span>|<span data-ttu-id="85392-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85392-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85392-124">Accept</span><span class="sxs-lookup"><span data-stu-id="85392-124">Accept</span></span>|<span data-ttu-id="85392-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85392-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85392-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85392-126">Request body</span></span>
<span data-ttu-id="85392-127">В тексте запроса добавьте представление объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85392-127">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="85392-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-128">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="85392-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="85392-129">Property</span></span>|<span data-ttu-id="85392-130">Тип</span><span class="sxs-lookup"><span data-stu-id="85392-130">Type</span></span>|<span data-ttu-id="85392-131">Описание</span><span class="sxs-lookup"><span data-stu-id="85392-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85392-132">id</span><span class="sxs-lookup"><span data-stu-id="85392-132">id</span></span>|<span data-ttu-id="85392-133">Строка</span><span class="sxs-lookup"><span data-stu-id="85392-133">String</span></span>|<span data-ttu-id="85392-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="85392-134">Key of the entity.</span></span> <span data-ttu-id="85392-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85392-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85392-136">lastModifiedDateTime</span></span>|<span data-ttu-id="85392-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85392-137">DateTimeOffset</span></span>|<span data-ttu-id="85392-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="85392-138">DateTime the object was last modified.</span></span> <span data-ttu-id="85392-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85392-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85392-140">roleScopeTagIds</span></span>|<span data-ttu-id="85392-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="85392-141">String collection</span></span>|<span data-ttu-id="85392-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="85392-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="85392-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85392-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="85392-144">supportsScopeTags</span></span>|<span data-ttu-id="85392-145">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-145">Boolean</span></span>|<span data-ttu-id="85392-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="85392-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="85392-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="85392-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="85392-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="85392-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="85392-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85392-149">This property is read-only.</span></span> <span data-ttu-id="85392-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85392-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="85392-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="85392-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="85392-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="85392-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="85392-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="85392-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85392-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="85392-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="85392-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="85392-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="85392-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="85392-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="85392-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85392-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="85392-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="85392-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="85392-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="85392-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="85392-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="85392-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85392-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85392-163">createdDateTime</span></span>|<span data-ttu-id="85392-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85392-164">DateTimeOffset</span></span>|<span data-ttu-id="85392-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="85392-165">DateTime the object was created.</span></span> <span data-ttu-id="85392-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85392-167">description</span><span class="sxs-lookup"><span data-stu-id="85392-167">description</span></span>|<span data-ttu-id="85392-168">String</span><span class="sxs-lookup"><span data-stu-id="85392-168">String</span></span>|<span data-ttu-id="85392-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="85392-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="85392-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85392-171">displayName</span><span class="sxs-lookup"><span data-stu-id="85392-171">displayName</span></span>|<span data-ttu-id="85392-172">Строка</span><span class="sxs-lookup"><span data-stu-id="85392-172">String</span></span>|<span data-ttu-id="85392-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="85392-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="85392-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85392-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85392-175">version</span><span class="sxs-lookup"><span data-stu-id="85392-175">version</span></span>|<span data-ttu-id="85392-176">Int32</span><span class="sxs-lookup"><span data-stu-id="85392-176">Int32</span></span>|<span data-ttu-id="85392-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="85392-177">Version of the device configuration.</span></span> <span data-ttu-id="85392-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85392-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85392-179">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="85392-179">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="85392-180">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-180">Boolean</span></span>|<span data-ttu-id="85392-181">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="85392-181">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="85392-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="85392-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="85392-183">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-183">Boolean</span></span>|<span data-ttu-id="85392-184">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="85392-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="85392-185">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85392-185">This property is read-only.</span></span>|
|<span data-ttu-id="85392-186">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="85392-186">browserBlockAutofill</span></span>|<span data-ttu-id="85392-187">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-187">Boolean</span></span>|<span data-ttu-id="85392-188">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="85392-188">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="85392-189">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="85392-189">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="85392-190">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-190">Boolean</span></span>|<span data-ttu-id="85392-191">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="85392-191">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="85392-192">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="85392-192">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="85392-193">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-193">Boolean</span></span>|<span data-ttu-id="85392-194">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="85392-194">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="85392-195">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="85392-195">browserBlockJavaScript</span></span>|<span data-ttu-id="85392-196">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-196">Boolean</span></span>|<span data-ttu-id="85392-197">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="85392-197">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="85392-198">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="85392-198">browserBlockPlugins</span></span>|<span data-ttu-id="85392-199">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-199">Boolean</span></span>|<span data-ttu-id="85392-200">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="85392-200">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="85392-201">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="85392-201">browserBlockPopups</span></span>|<span data-ttu-id="85392-202">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-202">Boolean</span></span>|<span data-ttu-id="85392-203">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="85392-203">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="85392-204">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="85392-204">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="85392-205">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-205">Boolean</span></span>|<span data-ttu-id="85392-206">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="85392-206">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="85392-207">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="85392-207">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="85392-208">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-208">Boolean</span></span>|<span data-ttu-id="85392-209">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="85392-209">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="85392-210">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="85392-210">browserRequireSmartScreen</span></span>|<span data-ttu-id="85392-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="85392-211">Boolean</span></span>|<span data-ttu-id="85392-212">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="85392-212">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="85392-213">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="85392-213">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="85392-214">String</span><span class="sxs-lookup"><span data-stu-id="85392-214">String</span></span>|<span data-ttu-id="85392-215">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="85392-215">The enterprise mode site list location.</span></span> <span data-ttu-id="85392-216">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="85392-216">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="85392-217">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="85392-217">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="85392-218">интернетситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="85392-218">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="85392-219">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="85392-219">The internet security level.</span></span> <span data-ttu-id="85392-220">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="85392-220">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="85392-221">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="85392-221">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="85392-222">ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="85392-222">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="85392-223">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="85392-223">The Intranet security level.</span></span> <span data-ttu-id="85392-224">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="85392-224">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="85392-225">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="85392-225">browserLoggingReportLocation</span></span>|<span data-ttu-id="85392-226">String</span><span class="sxs-lookup"><span data-stu-id="85392-226">String</span></span>|<span data-ttu-id="85392-227">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="85392-227">The logging report location.</span></span>|
|<span data-ttu-id="85392-228">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="85392-228">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="85392-229">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-229">Boolean</span></span>|<span data-ttu-id="85392-230">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="85392-230">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="85392-231">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="85392-231">browserRequireFirewall</span></span>|<span data-ttu-id="85392-232">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-232">Boolean</span></span>|<span data-ttu-id="85392-233">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="85392-233">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="85392-234">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="85392-234">browserRequireFraudWarning</span></span>|<span data-ttu-id="85392-235">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-235">Boolean</span></span>|<span data-ttu-id="85392-236">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="85392-236">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="85392-237">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="85392-237">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="85392-238">ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="85392-238">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="85392-239">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="85392-239">The trusted sites security level.</span></span> <span data-ttu-id="85392-240">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="85392-240">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="85392-241">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="85392-241">cellularBlockDataRoaming</span></span>|<span data-ttu-id="85392-242">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-242">Boolean</span></span>|<span data-ttu-id="85392-243">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="85392-243">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="85392-244">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="85392-244">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="85392-245">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-245">Boolean</span></span>|<span data-ttu-id="85392-246">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="85392-246">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="85392-247">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="85392-247">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="85392-248">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-248">Boolean</span></span>|<span data-ttu-id="85392-249">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="85392-249">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="85392-250">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="85392-250">passwordExpirationDays</span></span>|<span data-ttu-id="85392-251">Int32</span><span class="sxs-lookup"><span data-stu-id="85392-251">Int32</span></span>|<span data-ttu-id="85392-252">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="85392-252">Password expiration in days.</span></span>|
|<span data-ttu-id="85392-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="85392-253">passwordMinimumLength</span></span>|<span data-ttu-id="85392-254">Int32</span><span class="sxs-lookup"><span data-stu-id="85392-254">Int32</span></span>|<span data-ttu-id="85392-255">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="85392-255">The minimum password length.</span></span>|
|<span data-ttu-id="85392-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="85392-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="85392-257">Int32</span><span class="sxs-lookup"><span data-stu-id="85392-257">Int32</span></span>|<span data-ttu-id="85392-258">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="85392-258">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="85392-259">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="85392-259">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="85392-260">Int32</span><span class="sxs-lookup"><span data-stu-id="85392-260">Int32</span></span>|<span data-ttu-id="85392-261">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="85392-261">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="85392-262">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="85392-262">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="85392-263">Int32</span><span class="sxs-lookup"><span data-stu-id="85392-263">Int32</span></span>|<span data-ttu-id="85392-264">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="85392-264">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="85392-265">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="85392-265">Valid values 0 to 24</span></span>|
|<span data-ttu-id="85392-266">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="85392-266">passwordRequiredType</span></span>|[<span data-ttu-id="85392-267">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="85392-267">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="85392-268">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="85392-268">The required password type.</span></span> <span data-ttu-id="85392-269">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="85392-269">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="85392-270">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="85392-270">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="85392-271">Int32</span><span class="sxs-lookup"><span data-stu-id="85392-271">Int32</span></span>|<span data-ttu-id="85392-272">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="85392-272">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="85392-273">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="85392-273">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="85392-274">Логический</span><span class="sxs-lookup"><span data-stu-id="85392-274">Boolean</span></span>|<span data-ttu-id="85392-275">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="85392-275">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="85392-276">минимумаутоинсталлклассификатион</span><span class="sxs-lookup"><span data-stu-id="85392-276">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="85392-277">упдатеклассификатион</span><span class="sxs-lookup"><span data-stu-id="85392-277">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="85392-278">Минимальная Классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="85392-278">The minimum update classification to install automatically.</span></span> <span data-ttu-id="85392-279">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="85392-279">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="85392-280">упдатесминимумаутоинсталлклассификатион</span><span class="sxs-lookup"><span data-stu-id="85392-280">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="85392-281">упдатеклассификатион</span><span class="sxs-lookup"><span data-stu-id="85392-281">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="85392-282">Минимальная Классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="85392-282">The minimum update classification to install automatically.</span></span> <span data-ttu-id="85392-283">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="85392-283">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="85392-284">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="85392-284">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="85392-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="85392-285">Boolean</span></span>|<span data-ttu-id="85392-286">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="85392-286">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="85392-287">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="85392-287">userAccountControlSettings</span></span>|[<span data-ttu-id="85392-288">виндовсусераккаунтконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="85392-288">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="85392-289">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="85392-289">The user account control settings.</span></span> <span data-ttu-id="85392-290">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="85392-290">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="85392-291">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="85392-291">workFoldersUrl</span></span>|<span data-ttu-id="85392-292">String</span><span class="sxs-lookup"><span data-stu-id="85392-292">String</span></span>|<span data-ttu-id="85392-293">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="85392-293">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="85392-294">Ответ</span><span class="sxs-lookup"><span data-stu-id="85392-294">Response</span></span>
<span data-ttu-id="85392-295">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="85392-295">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85392-296">Пример</span><span class="sxs-lookup"><span data-stu-id="85392-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="85392-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="85392-297">Request</span></span>
<span data-ttu-id="85392-298">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85392-298">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="85392-299">Отклик</span><span class="sxs-lookup"><span data-stu-id="85392-299">Response</span></span>
<span data-ttu-id="85392-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85392-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






