---
title: Создание windows81GeneralConfiguration
description: Создание объекта windows81GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a205fce73ab918107a4aa4582e08f92b2e1fdc2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918278"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="c50a2-103">Создание windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="c50a2-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="c50a2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c50a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c50a2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c50a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c50a2-106">Создание объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c50a2-106">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c50a2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c50a2-107">Prerequisites</span></span>
<span data-ttu-id="c50a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c50a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c50a2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c50a2-110">Permission type</span></span>|<span data-ttu-id="c50a2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c50a2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c50a2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c50a2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c50a2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c50a2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c50a2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c50a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c50a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c50a2-115">Not supported.</span></span>|
|<span data-ttu-id="c50a2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c50a2-116">Application</span></span>|<span data-ttu-id="c50a2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c50a2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c50a2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c50a2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c50a2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c50a2-119">Request headers</span></span>
|<span data-ttu-id="c50a2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c50a2-120">Header</span></span>|<span data-ttu-id="c50a2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c50a2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c50a2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c50a2-122">Authorization</span></span>|<span data-ttu-id="c50a2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c50a2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c50a2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c50a2-124">Accept</span></span>|<span data-ttu-id="c50a2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c50a2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c50a2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c50a2-126">Request body</span></span>
<span data-ttu-id="c50a2-127">В теле запроса добавьте представление объекта windows81GeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c50a2-127">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="c50a2-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c50a2-128">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="c50a2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c50a2-129">Property</span></span>|<span data-ttu-id="c50a2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c50a2-130">Type</span></span>|<span data-ttu-id="c50a2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c50a2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c50a2-132">id</span><span class="sxs-lookup"><span data-stu-id="c50a2-132">id</span></span>|<span data-ttu-id="c50a2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c50a2-133">String</span></span>|<span data-ttu-id="c50a2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c50a2-134">Key of the entity.</span></span> <span data-ttu-id="c50a2-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c50a2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c50a2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c50a2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c50a2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c50a2-137">DateTimeOffset</span></span>|<span data-ttu-id="c50a2-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c50a2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c50a2-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c50a2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c50a2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c50a2-140">roleScopeTagIds</span></span>|<span data-ttu-id="c50a2-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c50a2-141">String collection</span></span>|<span data-ttu-id="c50a2-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c50a2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c50a2-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c50a2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c50a2-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c50a2-144">supportsScopeTags</span></span>|<span data-ttu-id="c50a2-145">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-145">Boolean</span></span>|<span data-ttu-id="c50a2-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c50a2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c50a2-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c50a2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c50a2-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c50a2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c50a2-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c50a2-149">This property is read-only.</span></span> <span data-ttu-id="c50a2-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c50a2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c50a2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c50a2-151">createdDateTime</span></span>|<span data-ttu-id="c50a2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c50a2-152">DateTimeOffset</span></span>|<span data-ttu-id="c50a2-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c50a2-153">DateTime the object was created.</span></span> <span data-ttu-id="c50a2-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c50a2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c50a2-155">description</span><span class="sxs-lookup"><span data-stu-id="c50a2-155">description</span></span>|<span data-ttu-id="c50a2-156">String</span><span class="sxs-lookup"><span data-stu-id="c50a2-156">String</span></span>|<span data-ttu-id="c50a2-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c50a2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c50a2-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c50a2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c50a2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c50a2-159">displayName</span></span>|<span data-ttu-id="c50a2-160">Строка</span><span class="sxs-lookup"><span data-stu-id="c50a2-160">String</span></span>|<span data-ttu-id="c50a2-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c50a2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c50a2-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c50a2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c50a2-163">version</span><span class="sxs-lookup"><span data-stu-id="c50a2-163">version</span></span>|<span data-ttu-id="c50a2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c50a2-164">Int32</span></span>|<span data-ttu-id="c50a2-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c50a2-165">Version of the device configuration.</span></span> <span data-ttu-id="c50a2-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c50a2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c50a2-167">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="c50a2-167">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="c50a2-168">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-168">Boolean</span></span>|<span data-ttu-id="c50a2-169">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c50a2-169">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="c50a2-170">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="c50a2-170">applyOnlyToWindows81</span></span>|<span data-ttu-id="c50a2-171">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-171">Boolean</span></span>|<span data-ttu-id="c50a2-172">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="c50a2-172">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="c50a2-173">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c50a2-173">This property is read-only.</span></span>|
|<span data-ttu-id="c50a2-174">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="c50a2-174">browserBlockAutofill</span></span>|<span data-ttu-id="c50a2-175">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-175">Boolean</span></span>|<span data-ttu-id="c50a2-176">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="c50a2-176">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="c50a2-177">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="c50a2-177">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="c50a2-178">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-178">Boolean</span></span>|<span data-ttu-id="c50a2-179">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="c50a2-179">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="c50a2-180">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="c50a2-180">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="c50a2-181">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-181">Boolean</span></span>|<span data-ttu-id="c50a2-182">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="c50a2-182">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="c50a2-183">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="c50a2-183">browserBlockJavaScript</span></span>|<span data-ttu-id="c50a2-184">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-184">Boolean</span></span>|<span data-ttu-id="c50a2-185">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="c50a2-185">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="c50a2-186">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="c50a2-186">browserBlockPlugins</span></span>|<span data-ttu-id="c50a2-187">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-187">Boolean</span></span>|<span data-ttu-id="c50a2-188">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="c50a2-188">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="c50a2-189">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="c50a2-189">browserBlockPopups</span></span>|<span data-ttu-id="c50a2-190">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-190">Boolean</span></span>|<span data-ttu-id="c50a2-191">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="c50a2-191">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="c50a2-192">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="c50a2-192">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="c50a2-193">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-193">Boolean</span></span>|<span data-ttu-id="c50a2-194">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="c50a2-194">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="c50a2-195">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="c50a2-195">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="c50a2-196">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-196">Boolean</span></span>|<span data-ttu-id="c50a2-197">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="c50a2-197">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="c50a2-198">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="c50a2-198">browserRequireSmartScreen</span></span>|<span data-ttu-id="c50a2-199">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-199">Boolean</span></span>|<span data-ttu-id="c50a2-200">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="c50a2-200">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="c50a2-201">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="c50a2-201">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="c50a2-202">Строка</span><span class="sxs-lookup"><span data-stu-id="c50a2-202">String</span></span>|<span data-ttu-id="c50a2-203">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="c50a2-203">The enterprise mode site list location.</span></span> <span data-ttu-id="c50a2-204">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="c50a2-204">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="c50a2-205">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c50a2-205">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="c50a2-206">Интернетситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="c50a2-206">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="c50a2-207">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="c50a2-207">The internet security level.</span></span> <span data-ttu-id="c50a2-208">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="c50a2-208">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="c50a2-209">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c50a2-209">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="c50a2-210">Ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="c50a2-210">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="c50a2-211">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="c50a2-211">The Intranet security level.</span></span> <span data-ttu-id="c50a2-212">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="c50a2-212">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="c50a2-213">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="c50a2-213">browserLoggingReportLocation</span></span>|<span data-ttu-id="c50a2-214">String</span><span class="sxs-lookup"><span data-stu-id="c50a2-214">String</span></span>|<span data-ttu-id="c50a2-215">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="c50a2-215">The logging report location.</span></span>|
|<span data-ttu-id="c50a2-216">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="c50a2-216">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="c50a2-217">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-217">Boolean</span></span>|<span data-ttu-id="c50a2-218">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="c50a2-218">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="c50a2-219">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="c50a2-219">browserRequireFirewall</span></span>|<span data-ttu-id="c50a2-220">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-220">Boolean</span></span>|<span data-ttu-id="c50a2-221">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="c50a2-221">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="c50a2-222">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="c50a2-222">browserRequireFraudWarning</span></span>|<span data-ttu-id="c50a2-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="c50a2-223">Boolean</span></span>|<span data-ttu-id="c50a2-224">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="c50a2-224">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="c50a2-225">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c50a2-225">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="c50a2-226">Ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="c50a2-226">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="c50a2-227">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="c50a2-227">The trusted sites security level.</span></span> <span data-ttu-id="c50a2-228">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="c50a2-228">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="c50a2-229">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="c50a2-229">cellularBlockDataRoaming</span></span>|<span data-ttu-id="c50a2-230">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-230">Boolean</span></span>|<span data-ttu-id="c50a2-231">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="c50a2-231">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="c50a2-232">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="c50a2-232">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="c50a2-233">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-233">Boolean</span></span>|<span data-ttu-id="c50a2-234">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="c50a2-234">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="c50a2-235">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="c50a2-235">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="c50a2-236">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-236">Boolean</span></span>|<span data-ttu-id="c50a2-237">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="c50a2-237">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="c50a2-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c50a2-238">passwordExpirationDays</span></span>|<span data-ttu-id="c50a2-239">Int32</span><span class="sxs-lookup"><span data-stu-id="c50a2-239">Int32</span></span>|<span data-ttu-id="c50a2-240">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="c50a2-240">Password expiration in days.</span></span>|
|<span data-ttu-id="c50a2-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c50a2-241">passwordMinimumLength</span></span>|<span data-ttu-id="c50a2-242">Int32</span><span class="sxs-lookup"><span data-stu-id="c50a2-242">Int32</span></span>|<span data-ttu-id="c50a2-243">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="c50a2-243">The minimum password length.</span></span>|
|<span data-ttu-id="c50a2-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c50a2-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c50a2-245">Int32</span><span class="sxs-lookup"><span data-stu-id="c50a2-245">Int32</span></span>|<span data-ttu-id="c50a2-246">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="c50a2-246">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c50a2-247">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c50a2-247">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c50a2-248">Int32</span><span class="sxs-lookup"><span data-stu-id="c50a2-248">Int32</span></span>|<span data-ttu-id="c50a2-249">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="c50a2-249">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c50a2-250">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c50a2-250">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c50a2-251">Int32</span><span class="sxs-lookup"><span data-stu-id="c50a2-251">Int32</span></span>|<span data-ttu-id="c50a2-252">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="c50a2-252">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="c50a2-253">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="c50a2-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c50a2-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c50a2-254">passwordRequiredType</span></span>|[<span data-ttu-id="c50a2-255">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c50a2-255">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c50a2-256">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c50a2-256">The required password type.</span></span> <span data-ttu-id="c50a2-257">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="c50a2-257">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c50a2-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c50a2-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c50a2-259">Int32</span><span class="sxs-lookup"><span data-stu-id="c50a2-259">Int32</span></span>|<span data-ttu-id="c50a2-260">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="c50a2-260">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="c50a2-261">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="c50a2-261">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="c50a2-262">Логический</span><span class="sxs-lookup"><span data-stu-id="c50a2-262">Boolean</span></span>|<span data-ttu-id="c50a2-263">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="c50a2-263">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="c50a2-264">Минимумаутоинсталлклассификатион</span><span class="sxs-lookup"><span data-stu-id="c50a2-264">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="c50a2-265">Упдатеклассификатион</span><span class="sxs-lookup"><span data-stu-id="c50a2-265">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="c50a2-266">Минимальная Классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="c50a2-266">The minimum update classification to install automatically.</span></span> <span data-ttu-id="c50a2-267">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="c50a2-267">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="c50a2-268">Упдатесминимумаутоинсталлклассификатион</span><span class="sxs-lookup"><span data-stu-id="c50a2-268">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="c50a2-269">Упдатеклассификатион</span><span class="sxs-lookup"><span data-stu-id="c50a2-269">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="c50a2-270">Минимальная Классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="c50a2-270">The minimum update classification to install automatically.</span></span> <span data-ttu-id="c50a2-271">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="c50a2-271">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="c50a2-272">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="c50a2-272">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="c50a2-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="c50a2-273">Boolean</span></span>|<span data-ttu-id="c50a2-274">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="c50a2-274">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="c50a2-275">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="c50a2-275">userAccountControlSettings</span></span>|[<span data-ttu-id="c50a2-276">Виндовсусераккаунтконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="c50a2-276">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="c50a2-277">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="c50a2-277">The user account control settings.</span></span> <span data-ttu-id="c50a2-278">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="c50a2-278">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="c50a2-279">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="c50a2-279">workFoldersUrl</span></span>|<span data-ttu-id="c50a2-280">String</span><span class="sxs-lookup"><span data-stu-id="c50a2-280">String</span></span>|<span data-ttu-id="c50a2-281">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="c50a2-281">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="c50a2-282">Отклик</span><span class="sxs-lookup"><span data-stu-id="c50a2-282">Response</span></span>
<span data-ttu-id="c50a2-283">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c50a2-283">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c50a2-284">Пример</span><span class="sxs-lookup"><span data-stu-id="c50a2-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="c50a2-285">Запрос</span><span class="sxs-lookup"><span data-stu-id="c50a2-285">Request</span></span>
<span data-ttu-id="c50a2-286">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c50a2-286">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1924

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="c50a2-287">Отклик</span><span class="sxs-lookup"><span data-stu-id="c50a2-287">Response</span></span>
<span data-ttu-id="c50a2-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c50a2-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2096

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




