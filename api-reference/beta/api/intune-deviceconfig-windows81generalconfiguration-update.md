---
title: Update windows81GeneralConfiguration
description: Обновление свойств объекта windows81GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26436c15fd71d861d3326447375ac95b2b3c9f08
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974971"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="bba8b-103">Update windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="bba8b-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="bba8b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bba8b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bba8b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bba8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bba8b-106">Обновление свойств объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-106">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bba8b-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bba8b-107">Prerequisites</span></span>
<span data-ttu-id="bba8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bba8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bba8b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bba8b-110">Permission type</span></span>|<span data-ttu-id="bba8b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bba8b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bba8b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bba8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bba8b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bba8b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bba8b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bba8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bba8b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bba8b-115">Not supported.</span></span>|
|<span data-ttu-id="bba8b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bba8b-116">Application</span></span>|<span data-ttu-id="bba8b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bba8b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bba8b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bba8b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bba8b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bba8b-119">Request headers</span></span>
|<span data-ttu-id="bba8b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bba8b-120">Header</span></span>|<span data-ttu-id="bba8b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bba8b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bba8b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bba8b-122">Authorization</span></span>|<span data-ttu-id="bba8b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bba8b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bba8b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bba8b-124">Accept</span></span>|<span data-ttu-id="bba8b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bba8b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bba8b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bba8b-126">Request body</span></span>
<span data-ttu-id="bba8b-127">В тексте запроса добавьте представление объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bba8b-127">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="bba8b-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-128">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="bba8b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bba8b-129">Property</span></span>|<span data-ttu-id="bba8b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bba8b-130">Type</span></span>|<span data-ttu-id="bba8b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bba8b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bba8b-132">id</span><span class="sxs-lookup"><span data-stu-id="bba8b-132">id</span></span>|<span data-ttu-id="bba8b-133">Строка</span><span class="sxs-lookup"><span data-stu-id="bba8b-133">String</span></span>|<span data-ttu-id="bba8b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bba8b-134">Key of the entity.</span></span> <span data-ttu-id="bba8b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bba8b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bba8b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bba8b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bba8b-137">DateTimeOffset</span></span>|<span data-ttu-id="bba8b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bba8b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bba8b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bba8b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bba8b-140">roleScopeTagIds</span></span>|<span data-ttu-id="bba8b-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bba8b-141">String collection</span></span>|<span data-ttu-id="bba8b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bba8b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bba8b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bba8b-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="bba8b-144">supportsScopeTags</span></span>|<span data-ttu-id="bba8b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-145">Boolean</span></span>|<span data-ttu-id="bba8b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bba8b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bba8b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="bba8b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bba8b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bba8b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bba8b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bba8b-149">This property is read-only.</span></span> <span data-ttu-id="bba8b-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bba8b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bba8b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bba8b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bba8b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bba8b-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bba8b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bba8b-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bba8b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bba8b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bba8b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bba8b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bba8b-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bba8b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bba8b-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bba8b-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="bba8b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bba8b-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="bba8b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bba8b-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bba8b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bba8b-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bba8b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bba8b-163">createdDateTime</span></span>|<span data-ttu-id="bba8b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bba8b-164">DateTimeOffset</span></span>|<span data-ttu-id="bba8b-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bba8b-165">DateTime the object was created.</span></span> <span data-ttu-id="bba8b-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bba8b-167">description</span><span class="sxs-lookup"><span data-stu-id="bba8b-167">description</span></span>|<span data-ttu-id="bba8b-168">String</span><span class="sxs-lookup"><span data-stu-id="bba8b-168">String</span></span>|<span data-ttu-id="bba8b-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bba8b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bba8b-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bba8b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="bba8b-171">displayName</span></span>|<span data-ttu-id="bba8b-172">Строка</span><span class="sxs-lookup"><span data-stu-id="bba8b-172">String</span></span>|<span data-ttu-id="bba8b-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bba8b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bba8b-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bba8b-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bba8b-175">version</span><span class="sxs-lookup"><span data-stu-id="bba8b-175">version</span></span>|<span data-ttu-id="bba8b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="bba8b-176">Int32</span></span>|<span data-ttu-id="bba8b-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bba8b-177">Version of the device configuration.</span></span> <span data-ttu-id="bba8b-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bba8b-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bba8b-179">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="bba8b-179">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="bba8b-180">Логический</span><span class="sxs-lookup"><span data-stu-id="bba8b-180">Boolean</span></span>|<span data-ttu-id="bba8b-181">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bba8b-181">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="bba8b-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="bba8b-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="bba8b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-183">Boolean</span></span>|<span data-ttu-id="bba8b-184">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="bba8b-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="bba8b-185">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bba8b-185">This property is read-only.</span></span>|
|<span data-ttu-id="bba8b-186">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="bba8b-186">browserBlockAutofill</span></span>|<span data-ttu-id="bba8b-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-187">Boolean</span></span>|<span data-ttu-id="bba8b-188">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="bba8b-188">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="bba8b-189">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="bba8b-189">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="bba8b-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-190">Boolean</span></span>|<span data-ttu-id="bba8b-191">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="bba8b-191">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="bba8b-192">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="bba8b-192">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="bba8b-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-193">Boolean</span></span>|<span data-ttu-id="bba8b-194">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="bba8b-194">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="bba8b-195">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="bba8b-195">browserBlockJavaScript</span></span>|<span data-ttu-id="bba8b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-196">Boolean</span></span>|<span data-ttu-id="bba8b-197">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="bba8b-197">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="bba8b-198">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="bba8b-198">browserBlockPlugins</span></span>|<span data-ttu-id="bba8b-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-199">Boolean</span></span>|<span data-ttu-id="bba8b-200">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="bba8b-200">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="bba8b-201">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="bba8b-201">browserBlockPopups</span></span>|<span data-ttu-id="bba8b-202">Логический</span><span class="sxs-lookup"><span data-stu-id="bba8b-202">Boolean</span></span>|<span data-ttu-id="bba8b-203">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="bba8b-203">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="bba8b-204">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="bba8b-204">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="bba8b-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-205">Boolean</span></span>|<span data-ttu-id="bba8b-206">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="bba8b-206">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="bba8b-207">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="bba8b-207">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="bba8b-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-208">Boolean</span></span>|<span data-ttu-id="bba8b-209">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="bba8b-209">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="bba8b-210">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="bba8b-210">browserRequireSmartScreen</span></span>|<span data-ttu-id="bba8b-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-211">Boolean</span></span>|<span data-ttu-id="bba8b-212">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="bba8b-212">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="bba8b-213">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="bba8b-213">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="bba8b-214">String</span><span class="sxs-lookup"><span data-stu-id="bba8b-214">String</span></span>|<span data-ttu-id="bba8b-215">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="bba8b-215">The enterprise mode site list location.</span></span> <span data-ttu-id="bba8b-216">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="bba8b-216">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="bba8b-217">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="bba8b-217">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="bba8b-218">Интернетситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="bba8b-218">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="bba8b-219">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="bba8b-219">The internet security level.</span></span> <span data-ttu-id="bba8b-220">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="bba8b-220">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="bba8b-221">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="bba8b-221">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="bba8b-222">Ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="bba8b-222">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="bba8b-223">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="bba8b-223">The Intranet security level.</span></span> <span data-ttu-id="bba8b-224">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="bba8b-224">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="bba8b-225">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="bba8b-225">browserLoggingReportLocation</span></span>|<span data-ttu-id="bba8b-226">String</span><span class="sxs-lookup"><span data-stu-id="bba8b-226">String</span></span>|<span data-ttu-id="bba8b-227">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="bba8b-227">The logging report location.</span></span>|
|<span data-ttu-id="bba8b-228">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="bba8b-228">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="bba8b-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-229">Boolean</span></span>|<span data-ttu-id="bba8b-230">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="bba8b-230">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="bba8b-231">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="bba8b-231">browserRequireFirewall</span></span>|<span data-ttu-id="bba8b-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-232">Boolean</span></span>|<span data-ttu-id="bba8b-233">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="bba8b-233">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="bba8b-234">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="bba8b-234">browserRequireFraudWarning</span></span>|<span data-ttu-id="bba8b-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-235">Boolean</span></span>|<span data-ttu-id="bba8b-236">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="bba8b-236">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="bba8b-237">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="bba8b-237">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="bba8b-238">Ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="bba8b-238">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="bba8b-239">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="bba8b-239">The trusted sites security level.</span></span> <span data-ttu-id="bba8b-240">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="bba8b-240">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="bba8b-241">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="bba8b-241">cellularBlockDataRoaming</span></span>|<span data-ttu-id="bba8b-242">Логический</span><span class="sxs-lookup"><span data-stu-id="bba8b-242">Boolean</span></span>|<span data-ttu-id="bba8b-243">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="bba8b-243">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="bba8b-244">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="bba8b-244">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="bba8b-245">Логический</span><span class="sxs-lookup"><span data-stu-id="bba8b-245">Boolean</span></span>|<span data-ttu-id="bba8b-246">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="bba8b-246">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="bba8b-247">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="bba8b-247">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="bba8b-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-248">Boolean</span></span>|<span data-ttu-id="bba8b-249">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="bba8b-249">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="bba8b-250">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bba8b-250">passwordExpirationDays</span></span>|<span data-ttu-id="bba8b-251">Int32</span><span class="sxs-lookup"><span data-stu-id="bba8b-251">Int32</span></span>|<span data-ttu-id="bba8b-252">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="bba8b-252">Password expiration in days.</span></span>|
|<span data-ttu-id="bba8b-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bba8b-253">passwordMinimumLength</span></span>|<span data-ttu-id="bba8b-254">Int32</span><span class="sxs-lookup"><span data-stu-id="bba8b-254">Int32</span></span>|<span data-ttu-id="bba8b-255">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="bba8b-255">The minimum password length.</span></span>|
|<span data-ttu-id="bba8b-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="bba8b-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="bba8b-257">Int32</span><span class="sxs-lookup"><span data-stu-id="bba8b-257">Int32</span></span>|<span data-ttu-id="bba8b-258">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="bba8b-258">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="bba8b-259">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bba8b-259">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="bba8b-260">Int32</span><span class="sxs-lookup"><span data-stu-id="bba8b-260">Int32</span></span>|<span data-ttu-id="bba8b-261">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="bba8b-261">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="bba8b-262">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bba8b-262">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bba8b-263">Int32</span><span class="sxs-lookup"><span data-stu-id="bba8b-263">Int32</span></span>|<span data-ttu-id="bba8b-264">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="bba8b-264">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="bba8b-265">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="bba8b-265">Valid values 0 to 24</span></span>|
|<span data-ttu-id="bba8b-266">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bba8b-266">passwordRequiredType</span></span>|[<span data-ttu-id="bba8b-267">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="bba8b-267">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="bba8b-268">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="bba8b-268">The required password type.</span></span> <span data-ttu-id="bba8b-269">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="bba8b-269">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="bba8b-270">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="bba8b-270">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="bba8b-271">Int32</span><span class="sxs-lookup"><span data-stu-id="bba8b-271">Int32</span></span>|<span data-ttu-id="bba8b-272">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="bba8b-272">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="bba8b-273">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="bba8b-273">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="bba8b-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-274">Boolean</span></span>|<span data-ttu-id="bba8b-275">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="bba8b-275">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="bba8b-276">Минимумаутоинсталлклассификатион</span><span class="sxs-lookup"><span data-stu-id="bba8b-276">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="bba8b-277">Упдатеклассификатион</span><span class="sxs-lookup"><span data-stu-id="bba8b-277">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="bba8b-278">Минимальная Классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="bba8b-278">The minimum update classification to install automatically.</span></span> <span data-ttu-id="bba8b-279">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="bba8b-279">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="bba8b-280">Упдатесминимумаутоинсталлклассификатион</span><span class="sxs-lookup"><span data-stu-id="bba8b-280">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="bba8b-281">Упдатеклассификатион</span><span class="sxs-lookup"><span data-stu-id="bba8b-281">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="bba8b-282">Минимальная Классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="bba8b-282">The minimum update classification to install automatically.</span></span> <span data-ttu-id="bba8b-283">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="bba8b-283">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="bba8b-284">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="bba8b-284">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="bba8b-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba8b-285">Boolean</span></span>|<span data-ttu-id="bba8b-286">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="bba8b-286">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="bba8b-287">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="bba8b-287">userAccountControlSettings</span></span>|[<span data-ttu-id="bba8b-288">Виндовсусераккаунтконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="bba8b-288">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="bba8b-289">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="bba8b-289">The user account control settings.</span></span> <span data-ttu-id="bba8b-290">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="bba8b-290">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="bba8b-291">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="bba8b-291">workFoldersUrl</span></span>|<span data-ttu-id="bba8b-292">String</span><span class="sxs-lookup"><span data-stu-id="bba8b-292">String</span></span>|<span data-ttu-id="bba8b-293">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="bba8b-293">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="bba8b-294">Ответ</span><span class="sxs-lookup"><span data-stu-id="bba8b-294">Response</span></span>
<span data-ttu-id="bba8b-295">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bba8b-295">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bba8b-296">Пример</span><span class="sxs-lookup"><span data-stu-id="bba8b-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="bba8b-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="bba8b-297">Request</span></span>
<span data-ttu-id="bba8b-298">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bba8b-298">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bba8b-299">Отклик</span><span class="sxs-lookup"><span data-stu-id="bba8b-299">Response</span></span>
<span data-ttu-id="bba8b-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bba8b-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





