---
title: Update iosDeviceFeaturesConfiguration
description: Обновление свойств объекта iosDeviceFeaturesConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ae849321f90509132425cdb01c9a00a74232aff
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42751771"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="421ba-103">Update iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="421ba-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="421ba-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="421ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="421ba-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="421ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="421ba-106">Обновление свойств объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-106">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="421ba-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="421ba-107">Prerequisites</span></span>
<span data-ttu-id="421ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="421ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="421ba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="421ba-110">Permission type</span></span>|<span data-ttu-id="421ba-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="421ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="421ba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="421ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="421ba-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="421ba-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="421ba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="421ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="421ba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="421ba-115">Not supported.</span></span>|
|<span data-ttu-id="421ba-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="421ba-116">Application</span></span>|<span data-ttu-id="421ba-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="421ba-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="421ba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="421ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="421ba-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="421ba-119">Request headers</span></span>
|<span data-ttu-id="421ba-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="421ba-120">Header</span></span>|<span data-ttu-id="421ba-121">Значение</span><span class="sxs-lookup"><span data-stu-id="421ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="421ba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="421ba-122">Authorization</span></span>|<span data-ttu-id="421ba-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="421ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="421ba-124">Accept</span><span class="sxs-lookup"><span data-stu-id="421ba-124">Accept</span></span>|<span data-ttu-id="421ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="421ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="421ba-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="421ba-126">Request body</span></span>
<span data-ttu-id="421ba-127">В тексте запроса добавьте представление объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="421ba-127">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="421ba-128">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-128">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="421ba-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="421ba-129">Property</span></span>|<span data-ttu-id="421ba-130">Тип</span><span class="sxs-lookup"><span data-stu-id="421ba-130">Type</span></span>|<span data-ttu-id="421ba-131">Описание</span><span class="sxs-lookup"><span data-stu-id="421ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="421ba-132">id</span><span class="sxs-lookup"><span data-stu-id="421ba-132">id</span></span>|<span data-ttu-id="421ba-133">Строка</span><span class="sxs-lookup"><span data-stu-id="421ba-133">String</span></span>|<span data-ttu-id="421ba-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="421ba-134">Key of the entity.</span></span> <span data-ttu-id="421ba-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="421ba-136">lastModifiedDateTime</span></span>|<span data-ttu-id="421ba-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="421ba-137">DateTimeOffset</span></span>|<span data-ttu-id="421ba-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="421ba-138">DateTime the object was last modified.</span></span> <span data-ttu-id="421ba-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="421ba-140">roleScopeTagIds</span></span>|<span data-ttu-id="421ba-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="421ba-141">String collection</span></span>|<span data-ttu-id="421ba-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="421ba-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="421ba-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="421ba-144">supportsScopeTags</span></span>|<span data-ttu-id="421ba-145">Логический</span><span class="sxs-lookup"><span data-stu-id="421ba-145">Boolean</span></span>|<span data-ttu-id="421ba-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="421ba-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="421ba-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="421ba-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="421ba-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="421ba-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="421ba-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="421ba-149">This property is read-only.</span></span> <span data-ttu-id="421ba-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="421ba-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="421ba-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="421ba-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="421ba-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="421ba-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="421ba-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="421ba-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="421ba-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="421ba-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="421ba-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="421ba-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="421ba-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="421ba-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="421ba-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="421ba-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="421ba-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="421ba-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="421ba-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="421ba-163">createdDateTime</span></span>|<span data-ttu-id="421ba-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="421ba-164">DateTimeOffset</span></span>|<span data-ttu-id="421ba-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="421ba-165">DateTime the object was created.</span></span> <span data-ttu-id="421ba-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-167">description</span><span class="sxs-lookup"><span data-stu-id="421ba-167">description</span></span>|<span data-ttu-id="421ba-168">String</span><span class="sxs-lookup"><span data-stu-id="421ba-168">String</span></span>|<span data-ttu-id="421ba-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="421ba-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="421ba-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-171">displayName</span><span class="sxs-lookup"><span data-stu-id="421ba-171">displayName</span></span>|<span data-ttu-id="421ba-172">Строка</span><span class="sxs-lookup"><span data-stu-id="421ba-172">String</span></span>|<span data-ttu-id="421ba-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="421ba-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="421ba-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-175">version</span><span class="sxs-lookup"><span data-stu-id="421ba-175">version</span></span>|<span data-ttu-id="421ba-176">Int32</span><span class="sxs-lookup"><span data-stu-id="421ba-176">Int32</span></span>|<span data-ttu-id="421ba-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="421ba-177">Version of the device configuration.</span></span> <span data-ttu-id="421ba-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="421ba-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="421ba-179">аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="421ba-179">airPrintDestinations</span></span>|<span data-ttu-id="421ba-180">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="421ba-181">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="421ba-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="421ba-182">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="421ba-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="421ba-183">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="421ba-184">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="421ba-184">assetTagTemplate</span></span>|<span data-ttu-id="421ba-185">String</span><span class="sxs-lookup"><span data-stu-id="421ba-185">String</span></span>|<span data-ttu-id="421ba-186">Сведения о теге ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="421ba-186">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="421ba-187">Contentfiltersettings к объекту</span><span class="sxs-lookup"><span data-stu-id="421ba-187">contentFilterSettings</span></span>|<span data-ttu-id="421ba-188">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md);</span><span class="sxs-lookup"><span data-stu-id="421ba-188">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>|<span data-ttu-id="421ba-189">Получает или задает параметры фильтра веб-содержимого iOS, режим с контролируемым режимом</span><span class="sxs-lookup"><span data-stu-id="421ba-189">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="421ba-190">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="421ba-190">lockScreenFootnote</span></span>|<span data-ttu-id="421ba-191">String</span><span class="sxs-lookup"><span data-stu-id="421ba-191">String</span></span>|<span data-ttu-id="421ba-192">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="421ba-192">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="421ba-193">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="421ba-193">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="421ba-194">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="421ba-194">homeScreenDockIcons</span></span>|<span data-ttu-id="421ba-195">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-195">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="421ba-196">Список приложений и папок, которые должны отображаться на панели Dock на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="421ba-196">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="421ba-197">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="421ba-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="421ba-198">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="421ba-198">homeScreenPages</span></span>|<span data-ttu-id="421ba-199">Коллекция [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-199">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="421ba-200">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="421ba-200">A list of pages on the Home Screen.</span></span> <span data-ttu-id="421ba-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="421ba-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="421ba-202">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="421ba-202">notificationSettings</span></span>|<span data-ttu-id="421ba-203">Коллекция [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="421ba-203">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="421ba-204">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="421ba-204">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="421ba-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="421ba-205">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="421ba-206">синглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="421ba-206">singleSignOnSettings</span></span>|[<span data-ttu-id="421ba-207">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="421ba-207">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="421ba-208">Параметры входа в систему Kerberos, позволяющие приложениям на принимающих устройствах беспрепятственно выполнять проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="421ba-208">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="421ba-209">валлпапердисплайлокатион</span><span class="sxs-lookup"><span data-stu-id="421ba-209">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="421ba-210">иосваллпапердисплайлокатион</span><span class="sxs-lookup"><span data-stu-id="421ba-210">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="421ba-211">Описатель расположения для отображения фонового рисунка.</span><span class="sxs-lookup"><span data-stu-id="421ba-211">A wallpaper display location specifier.</span></span> <span data-ttu-id="421ba-212">Возможные значения: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span><span class="sxs-lookup"><span data-stu-id="421ba-212">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="421ba-213">валлпаперимаже</span><span class="sxs-lookup"><span data-stu-id="421ba-213">wallpaperImage</span></span>|<span data-ttu-id="421ba-214">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="421ba-214">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="421ba-215">Изображение фонового рисунка должно иметь формат PNG или JPEG.</span><span class="sxs-lookup"><span data-stu-id="421ba-215">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="421ba-216">Для этого требуется контролируемое устройство с iOS 8 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="421ba-216">It requires a supervised device with iOS 8 or later version.</span></span>|
|<span data-ttu-id="421ba-217">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="421ba-217">singleSignOnExtension</span></span>|[<span data-ttu-id="421ba-218">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="421ba-218">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="421ba-219">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="421ba-219">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="421ba-220">Устарело: вместо этого используйте Иоссинглесигнонекстенсион.</span><span class="sxs-lookup"><span data-stu-id="421ba-220">Deprecated: use IOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="421ba-221">iosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="421ba-221">iosSingleSignOnExtension</span></span>|[<span data-ttu-id="421ba-222">iosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="421ba-222">iosSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-iossinglesignonextension.md)|<span data-ttu-id="421ba-223">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="421ba-223">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="421ba-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="421ba-224">Response</span></span>
<span data-ttu-id="421ba-225">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="421ba-225">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="421ba-226">Пример</span><span class="sxs-lookup"><span data-stu-id="421ba-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="421ba-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="421ba-227">Request</span></span>
<span data-ttu-id="421ba-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="421ba-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 6716

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  },
  "wallpaperDisplayLocation": "lockScreen",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "iosSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  }
}
```

### <a name="response"></a><span data-ttu-id="421ba-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="421ba-229">Response</span></span>
<span data-ttu-id="421ba-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="421ba-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6888

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "Asset Tag Template value",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "Url value",
        "bookmarkFolder": "Bookmark Folder value",
        "displayName": "Display Name value"
      }
    ]
  },
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "allowedUrls": [
      "Allowed Urls value"
    ],
    "displayName": "Display Name value",
    "kerberosPrincipalName": "Kerberos Principal Name value",
    "kerberosRealm": "Kerberos Realm value"
  },
  "wallpaperDisplayLocation": "lockScreen",
  "wallpaperImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "iosSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  }
}
```




