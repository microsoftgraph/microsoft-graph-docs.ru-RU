---
title: Update windows81GeneralConfiguration
description: Обновление свойств объекта windows81GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b1eb084192aac9ed7d8f8f2827cb979b8c3424d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962234"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="70072-103">Update windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="70072-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="70072-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70072-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70072-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70072-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70072-106">Обновление свойств объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-106">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70072-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="70072-107">Prerequisites</span></span>
<span data-ttu-id="70072-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70072-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70072-110">Permission type</span></span>|<span data-ttu-id="70072-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70072-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70072-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70072-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70072-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70072-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="70072-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70072-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70072-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70072-115">Not supported.</span></span>|
|<span data-ttu-id="70072-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70072-116">Application</span></span>|<span data-ttu-id="70072-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70072-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70072-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70072-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="70072-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70072-119">Request headers</span></span>
|<span data-ttu-id="70072-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70072-120">Header</span></span>|<span data-ttu-id="70072-121">Значение</span><span class="sxs-lookup"><span data-stu-id="70072-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70072-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70072-122">Authorization</span></span>|<span data-ttu-id="70072-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70072-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70072-124">Accept</span><span class="sxs-lookup"><span data-stu-id="70072-124">Accept</span></span>|<span data-ttu-id="70072-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70072-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70072-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70072-126">Request body</span></span>
<span data-ttu-id="70072-127">В тексте запроса добавьте представление объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70072-127">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="70072-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-128">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="70072-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="70072-129">Property</span></span>|<span data-ttu-id="70072-130">Тип</span><span class="sxs-lookup"><span data-stu-id="70072-130">Type</span></span>|<span data-ttu-id="70072-131">Описание</span><span class="sxs-lookup"><span data-stu-id="70072-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70072-132">id</span><span class="sxs-lookup"><span data-stu-id="70072-132">id</span></span>|<span data-ttu-id="70072-133">Строка</span><span class="sxs-lookup"><span data-stu-id="70072-133">String</span></span>|<span data-ttu-id="70072-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="70072-134">Key of the entity.</span></span> <span data-ttu-id="70072-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70072-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70072-136">lastModifiedDateTime</span></span>|<span data-ttu-id="70072-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70072-137">DateTimeOffset</span></span>|<span data-ttu-id="70072-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="70072-138">DateTime the object was last modified.</span></span> <span data-ttu-id="70072-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70072-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="70072-140">roleScopeTagIds</span></span>|<span data-ttu-id="70072-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="70072-141">String collection</span></span>|<span data-ttu-id="70072-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="70072-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="70072-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70072-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="70072-144">supportsScopeTags</span></span>|<span data-ttu-id="70072-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-145">Boolean</span></span>|<span data-ttu-id="70072-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="70072-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="70072-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="70072-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="70072-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="70072-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="70072-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70072-149">This property is read-only.</span></span> <span data-ttu-id="70072-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70072-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="70072-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="70072-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="70072-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="70072-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="70072-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="70072-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70072-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="70072-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="70072-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="70072-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="70072-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="70072-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="70072-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70072-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="70072-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="70072-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="70072-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="70072-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="70072-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="70072-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70072-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70072-163">createdDateTime</span></span>|<span data-ttu-id="70072-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70072-164">DateTimeOffset</span></span>|<span data-ttu-id="70072-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="70072-165">DateTime the object was created.</span></span> <span data-ttu-id="70072-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70072-167">description</span><span class="sxs-lookup"><span data-stu-id="70072-167">description</span></span>|<span data-ttu-id="70072-168">String</span><span class="sxs-lookup"><span data-stu-id="70072-168">String</span></span>|<span data-ttu-id="70072-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="70072-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="70072-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70072-171">displayName</span><span class="sxs-lookup"><span data-stu-id="70072-171">displayName</span></span>|<span data-ttu-id="70072-172">Строка</span><span class="sxs-lookup"><span data-stu-id="70072-172">String</span></span>|<span data-ttu-id="70072-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="70072-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="70072-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70072-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70072-175">version</span><span class="sxs-lookup"><span data-stu-id="70072-175">version</span></span>|<span data-ttu-id="70072-176">Int32</span><span class="sxs-lookup"><span data-stu-id="70072-176">Int32</span></span>|<span data-ttu-id="70072-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="70072-177">Version of the device configuration.</span></span> <span data-ttu-id="70072-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70072-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70072-179">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="70072-179">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="70072-180">Логический</span><span class="sxs-lookup"><span data-stu-id="70072-180">Boolean</span></span>|<span data-ttu-id="70072-181">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="70072-181">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="70072-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="70072-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="70072-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-183">Boolean</span></span>|<span data-ttu-id="70072-184">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="70072-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="70072-185">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70072-185">This property is read-only.</span></span>|
|<span data-ttu-id="70072-186">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="70072-186">browserBlockAutofill</span></span>|<span data-ttu-id="70072-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-187">Boolean</span></span>|<span data-ttu-id="70072-188">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="70072-188">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="70072-189">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="70072-189">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="70072-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-190">Boolean</span></span>|<span data-ttu-id="70072-191">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="70072-191">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="70072-192">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="70072-192">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="70072-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-193">Boolean</span></span>|<span data-ttu-id="70072-194">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="70072-194">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="70072-195">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="70072-195">browserBlockJavaScript</span></span>|<span data-ttu-id="70072-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-196">Boolean</span></span>|<span data-ttu-id="70072-197">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="70072-197">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="70072-198">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="70072-198">browserBlockPlugins</span></span>|<span data-ttu-id="70072-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-199">Boolean</span></span>|<span data-ttu-id="70072-200">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="70072-200">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="70072-201">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="70072-201">browserBlockPopups</span></span>|<span data-ttu-id="70072-202">Логический</span><span class="sxs-lookup"><span data-stu-id="70072-202">Boolean</span></span>|<span data-ttu-id="70072-203">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="70072-203">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="70072-204">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="70072-204">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="70072-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-205">Boolean</span></span>|<span data-ttu-id="70072-206">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="70072-206">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="70072-207">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="70072-207">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="70072-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-208">Boolean</span></span>|<span data-ttu-id="70072-209">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="70072-209">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="70072-210">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="70072-210">browserRequireSmartScreen</span></span>|<span data-ttu-id="70072-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-211">Boolean</span></span>|<span data-ttu-id="70072-212">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="70072-212">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="70072-213">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="70072-213">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="70072-214">String</span><span class="sxs-lookup"><span data-stu-id="70072-214">String</span></span>|<span data-ttu-id="70072-215">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="70072-215">The enterprise mode site list location.</span></span> <span data-ttu-id="70072-216">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="70072-216">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="70072-217">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="70072-217">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="70072-218">Интернетситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="70072-218">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="70072-219">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="70072-219">The internet security level.</span></span> <span data-ttu-id="70072-220">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="70072-220">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="70072-221">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="70072-221">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="70072-222">Ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="70072-222">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="70072-223">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="70072-223">The Intranet security level.</span></span> <span data-ttu-id="70072-224">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="70072-224">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="70072-225">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="70072-225">browserLoggingReportLocation</span></span>|<span data-ttu-id="70072-226">String</span><span class="sxs-lookup"><span data-stu-id="70072-226">String</span></span>|<span data-ttu-id="70072-227">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="70072-227">The logging report location.</span></span>|
|<span data-ttu-id="70072-228">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="70072-228">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="70072-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-229">Boolean</span></span>|<span data-ttu-id="70072-230">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="70072-230">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="70072-231">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="70072-231">browserRequireFirewall</span></span>|<span data-ttu-id="70072-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-232">Boolean</span></span>|<span data-ttu-id="70072-233">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="70072-233">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="70072-234">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="70072-234">browserRequireFraudWarning</span></span>|<span data-ttu-id="70072-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-235">Boolean</span></span>|<span data-ttu-id="70072-236">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="70072-236">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="70072-237">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="70072-237">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="70072-238">Ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="70072-238">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="70072-239">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="70072-239">The trusted sites security level.</span></span> <span data-ttu-id="70072-240">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="70072-240">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="70072-241">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="70072-241">cellularBlockDataRoaming</span></span>|<span data-ttu-id="70072-242">Логический</span><span class="sxs-lookup"><span data-stu-id="70072-242">Boolean</span></span>|<span data-ttu-id="70072-243">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="70072-243">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="70072-244">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="70072-244">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="70072-245">Логический</span><span class="sxs-lookup"><span data-stu-id="70072-245">Boolean</span></span>|<span data-ttu-id="70072-246">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="70072-246">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="70072-247">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="70072-247">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="70072-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-248">Boolean</span></span>|<span data-ttu-id="70072-249">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="70072-249">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="70072-250">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="70072-250">passwordExpirationDays</span></span>|<span data-ttu-id="70072-251">Int32</span><span class="sxs-lookup"><span data-stu-id="70072-251">Int32</span></span>|<span data-ttu-id="70072-252">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="70072-252">Password expiration in days.</span></span>|
|<span data-ttu-id="70072-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="70072-253">passwordMinimumLength</span></span>|<span data-ttu-id="70072-254">Int32</span><span class="sxs-lookup"><span data-stu-id="70072-254">Int32</span></span>|<span data-ttu-id="70072-255">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="70072-255">The minimum password length.</span></span>|
|<span data-ttu-id="70072-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="70072-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="70072-257">Int32</span><span class="sxs-lookup"><span data-stu-id="70072-257">Int32</span></span>|<span data-ttu-id="70072-258">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="70072-258">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="70072-259">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="70072-259">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="70072-260">Int32</span><span class="sxs-lookup"><span data-stu-id="70072-260">Int32</span></span>|<span data-ttu-id="70072-261">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="70072-261">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="70072-262">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="70072-262">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="70072-263">Int32</span><span class="sxs-lookup"><span data-stu-id="70072-263">Int32</span></span>|<span data-ttu-id="70072-264">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="70072-264">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="70072-265">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="70072-265">Valid values 0 to 24</span></span>|
|<span data-ttu-id="70072-266">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="70072-266">passwordRequiredType</span></span>|[<span data-ttu-id="70072-267">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="70072-267">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="70072-268">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="70072-268">The required password type.</span></span> <span data-ttu-id="70072-269">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="70072-269">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="70072-270">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="70072-270">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="70072-271">Int32</span><span class="sxs-lookup"><span data-stu-id="70072-271">Int32</span></span>|<span data-ttu-id="70072-272">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="70072-272">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="70072-273">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="70072-273">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="70072-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-274">Boolean</span></span>|<span data-ttu-id="70072-275">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="70072-275">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="70072-276">Минимумаутоинсталлклассификатион</span><span class="sxs-lookup"><span data-stu-id="70072-276">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="70072-277">Упдатеклассификатион</span><span class="sxs-lookup"><span data-stu-id="70072-277">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="70072-278">Минимальная Классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="70072-278">The minimum update classification to install automatically.</span></span> <span data-ttu-id="70072-279">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="70072-279">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="70072-280">Упдатесминимумаутоинсталлклассификатион</span><span class="sxs-lookup"><span data-stu-id="70072-280">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="70072-281">Упдатеклассификатион</span><span class="sxs-lookup"><span data-stu-id="70072-281">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="70072-282">Минимальная Классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="70072-282">The minimum update classification to install automatically.</span></span> <span data-ttu-id="70072-283">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="70072-283">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="70072-284">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="70072-284">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="70072-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="70072-285">Boolean</span></span>|<span data-ttu-id="70072-286">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="70072-286">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="70072-287">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="70072-287">userAccountControlSettings</span></span>|[<span data-ttu-id="70072-288">Виндовсусераккаунтконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="70072-288">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="70072-289">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="70072-289">The user account control settings.</span></span> <span data-ttu-id="70072-290">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="70072-290">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="70072-291">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="70072-291">workFoldersUrl</span></span>|<span data-ttu-id="70072-292">String</span><span class="sxs-lookup"><span data-stu-id="70072-292">String</span></span>|<span data-ttu-id="70072-293">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="70072-293">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="70072-294">Ответ</span><span class="sxs-lookup"><span data-stu-id="70072-294">Response</span></span>
<span data-ttu-id="70072-295">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="70072-295">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70072-296">Пример</span><span class="sxs-lookup"><span data-stu-id="70072-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="70072-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="70072-297">Request</span></span>
<span data-ttu-id="70072-298">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70072-298">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="70072-299">Отклик</span><span class="sxs-lookup"><span data-stu-id="70072-299">Response</span></span>
<span data-ttu-id="70072-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70072-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





