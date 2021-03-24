---
title: Создание windows81GeneralConfiguration
description: Создание объекта windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8376bf7b1afbb37656adbfe002ce6cb20be551eb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147401"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="24132-103">Создание windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="24132-103">Create windows81GeneralConfiguration</span></span>

<span data-ttu-id="24132-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24132-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24132-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24132-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24132-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24132-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24132-107">Создание объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24132-107">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24132-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="24132-108">Prerequisites</span></span>
<span data-ttu-id="24132-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24132-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24132-111">Permission type</span></span>|<span data-ttu-id="24132-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24132-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24132-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24132-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24132-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24132-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24132-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24132-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24132-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24132-116">Not supported.</span></span>|
|<span data-ttu-id="24132-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="24132-117">Application</span></span>|<span data-ttu-id="24132-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24132-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24132-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24132-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="24132-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24132-120">Request headers</span></span>
|<span data-ttu-id="24132-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24132-121">Header</span></span>|<span data-ttu-id="24132-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24132-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24132-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24132-123">Authorization</span></span>|<span data-ttu-id="24132-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24132-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24132-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24132-125">Accept</span></span>|<span data-ttu-id="24132-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24132-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24132-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24132-127">Request body</span></span>
<span data-ttu-id="24132-128">В теле запроса добавьте представление объекта windows81GeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24132-128">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="24132-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="24132-129">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="24132-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="24132-130">Property</span></span>|<span data-ttu-id="24132-131">Тип</span><span class="sxs-lookup"><span data-stu-id="24132-131">Type</span></span>|<span data-ttu-id="24132-132">Описание</span><span class="sxs-lookup"><span data-stu-id="24132-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24132-133">id</span><span class="sxs-lookup"><span data-stu-id="24132-133">id</span></span>|<span data-ttu-id="24132-134">Строка</span><span class="sxs-lookup"><span data-stu-id="24132-134">String</span></span>|<span data-ttu-id="24132-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="24132-135">Key of the entity.</span></span> <span data-ttu-id="24132-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24132-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24132-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24132-137">lastModifiedDateTime</span></span>|<span data-ttu-id="24132-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24132-138">DateTimeOffset</span></span>|<span data-ttu-id="24132-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="24132-139">DateTime the object was last modified.</span></span> <span data-ttu-id="24132-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24132-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24132-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="24132-141">roleScopeTagIds</span></span>|<span data-ttu-id="24132-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="24132-142">String collection</span></span>|<span data-ttu-id="24132-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="24132-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="24132-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24132-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24132-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="24132-145">supportsScopeTags</span></span>|<span data-ttu-id="24132-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-146">Boolean</span></span>|<span data-ttu-id="24132-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="24132-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="24132-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="24132-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="24132-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="24132-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="24132-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="24132-150">This property is read-only.</span></span> <span data-ttu-id="24132-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24132-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24132-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="24132-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="24132-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="24132-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="24132-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="24132-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="24132-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24132-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24132-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="24132-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="24132-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="24132-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="24132-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="24132-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="24132-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24132-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24132-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="24132-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="24132-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="24132-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="24132-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="24132-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="24132-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24132-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24132-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24132-164">createdDateTime</span></span>|<span data-ttu-id="24132-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24132-165">DateTimeOffset</span></span>|<span data-ttu-id="24132-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="24132-166">DateTime the object was created.</span></span> <span data-ttu-id="24132-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24132-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24132-168">description</span><span class="sxs-lookup"><span data-stu-id="24132-168">description</span></span>|<span data-ttu-id="24132-169">Строка</span><span class="sxs-lookup"><span data-stu-id="24132-169">String</span></span>|<span data-ttu-id="24132-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="24132-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="24132-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24132-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24132-172">displayName</span><span class="sxs-lookup"><span data-stu-id="24132-172">displayName</span></span>|<span data-ttu-id="24132-173">Строка</span><span class="sxs-lookup"><span data-stu-id="24132-173">String</span></span>|<span data-ttu-id="24132-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="24132-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="24132-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24132-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24132-176">version</span><span class="sxs-lookup"><span data-stu-id="24132-176">version</span></span>|<span data-ttu-id="24132-177">Int32</span><span class="sxs-lookup"><span data-stu-id="24132-177">Int32</span></span>|<span data-ttu-id="24132-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="24132-178">Version of the device configuration.</span></span> <span data-ttu-id="24132-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24132-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24132-180">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="24132-180">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="24132-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-181">Boolean</span></span>|<span data-ttu-id="24132-182">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="24132-182">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="24132-183">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="24132-183">applyOnlyToWindows81</span></span>|<span data-ttu-id="24132-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-184">Boolean</span></span>|<span data-ttu-id="24132-185">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="24132-185">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="24132-186">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="24132-186">This property is read-only.</span></span>|
|<span data-ttu-id="24132-187">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="24132-187">browserBlockAutofill</span></span>|<span data-ttu-id="24132-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-188">Boolean</span></span>|<span data-ttu-id="24132-189">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="24132-189">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="24132-190">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="24132-190">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="24132-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-191">Boolean</span></span>|<span data-ttu-id="24132-192">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="24132-192">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="24132-193">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="24132-193">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="24132-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-194">Boolean</span></span>|<span data-ttu-id="24132-195">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="24132-195">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="24132-196">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="24132-196">browserBlockJavaScript</span></span>|<span data-ttu-id="24132-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-197">Boolean</span></span>|<span data-ttu-id="24132-198">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="24132-198">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="24132-199">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="24132-199">browserBlockPlugins</span></span>|<span data-ttu-id="24132-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-200">Boolean</span></span>|<span data-ttu-id="24132-201">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="24132-201">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="24132-202">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="24132-202">browserBlockPopups</span></span>|<span data-ttu-id="24132-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-203">Boolean</span></span>|<span data-ttu-id="24132-204">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="24132-204">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="24132-205">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="24132-205">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="24132-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-206">Boolean</span></span>|<span data-ttu-id="24132-207">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="24132-207">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="24132-208">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="24132-208">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="24132-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-209">Boolean</span></span>|<span data-ttu-id="24132-210">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="24132-210">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="24132-211">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="24132-211">browserRequireSmartScreen</span></span>|<span data-ttu-id="24132-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-212">Boolean</span></span>|<span data-ttu-id="24132-213">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="24132-213">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="24132-214">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="24132-214">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="24132-215">String</span><span class="sxs-lookup"><span data-stu-id="24132-215">String</span></span>|<span data-ttu-id="24132-216">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="24132-216">The enterprise mode site list location.</span></span> <span data-ttu-id="24132-217">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="24132-217">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="24132-218">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="24132-218">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="24132-219">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="24132-219">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="24132-220">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="24132-220">The internet security level.</span></span> <span data-ttu-id="24132-221">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="24132-221">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="24132-222">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="24132-222">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="24132-223">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="24132-223">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="24132-224">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="24132-224">The Intranet security level.</span></span> <span data-ttu-id="24132-225">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="24132-225">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="24132-226">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="24132-226">browserLoggingReportLocation</span></span>|<span data-ttu-id="24132-227">String</span><span class="sxs-lookup"><span data-stu-id="24132-227">String</span></span>|<span data-ttu-id="24132-228">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="24132-228">The logging report location.</span></span>|
|<span data-ttu-id="24132-229">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="24132-229">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="24132-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-230">Boolean</span></span>|<span data-ttu-id="24132-231">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="24132-231">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="24132-232">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="24132-232">browserRequireFirewall</span></span>|<span data-ttu-id="24132-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-233">Boolean</span></span>|<span data-ttu-id="24132-234">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="24132-234">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="24132-235">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="24132-235">browserRequireFraudWarning</span></span>|<span data-ttu-id="24132-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-236">Boolean</span></span>|<span data-ttu-id="24132-237">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="24132-237">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="24132-238">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="24132-238">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="24132-239">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="24132-239">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="24132-240">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="24132-240">The trusted sites security level.</span></span> <span data-ttu-id="24132-241">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="24132-241">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="24132-242">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="24132-242">cellularBlockDataRoaming</span></span>|<span data-ttu-id="24132-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-243">Boolean</span></span>|<span data-ttu-id="24132-244">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="24132-244">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="24132-245">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="24132-245">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="24132-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-246">Boolean</span></span>|<span data-ttu-id="24132-247">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="24132-247">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="24132-248">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="24132-248">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="24132-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-249">Boolean</span></span>|<span data-ttu-id="24132-250">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="24132-250">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="24132-251">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="24132-251">passwordExpirationDays</span></span>|<span data-ttu-id="24132-252">Int32</span><span class="sxs-lookup"><span data-stu-id="24132-252">Int32</span></span>|<span data-ttu-id="24132-253">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="24132-253">Password expiration in days.</span></span>|
|<span data-ttu-id="24132-254">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="24132-254">passwordMinimumLength</span></span>|<span data-ttu-id="24132-255">Int32</span><span class="sxs-lookup"><span data-stu-id="24132-255">Int32</span></span>|<span data-ttu-id="24132-256">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="24132-256">The minimum password length.</span></span>|
|<span data-ttu-id="24132-257">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="24132-257">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="24132-258">Int32</span><span class="sxs-lookup"><span data-stu-id="24132-258">Int32</span></span>|<span data-ttu-id="24132-259">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="24132-259">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="24132-260">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="24132-260">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="24132-261">Int32</span><span class="sxs-lookup"><span data-stu-id="24132-261">Int32</span></span>|<span data-ttu-id="24132-262">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="24132-262">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="24132-263">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="24132-263">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="24132-264">Int32</span><span class="sxs-lookup"><span data-stu-id="24132-264">Int32</span></span>|<span data-ttu-id="24132-265">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="24132-265">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="24132-266">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="24132-266">Valid values 0 to 24</span></span>|
|<span data-ttu-id="24132-267">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="24132-267">passwordRequiredType</span></span>|[<span data-ttu-id="24132-268">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="24132-268">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="24132-269">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="24132-269">The required password type.</span></span> <span data-ttu-id="24132-270">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="24132-270">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="24132-271">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="24132-271">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="24132-272">Int32</span><span class="sxs-lookup"><span data-stu-id="24132-272">Int32</span></span>|<span data-ttu-id="24132-273">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="24132-273">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="24132-274">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="24132-274">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="24132-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-275">Boolean</span></span>|<span data-ttu-id="24132-276">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="24132-276">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="24132-277">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="24132-277">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="24132-278">updateClassification</span><span class="sxs-lookup"><span data-stu-id="24132-278">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="24132-279">Минимальная классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="24132-279">The minimum update classification to install automatically.</span></span> <span data-ttu-id="24132-280">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="24132-280">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="24132-281">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="24132-281">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="24132-282">updateClassification</span><span class="sxs-lookup"><span data-stu-id="24132-282">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="24132-283">Минимальная классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="24132-283">The minimum update classification to install automatically.</span></span> <span data-ttu-id="24132-284">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="24132-284">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="24132-285">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="24132-285">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="24132-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="24132-286">Boolean</span></span>|<span data-ttu-id="24132-287">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="24132-287">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="24132-288">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="24132-288">userAccountControlSettings</span></span>|[<span data-ttu-id="24132-289">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="24132-289">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="24132-290">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="24132-290">The user account control settings.</span></span> <span data-ttu-id="24132-291">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="24132-291">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="24132-292">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="24132-292">workFoldersUrl</span></span>|<span data-ttu-id="24132-293">String</span><span class="sxs-lookup"><span data-stu-id="24132-293">String</span></span>|<span data-ttu-id="24132-294">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="24132-294">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="24132-295">Отклик</span><span class="sxs-lookup"><span data-stu-id="24132-295">Response</span></span>
<span data-ttu-id="24132-296">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="24132-296">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24132-297">Пример</span><span class="sxs-lookup"><span data-stu-id="24132-297">Example</span></span>

### <a name="request"></a><span data-ttu-id="24132-298">Запрос</span><span class="sxs-lookup"><span data-stu-id="24132-298">Request</span></span>
<span data-ttu-id="24132-299">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24132-299">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="24132-300">Отклик</span><span class="sxs-lookup"><span data-stu-id="24132-300">Response</span></span>
<span data-ttu-id="24132-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24132-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




