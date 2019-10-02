---
title: Создание windows81GeneralConfiguration
description: Создание объекта windows81GeneralConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cdebf5c5b7beb04a05747b69a1b571534990d333
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365098"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="601f8-103">Создание windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="601f8-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="601f8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="601f8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="601f8-105">Создание объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="601f8-105">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="601f8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="601f8-106">Prerequisites</span></span>
<span data-ttu-id="601f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="601f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="601f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="601f8-109">Permission type</span></span>|<span data-ttu-id="601f8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="601f8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="601f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="601f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="601f8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="601f8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="601f8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="601f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="601f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="601f8-114">Not supported.</span></span>|
|<span data-ttu-id="601f8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="601f8-115">Application</span></span>|<span data-ttu-id="601f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="601f8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="601f8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="601f8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="601f8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="601f8-118">Request headers</span></span>
|<span data-ttu-id="601f8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="601f8-119">Header</span></span>|<span data-ttu-id="601f8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="601f8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="601f8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="601f8-121">Authorization</span></span>|<span data-ttu-id="601f8-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="601f8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="601f8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="601f8-123">Accept</span></span>|<span data-ttu-id="601f8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="601f8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="601f8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="601f8-125">Request body</span></span>
<span data-ttu-id="601f8-126">В теле запроса добавьте представление объекта windows81GeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="601f8-126">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="601f8-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="601f8-127">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="601f8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="601f8-128">Property</span></span>|<span data-ttu-id="601f8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="601f8-129">Type</span></span>|<span data-ttu-id="601f8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="601f8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="601f8-131">id</span><span class="sxs-lookup"><span data-stu-id="601f8-131">id</span></span>|<span data-ttu-id="601f8-132">Строка</span><span class="sxs-lookup"><span data-stu-id="601f8-132">String</span></span>|<span data-ttu-id="601f8-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="601f8-133">Key of the entity.</span></span> <span data-ttu-id="601f8-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="601f8-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="601f8-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="601f8-135">lastModifiedDateTime</span></span>|<span data-ttu-id="601f8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="601f8-136">DateTimeOffset</span></span>|<span data-ttu-id="601f8-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="601f8-137">DateTime the object was last modified.</span></span> <span data-ttu-id="601f8-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="601f8-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="601f8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="601f8-139">createdDateTime</span></span>|<span data-ttu-id="601f8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="601f8-140">DateTimeOffset</span></span>|<span data-ttu-id="601f8-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="601f8-141">DateTime the object was created.</span></span> <span data-ttu-id="601f8-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="601f8-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="601f8-143">description</span><span class="sxs-lookup"><span data-stu-id="601f8-143">description</span></span>|<span data-ttu-id="601f8-144">String</span><span class="sxs-lookup"><span data-stu-id="601f8-144">String</span></span>|<span data-ttu-id="601f8-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="601f8-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="601f8-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="601f8-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="601f8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="601f8-147">displayName</span></span>|<span data-ttu-id="601f8-148">Строка</span><span class="sxs-lookup"><span data-stu-id="601f8-148">String</span></span>|<span data-ttu-id="601f8-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="601f8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="601f8-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="601f8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="601f8-151">version</span><span class="sxs-lookup"><span data-stu-id="601f8-151">version</span></span>|<span data-ttu-id="601f8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="601f8-152">Int32</span></span>|<span data-ttu-id="601f8-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="601f8-153">Version of the device configuration.</span></span> <span data-ttu-id="601f8-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="601f8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="601f8-155">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="601f8-155">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="601f8-156">Логический</span><span class="sxs-lookup"><span data-stu-id="601f8-156">Boolean</span></span>|<span data-ttu-id="601f8-157">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="601f8-157">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="601f8-158">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="601f8-158">applyOnlyToWindows81</span></span>|<span data-ttu-id="601f8-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-159">Boolean</span></span>|<span data-ttu-id="601f8-160">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="601f8-160">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="601f8-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="601f8-161">This property is read-only.</span></span>|
|<span data-ttu-id="601f8-162">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="601f8-162">browserBlockAutofill</span></span>|<span data-ttu-id="601f8-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-163">Boolean</span></span>|<span data-ttu-id="601f8-164">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="601f8-164">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="601f8-165">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="601f8-165">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="601f8-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-166">Boolean</span></span>|<span data-ttu-id="601f8-167">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="601f8-167">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="601f8-168">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="601f8-168">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="601f8-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-169">Boolean</span></span>|<span data-ttu-id="601f8-170">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="601f8-170">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="601f8-171">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="601f8-171">browserBlockJavaScript</span></span>|<span data-ttu-id="601f8-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-172">Boolean</span></span>|<span data-ttu-id="601f8-173">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="601f8-173">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="601f8-174">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="601f8-174">browserBlockPlugins</span></span>|<span data-ttu-id="601f8-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-175">Boolean</span></span>|<span data-ttu-id="601f8-176">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="601f8-176">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="601f8-177">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="601f8-177">browserBlockPopups</span></span>|<span data-ttu-id="601f8-178">Логический</span><span class="sxs-lookup"><span data-stu-id="601f8-178">Boolean</span></span>|<span data-ttu-id="601f8-179">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="601f8-179">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="601f8-180">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="601f8-180">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="601f8-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-181">Boolean</span></span>|<span data-ttu-id="601f8-182">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="601f8-182">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="601f8-183">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="601f8-183">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="601f8-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-184">Boolean</span></span>|<span data-ttu-id="601f8-185">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="601f8-185">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="601f8-186">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="601f8-186">browserRequireSmartScreen</span></span>|<span data-ttu-id="601f8-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-187">Boolean</span></span>|<span data-ttu-id="601f8-188">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="601f8-188">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="601f8-189">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="601f8-189">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="601f8-190">String</span><span class="sxs-lookup"><span data-stu-id="601f8-190">String</span></span>|<span data-ttu-id="601f8-191">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="601f8-191">The enterprise mode site list location.</span></span> <span data-ttu-id="601f8-192">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="601f8-192">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="601f8-193">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="601f8-193">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="601f8-194">интернетситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="601f8-194">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="601f8-195">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="601f8-195">The internet security level.</span></span> <span data-ttu-id="601f8-196">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="601f8-196">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="601f8-197">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="601f8-197">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="601f8-198">ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="601f8-198">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="601f8-199">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="601f8-199">The Intranet security level.</span></span> <span data-ttu-id="601f8-200">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="601f8-200">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="601f8-201">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="601f8-201">browserLoggingReportLocation</span></span>|<span data-ttu-id="601f8-202">String</span><span class="sxs-lookup"><span data-stu-id="601f8-202">String</span></span>|<span data-ttu-id="601f8-203">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="601f8-203">The logging report location.</span></span>|
|<span data-ttu-id="601f8-204">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="601f8-204">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="601f8-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-205">Boolean</span></span>|<span data-ttu-id="601f8-206">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="601f8-206">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="601f8-207">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="601f8-207">browserRequireFirewall</span></span>|<span data-ttu-id="601f8-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-208">Boolean</span></span>|<span data-ttu-id="601f8-209">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="601f8-209">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="601f8-210">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="601f8-210">browserRequireFraudWarning</span></span>|<span data-ttu-id="601f8-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-211">Boolean</span></span>|<span data-ttu-id="601f8-212">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="601f8-212">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="601f8-213">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="601f8-213">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="601f8-214">ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="601f8-214">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="601f8-215">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="601f8-215">The trusted sites security level.</span></span> <span data-ttu-id="601f8-216">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="601f8-216">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="601f8-217">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="601f8-217">cellularBlockDataRoaming</span></span>|<span data-ttu-id="601f8-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-218">Boolean</span></span>|<span data-ttu-id="601f8-219">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="601f8-219">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="601f8-220">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="601f8-220">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="601f8-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-221">Boolean</span></span>|<span data-ttu-id="601f8-222">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="601f8-222">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="601f8-223">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="601f8-223">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="601f8-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-224">Boolean</span></span>|<span data-ttu-id="601f8-225">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="601f8-225">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="601f8-226">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="601f8-226">passwordExpirationDays</span></span>|<span data-ttu-id="601f8-227">Int32</span><span class="sxs-lookup"><span data-stu-id="601f8-227">Int32</span></span>|<span data-ttu-id="601f8-228">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="601f8-228">Password expiration in days.</span></span>|
|<span data-ttu-id="601f8-229">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="601f8-229">passwordMinimumLength</span></span>|<span data-ttu-id="601f8-230">Int32</span><span class="sxs-lookup"><span data-stu-id="601f8-230">Int32</span></span>|<span data-ttu-id="601f8-231">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="601f8-231">The minimum password length.</span></span>|
|<span data-ttu-id="601f8-232">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="601f8-232">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="601f8-233">Int32</span><span class="sxs-lookup"><span data-stu-id="601f8-233">Int32</span></span>|<span data-ttu-id="601f8-234">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="601f8-234">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="601f8-235">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="601f8-235">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="601f8-236">Int32</span><span class="sxs-lookup"><span data-stu-id="601f8-236">Int32</span></span>|<span data-ttu-id="601f8-237">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="601f8-237">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="601f8-238">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="601f8-238">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="601f8-239">Int32</span><span class="sxs-lookup"><span data-stu-id="601f8-239">Int32</span></span>|<span data-ttu-id="601f8-240">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="601f8-240">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="601f8-241">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="601f8-241">Valid values 0 to 24</span></span>|
|<span data-ttu-id="601f8-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="601f8-242">passwordRequiredType</span></span>|[<span data-ttu-id="601f8-243">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="601f8-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="601f8-244">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="601f8-244">The required password type.</span></span> <span data-ttu-id="601f8-245">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="601f8-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="601f8-246">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="601f8-246">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="601f8-247">Int32</span><span class="sxs-lookup"><span data-stu-id="601f8-247">Int32</span></span>|<span data-ttu-id="601f8-248">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="601f8-248">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="601f8-249">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="601f8-249">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="601f8-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-250">Boolean</span></span>|<span data-ttu-id="601f8-251">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="601f8-251">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="601f8-252">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="601f8-252">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="601f8-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="601f8-253">Boolean</span></span>|<span data-ttu-id="601f8-254">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="601f8-254">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="601f8-255">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="601f8-255">userAccountControlSettings</span></span>|[<span data-ttu-id="601f8-256">виндовсусераккаунтконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="601f8-256">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="601f8-257">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="601f8-257">The user account control settings.</span></span> <span data-ttu-id="601f8-258">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="601f8-258">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="601f8-259">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="601f8-259">workFoldersUrl</span></span>|<span data-ttu-id="601f8-260">String</span><span class="sxs-lookup"><span data-stu-id="601f8-260">String</span></span>|<span data-ttu-id="601f8-261">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="601f8-261">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="601f8-262">Отклик</span><span class="sxs-lookup"><span data-stu-id="601f8-262">Response</span></span>
<span data-ttu-id="601f8-263">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="601f8-263">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="601f8-264">Пример</span><span class="sxs-lookup"><span data-stu-id="601f8-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="601f8-265">Запрос</span><span class="sxs-lookup"><span data-stu-id="601f8-265">Request</span></span>
<span data-ttu-id="601f8-266">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="601f8-266">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1693

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
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
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="601f8-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="601f8-267">Response</span></span>
<span data-ttu-id="601f8-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="601f8-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```




