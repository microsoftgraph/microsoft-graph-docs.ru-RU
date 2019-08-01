---
title: Создание windows81GeneralConfiguration
description: Создание объекта windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbba1af44a624290615078b1fb7647b6a1b5f91b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018871"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="3bab5-103">Создание windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bab5-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="3bab5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3bab5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bab5-105">Создание объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bab5-105">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bab5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3bab5-106">Prerequisites</span></span>
<span data-ttu-id="3bab5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bab5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bab5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bab5-109">Permission type</span></span>|<span data-ttu-id="3bab5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bab5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bab5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bab5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3bab5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bab5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3bab5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bab5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bab5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bab5-114">Not supported.</span></span>|
|<span data-ttu-id="3bab5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bab5-115">Application</span></span>|<span data-ttu-id="3bab5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bab5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bab5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bab5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3bab5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bab5-118">Request headers</span></span>
|<span data-ttu-id="3bab5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3bab5-119">Header</span></span>|<span data-ttu-id="3bab5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3bab5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bab5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bab5-121">Authorization</span></span>|<span data-ttu-id="3bab5-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bab5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bab5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3bab5-123">Accept</span></span>|<span data-ttu-id="3bab5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3bab5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bab5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3bab5-125">Request body</span></span>
<span data-ttu-id="3bab5-126">В теле запроса добавьте представление объекта windows81GeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3bab5-126">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="3bab5-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3bab5-127">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="3bab5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3bab5-128">Property</span></span>|<span data-ttu-id="3bab5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3bab5-129">Type</span></span>|<span data-ttu-id="3bab5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3bab5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bab5-131">id</span><span class="sxs-lookup"><span data-stu-id="3bab5-131">id</span></span>|<span data-ttu-id="3bab5-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3bab5-132">String</span></span>|<span data-ttu-id="3bab5-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3bab5-133">Key of the entity.</span></span> <span data-ttu-id="3bab5-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bab5-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bab5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bab5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3bab5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bab5-136">DateTimeOffset</span></span>|<span data-ttu-id="3bab5-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3bab5-137">DateTime the object was last modified.</span></span> <span data-ttu-id="3bab5-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bab5-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bab5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bab5-139">createdDateTime</span></span>|<span data-ttu-id="3bab5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bab5-140">DateTimeOffset</span></span>|<span data-ttu-id="3bab5-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3bab5-141">DateTime the object was created.</span></span> <span data-ttu-id="3bab5-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bab5-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bab5-143">description</span><span class="sxs-lookup"><span data-stu-id="3bab5-143">description</span></span>|<span data-ttu-id="3bab5-144">String</span><span class="sxs-lookup"><span data-stu-id="3bab5-144">String</span></span>|<span data-ttu-id="3bab5-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3bab5-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3bab5-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bab5-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bab5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3bab5-147">displayName</span></span>|<span data-ttu-id="3bab5-148">Строка</span><span class="sxs-lookup"><span data-stu-id="3bab5-148">String</span></span>|<span data-ttu-id="3bab5-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3bab5-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3bab5-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bab5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bab5-151">version</span><span class="sxs-lookup"><span data-stu-id="3bab5-151">version</span></span>|<span data-ttu-id="3bab5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3bab5-152">Int32</span></span>|<span data-ttu-id="3bab5-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3bab5-153">Version of the device configuration.</span></span> <span data-ttu-id="3bab5-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bab5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bab5-155">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="3bab5-155">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="3bab5-156">Логический</span><span class="sxs-lookup"><span data-stu-id="3bab5-156">Boolean</span></span>|<span data-ttu-id="3bab5-157">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="3bab5-157">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="3bab5-158">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="3bab5-158">applyOnlyToWindows81</span></span>|<span data-ttu-id="3bab5-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-159">Boolean</span></span>|<span data-ttu-id="3bab5-160">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="3bab5-160">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="3bab5-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3bab5-161">This property is read-only.</span></span>|
|<span data-ttu-id="3bab5-162">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="3bab5-162">browserBlockAutofill</span></span>|<span data-ttu-id="3bab5-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-163">Boolean</span></span>|<span data-ttu-id="3bab5-164">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="3bab5-164">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="3bab5-165">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="3bab5-165">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="3bab5-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-166">Boolean</span></span>|<span data-ttu-id="3bab5-167">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="3bab5-167">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="3bab5-168">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="3bab5-168">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="3bab5-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-169">Boolean</span></span>|<span data-ttu-id="3bab5-170">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="3bab5-170">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="3bab5-171">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="3bab5-171">browserBlockJavaScript</span></span>|<span data-ttu-id="3bab5-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-172">Boolean</span></span>|<span data-ttu-id="3bab5-173">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="3bab5-173">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="3bab5-174">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="3bab5-174">browserBlockPlugins</span></span>|<span data-ttu-id="3bab5-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-175">Boolean</span></span>|<span data-ttu-id="3bab5-176">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="3bab5-176">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="3bab5-177">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="3bab5-177">browserBlockPopups</span></span>|<span data-ttu-id="3bab5-178">Логический</span><span class="sxs-lookup"><span data-stu-id="3bab5-178">Boolean</span></span>|<span data-ttu-id="3bab5-179">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="3bab5-179">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="3bab5-180">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="3bab5-180">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="3bab5-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-181">Boolean</span></span>|<span data-ttu-id="3bab5-182">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="3bab5-182">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="3bab5-183">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="3bab5-183">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="3bab5-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-184">Boolean</span></span>|<span data-ttu-id="3bab5-185">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="3bab5-185">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="3bab5-186">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="3bab5-186">browserRequireSmartScreen</span></span>|<span data-ttu-id="3bab5-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-187">Boolean</span></span>|<span data-ttu-id="3bab5-188">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="3bab5-188">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="3bab5-189">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="3bab5-189">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="3bab5-190">String</span><span class="sxs-lookup"><span data-stu-id="3bab5-190">String</span></span>|<span data-ttu-id="3bab5-191">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="3bab5-191">The enterprise mode site list location.</span></span> <span data-ttu-id="3bab5-192">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="3bab5-192">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="3bab5-193">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3bab5-193">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="3bab5-194">Интернетситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="3bab5-194">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="3bab5-195">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="3bab5-195">The internet security level.</span></span> <span data-ttu-id="3bab5-196">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="3bab5-196">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="3bab5-197">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3bab5-197">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="3bab5-198">Ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="3bab5-198">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="3bab5-199">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="3bab5-199">The Intranet security level.</span></span> <span data-ttu-id="3bab5-200">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="3bab5-200">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="3bab5-201">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="3bab5-201">browserLoggingReportLocation</span></span>|<span data-ttu-id="3bab5-202">String</span><span class="sxs-lookup"><span data-stu-id="3bab5-202">String</span></span>|<span data-ttu-id="3bab5-203">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="3bab5-203">The logging report location.</span></span>|
|<span data-ttu-id="3bab5-204">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="3bab5-204">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="3bab5-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-205">Boolean</span></span>|<span data-ttu-id="3bab5-206">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="3bab5-206">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="3bab5-207">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="3bab5-207">browserRequireFirewall</span></span>|<span data-ttu-id="3bab5-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-208">Boolean</span></span>|<span data-ttu-id="3bab5-209">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="3bab5-209">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="3bab5-210">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="3bab5-210">browserRequireFraudWarning</span></span>|<span data-ttu-id="3bab5-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-211">Boolean</span></span>|<span data-ttu-id="3bab5-212">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="3bab5-212">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="3bab5-213">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3bab5-213">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="3bab5-214">Ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="3bab5-214">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="3bab5-215">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="3bab5-215">The trusted sites security level.</span></span> <span data-ttu-id="3bab5-216">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="3bab5-216">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="3bab5-217">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="3bab5-217">cellularBlockDataRoaming</span></span>|<span data-ttu-id="3bab5-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-218">Boolean</span></span>|<span data-ttu-id="3bab5-219">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="3bab5-219">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="3bab5-220">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="3bab5-220">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="3bab5-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-221">Boolean</span></span>|<span data-ttu-id="3bab5-222">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="3bab5-222">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="3bab5-223">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="3bab5-223">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="3bab5-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-224">Boolean</span></span>|<span data-ttu-id="3bab5-225">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="3bab5-225">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="3bab5-226">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3bab5-226">passwordExpirationDays</span></span>|<span data-ttu-id="3bab5-227">Int32</span><span class="sxs-lookup"><span data-stu-id="3bab5-227">Int32</span></span>|<span data-ttu-id="3bab5-228">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="3bab5-228">Password expiration in days.</span></span>|
|<span data-ttu-id="3bab5-229">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3bab5-229">passwordMinimumLength</span></span>|<span data-ttu-id="3bab5-230">Int32</span><span class="sxs-lookup"><span data-stu-id="3bab5-230">Int32</span></span>|<span data-ttu-id="3bab5-231">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="3bab5-231">The minimum password length.</span></span>|
|<span data-ttu-id="3bab5-232">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="3bab5-232">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="3bab5-233">Int32</span><span class="sxs-lookup"><span data-stu-id="3bab5-233">Int32</span></span>|<span data-ttu-id="3bab5-234">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="3bab5-234">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="3bab5-235">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3bab5-235">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3bab5-236">Int32</span><span class="sxs-lookup"><span data-stu-id="3bab5-236">Int32</span></span>|<span data-ttu-id="3bab5-237">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="3bab5-237">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3bab5-238">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3bab5-238">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3bab5-239">Int32</span><span class="sxs-lookup"><span data-stu-id="3bab5-239">Int32</span></span>|<span data-ttu-id="3bab5-240">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="3bab5-240">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="3bab5-241">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="3bab5-241">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3bab5-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3bab5-242">passwordRequiredType</span></span>|[<span data-ttu-id="3bab5-243">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="3bab5-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3bab5-244">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="3bab5-244">The required password type.</span></span> <span data-ttu-id="3bab5-245">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3bab5-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3bab5-246">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3bab5-246">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3bab5-247">Int32</span><span class="sxs-lookup"><span data-stu-id="3bab5-247">Int32</span></span>|<span data-ttu-id="3bab5-248">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="3bab5-248">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="3bab5-249">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="3bab5-249">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="3bab5-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-250">Boolean</span></span>|<span data-ttu-id="3bab5-251">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="3bab5-251">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="3bab5-252">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="3bab5-252">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="3bab5-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bab5-253">Boolean</span></span>|<span data-ttu-id="3bab5-254">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="3bab5-254">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="3bab5-255">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="3bab5-255">userAccountControlSettings</span></span>|[<span data-ttu-id="3bab5-256">Виндовсусераккаунтконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="3bab5-256">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="3bab5-257">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="3bab5-257">The user account control settings.</span></span> <span data-ttu-id="3bab5-258">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="3bab5-258">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="3bab5-259">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="3bab5-259">workFoldersUrl</span></span>|<span data-ttu-id="3bab5-260">String</span><span class="sxs-lookup"><span data-stu-id="3bab5-260">String</span></span>|<span data-ttu-id="3bab5-261">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="3bab5-261">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="3bab5-262">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bab5-262">Response</span></span>
<span data-ttu-id="3bab5-263">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3bab5-263">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bab5-264">Пример</span><span class="sxs-lookup"><span data-stu-id="3bab5-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bab5-265">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bab5-265">Request</span></span>
<span data-ttu-id="3bab5-266">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bab5-266">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3bab5-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bab5-267">Response</span></span>
<span data-ttu-id="3bab5-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3bab5-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



