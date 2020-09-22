---
title: Update windows81GeneralConfiguration
description: Обновление свойств объекта windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f7069acaf08e574ee79bf35bcd5a9b1a09dd9be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069955"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="b0a80-103">Update windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0a80-103">Update windows81GeneralConfiguration</span></span>

<span data-ttu-id="b0a80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0a80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0a80-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0a80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0a80-106">Обновление свойств объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0a80-106">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0a80-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b0a80-107">Prerequisites</span></span>
<span data-ttu-id="b0a80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0a80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0a80-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0a80-110">Permission type</span></span>|<span data-ttu-id="b0a80-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0a80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0a80-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0a80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0a80-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a80-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0a80-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0a80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0a80-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0a80-115">Not supported.</span></span>|
|<span data-ttu-id="b0a80-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0a80-116">Application</span></span>|<span data-ttu-id="b0a80-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0a80-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0a80-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0a80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b0a80-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b0a80-119">Request headers</span></span>
|<span data-ttu-id="b0a80-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0a80-120">Header</span></span>|<span data-ttu-id="b0a80-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b0a80-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0a80-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0a80-122">Authorization</span></span>|<span data-ttu-id="b0a80-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0a80-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0a80-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b0a80-124">Accept</span></span>|<span data-ttu-id="b0a80-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0a80-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0a80-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0a80-126">Request body</span></span>
<span data-ttu-id="b0a80-127">В тексте запроса добавьте представление объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0a80-127">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="b0a80-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0a80-128">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="b0a80-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0a80-129">Property</span></span>|<span data-ttu-id="b0a80-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b0a80-130">Type</span></span>|<span data-ttu-id="b0a80-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b0a80-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0a80-132">id</span><span class="sxs-lookup"><span data-stu-id="b0a80-132">id</span></span>|<span data-ttu-id="b0a80-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b0a80-133">String</span></span>|<span data-ttu-id="b0a80-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b0a80-134">Key of the entity.</span></span> <span data-ttu-id="b0a80-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0a80-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a80-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0a80-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b0a80-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a80-137">DateTimeOffset</span></span>|<span data-ttu-id="b0a80-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b0a80-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b0a80-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0a80-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a80-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0a80-140">createdDateTime</span></span>|<span data-ttu-id="b0a80-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a80-141">DateTimeOffset</span></span>|<span data-ttu-id="b0a80-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b0a80-142">DateTime the object was created.</span></span> <span data-ttu-id="b0a80-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0a80-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a80-144">description</span><span class="sxs-lookup"><span data-stu-id="b0a80-144">description</span></span>|<span data-ttu-id="b0a80-145">Строка</span><span class="sxs-lookup"><span data-stu-id="b0a80-145">String</span></span>|<span data-ttu-id="b0a80-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b0a80-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b0a80-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0a80-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a80-148">displayName</span><span class="sxs-lookup"><span data-stu-id="b0a80-148">displayName</span></span>|<span data-ttu-id="b0a80-149">Строка</span><span class="sxs-lookup"><span data-stu-id="b0a80-149">String</span></span>|<span data-ttu-id="b0a80-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b0a80-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b0a80-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0a80-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a80-152">version</span><span class="sxs-lookup"><span data-stu-id="b0a80-152">version</span></span>|<span data-ttu-id="b0a80-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a80-153">Int32</span></span>|<span data-ttu-id="b0a80-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b0a80-154">Version of the device configuration.</span></span> <span data-ttu-id="b0a80-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0a80-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0a80-156">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="b0a80-156">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="b0a80-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-157">Boolean</span></span>|<span data-ttu-id="b0a80-158">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b0a80-158">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="b0a80-159">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="b0a80-159">applyOnlyToWindows81</span></span>|<span data-ttu-id="b0a80-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-160">Boolean</span></span>|<span data-ttu-id="b0a80-161">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="b0a80-161">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="b0a80-162">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0a80-162">This property is read-only.</span></span>|
|<span data-ttu-id="b0a80-163">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b0a80-163">browserBlockAutofill</span></span>|<span data-ttu-id="b0a80-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-164">Boolean</span></span>|<span data-ttu-id="b0a80-165">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="b0a80-165">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="b0a80-166">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="b0a80-166">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="b0a80-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-167">Boolean</span></span>|<span data-ttu-id="b0a80-168">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="b0a80-168">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="b0a80-169">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="b0a80-169">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="b0a80-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-170">Boolean</span></span>|<span data-ttu-id="b0a80-171">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="b0a80-171">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="b0a80-172">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b0a80-172">browserBlockJavaScript</span></span>|<span data-ttu-id="b0a80-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-173">Boolean</span></span>|<span data-ttu-id="b0a80-174">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="b0a80-174">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="b0a80-175">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="b0a80-175">browserBlockPlugins</span></span>|<span data-ttu-id="b0a80-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-176">Boolean</span></span>|<span data-ttu-id="b0a80-177">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="b0a80-177">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="b0a80-178">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b0a80-178">browserBlockPopups</span></span>|<span data-ttu-id="b0a80-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-179">Boolean</span></span>|<span data-ttu-id="b0a80-180">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="b0a80-180">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="b0a80-181">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="b0a80-181">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="b0a80-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-182">Boolean</span></span>|<span data-ttu-id="b0a80-183">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="b0a80-183">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="b0a80-184">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="b0a80-184">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="b0a80-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-185">Boolean</span></span>|<span data-ttu-id="b0a80-186">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="b0a80-186">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="b0a80-187">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="b0a80-187">browserRequireSmartScreen</span></span>|<span data-ttu-id="b0a80-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-188">Boolean</span></span>|<span data-ttu-id="b0a80-189">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="b0a80-189">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="b0a80-190">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="b0a80-190">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="b0a80-191">String</span><span class="sxs-lookup"><span data-stu-id="b0a80-191">String</span></span>|<span data-ttu-id="b0a80-192">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="b0a80-192">The enterprise mode site list location.</span></span> <span data-ttu-id="b0a80-193">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="b0a80-193">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="b0a80-194">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b0a80-194">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="b0a80-195">интернетситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="b0a80-195">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="b0a80-196">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="b0a80-196">The internet security level.</span></span> <span data-ttu-id="b0a80-197">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b0a80-197">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b0a80-198">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b0a80-198">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="b0a80-199">ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="b0a80-199">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="b0a80-200">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="b0a80-200">The Intranet security level.</span></span> <span data-ttu-id="b0a80-201">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b0a80-201">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b0a80-202">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="b0a80-202">browserLoggingReportLocation</span></span>|<span data-ttu-id="b0a80-203">String</span><span class="sxs-lookup"><span data-stu-id="b0a80-203">String</span></span>|<span data-ttu-id="b0a80-204">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="b0a80-204">The logging report location.</span></span>|
|<span data-ttu-id="b0a80-205">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="b0a80-205">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="b0a80-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-206">Boolean</span></span>|<span data-ttu-id="b0a80-207">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="b0a80-207">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="b0a80-208">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="b0a80-208">browserRequireFirewall</span></span>|<span data-ttu-id="b0a80-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-209">Boolean</span></span>|<span data-ttu-id="b0a80-210">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="b0a80-210">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="b0a80-211">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="b0a80-211">browserRequireFraudWarning</span></span>|<span data-ttu-id="b0a80-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-212">Boolean</span></span>|<span data-ttu-id="b0a80-213">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="b0a80-213">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="b0a80-214">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b0a80-214">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="b0a80-215">ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="b0a80-215">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="b0a80-216">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="b0a80-216">The trusted sites security level.</span></span> <span data-ttu-id="b0a80-217">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b0a80-217">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b0a80-218">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="b0a80-218">cellularBlockDataRoaming</span></span>|<span data-ttu-id="b0a80-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-219">Boolean</span></span>|<span data-ttu-id="b0a80-220">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="b0a80-220">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="b0a80-221">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="b0a80-221">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="b0a80-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-222">Boolean</span></span>|<span data-ttu-id="b0a80-223">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="b0a80-223">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b0a80-224">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="b0a80-224">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="b0a80-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-225">Boolean</span></span>|<span data-ttu-id="b0a80-226">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="b0a80-226">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="b0a80-227">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b0a80-227">passwordExpirationDays</span></span>|<span data-ttu-id="b0a80-228">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a80-228">Int32</span></span>|<span data-ttu-id="b0a80-229">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="b0a80-229">Password expiration in days.</span></span>|
|<span data-ttu-id="b0a80-230">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b0a80-230">passwordMinimumLength</span></span>|<span data-ttu-id="b0a80-231">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a80-231">Int32</span></span>|<span data-ttu-id="b0a80-232">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="b0a80-232">The minimum password length.</span></span>|
|<span data-ttu-id="b0a80-233">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b0a80-233">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b0a80-234">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a80-234">Int32</span></span>|<span data-ttu-id="b0a80-235">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="b0a80-235">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b0a80-236">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b0a80-236">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b0a80-237">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a80-237">Int32</span></span>|<span data-ttu-id="b0a80-238">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="b0a80-238">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b0a80-239">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b0a80-239">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b0a80-240">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a80-240">Int32</span></span>|<span data-ttu-id="b0a80-241">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="b0a80-241">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="b0a80-242">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="b0a80-242">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b0a80-243">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b0a80-243">passwordRequiredType</span></span>|[<span data-ttu-id="b0a80-244">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="b0a80-244">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b0a80-245">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="b0a80-245">The required password type.</span></span> <span data-ttu-id="b0a80-246">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b0a80-246">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b0a80-247">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b0a80-247">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b0a80-248">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a80-248">Int32</span></span>|<span data-ttu-id="b0a80-249">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="b0a80-249">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="b0a80-250">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="b0a80-250">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="b0a80-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-251">Boolean</span></span>|<span data-ttu-id="b0a80-252">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="b0a80-252">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="b0a80-253">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="b0a80-253">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="b0a80-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a80-254">Boolean</span></span>|<span data-ttu-id="b0a80-255">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="b0a80-255">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="b0a80-256">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="b0a80-256">userAccountControlSettings</span></span>|[<span data-ttu-id="b0a80-257">виндовсусераккаунтконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="b0a80-257">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="b0a80-258">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="b0a80-258">The user account control settings.</span></span> <span data-ttu-id="b0a80-259">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="b0a80-259">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="b0a80-260">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="b0a80-260">workFoldersUrl</span></span>|<span data-ttu-id="b0a80-261">String</span><span class="sxs-lookup"><span data-stu-id="b0a80-261">String</span></span>|<span data-ttu-id="b0a80-262">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="b0a80-262">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="b0a80-263">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0a80-263">Response</span></span>
<span data-ttu-id="b0a80-264">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b0a80-264">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0a80-265">Пример</span><span class="sxs-lookup"><span data-stu-id="b0a80-265">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0a80-266">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0a80-266">Request</span></span>
<span data-ttu-id="b0a80-267">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0a80-267">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="b0a80-268">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0a80-268">Response</span></span>
<span data-ttu-id="b0a80-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0a80-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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









