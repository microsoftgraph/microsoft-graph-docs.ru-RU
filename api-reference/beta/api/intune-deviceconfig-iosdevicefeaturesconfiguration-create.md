---
title: Создание объекта iosDeviceFeaturesConfiguration
description: Создание объекта iosDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e865d10a023be239dcbfdfc03302a5b0171ccec1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949070"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="4e9cb-103">Создание объекта iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="4e9cb-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="4e9cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e9cb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e9cb-106">Создание объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-106">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e9cb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e9cb-107">Prerequisites</span></span>
<span data-ttu-id="4e9cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e9cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e9cb-110">Permission type</span></span>|<span data-ttu-id="4e9cb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e9cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e9cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e9cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e9cb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e9cb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e9cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e9cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e9cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-115">Not supported.</span></span>|
|<span data-ttu-id="4e9cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e9cb-116">Application</span></span>|<span data-ttu-id="4e9cb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e9cb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e9cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e9cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4e9cb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e9cb-119">Request headers</span></span>
|<span data-ttu-id="4e9cb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e9cb-120">Header</span></span>|<span data-ttu-id="4e9cb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4e9cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e9cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e9cb-122">Authorization</span></span>|<span data-ttu-id="4e9cb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e9cb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4e9cb-124">Accept</span></span>|<span data-ttu-id="4e9cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e9cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e9cb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e9cb-126">Request body</span></span>
<span data-ttu-id="4e9cb-127">В теле запроса добавьте представление объекта iosDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-127">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="4e9cb-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-128">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="4e9cb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e9cb-129">Property</span></span>|<span data-ttu-id="4e9cb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4e9cb-130">Type</span></span>|<span data-ttu-id="4e9cb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4e9cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e9cb-132">id</span><span class="sxs-lookup"><span data-stu-id="4e9cb-132">id</span></span>|<span data-ttu-id="4e9cb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4e9cb-133">String</span></span>|<span data-ttu-id="4e9cb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-134">Key of the entity.</span></span> <span data-ttu-id="4e9cb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e9cb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e9cb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4e9cb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e9cb-137">DateTimeOffset</span></span>|<span data-ttu-id="4e9cb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4e9cb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e9cb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4e9cb-140">roleScopeTagIds</span></span>|<span data-ttu-id="4e9cb-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4e9cb-141">String collection</span></span>|<span data-ttu-id="4e9cb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4e9cb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e9cb-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4e9cb-144">supportsScopeTags</span></span>|<span data-ttu-id="4e9cb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e9cb-145">Boolean</span></span>|<span data-ttu-id="4e9cb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4e9cb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4e9cb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4e9cb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-149">This property is read-only.</span></span> <span data-ttu-id="4e9cb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e9cb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4e9cb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4e9cb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4e9cb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4e9cb-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4e9cb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e9cb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4e9cb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4e9cb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4e9cb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4e9cb-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4e9cb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e9cb-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4e9cb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4e9cb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4e9cb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4e9cb-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4e9cb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e9cb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e9cb-163">createdDateTime</span></span>|<span data-ttu-id="4e9cb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e9cb-164">DateTimeOffset</span></span>|<span data-ttu-id="4e9cb-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-165">DateTime the object was created.</span></span> <span data-ttu-id="4e9cb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e9cb-167">description</span><span class="sxs-lookup"><span data-stu-id="4e9cb-167">description</span></span>|<span data-ttu-id="4e9cb-168">String</span><span class="sxs-lookup"><span data-stu-id="4e9cb-168">String</span></span>|<span data-ttu-id="4e9cb-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4e9cb-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e9cb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4e9cb-171">displayName</span></span>|<span data-ttu-id="4e9cb-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4e9cb-172">String</span></span>|<span data-ttu-id="4e9cb-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4e9cb-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e9cb-175">version</span><span class="sxs-lookup"><span data-stu-id="4e9cb-175">version</span></span>|<span data-ttu-id="4e9cb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4e9cb-176">Int32</span></span>|<span data-ttu-id="4e9cb-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-177">Version of the device configuration.</span></span> <span data-ttu-id="4e9cb-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e9cb-179">аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="4e9cb-179">airPrintDestinations</span></span>|<span data-ttu-id="4e9cb-180">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="4e9cb-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="4e9cb-181">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="4e9cb-182">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="4e9cb-183">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="4e9cb-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="4e9cb-184">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="4e9cb-184">assetTagTemplate</span></span>|<span data-ttu-id="4e9cb-185">Строка</span><span class="sxs-lookup"><span data-stu-id="4e9cb-185">String</span></span>|<span data-ttu-id="4e9cb-186">Сведения о теге ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-186">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="4e9cb-187">Contentfiltersettings к объекту</span><span class="sxs-lookup"><span data-stu-id="4e9cb-187">contentFilterSettings</span></span>|<span data-ttu-id="4e9cb-188">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md);</span><span class="sxs-lookup"><span data-stu-id="4e9cb-188">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>|<span data-ttu-id="4e9cb-189">Получает или задает параметры фильтра веб-содержимого iOS, режим с контролируемым режимом</span><span class="sxs-lookup"><span data-stu-id="4e9cb-189">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="4e9cb-190">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="4e9cb-190">lockScreenFootnote</span></span>|<span data-ttu-id="4e9cb-191">String</span><span class="sxs-lookup"><span data-stu-id="4e9cb-191">String</span></span>|<span data-ttu-id="4e9cb-192">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-192">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="4e9cb-193">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-193">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="4e9cb-194">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="4e9cb-194">homeScreenDockIcons</span></span>|<span data-ttu-id="4e9cb-195">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="4e9cb-195">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="4e9cb-196">Список приложений и папок, которые должны отображаться на панели Dock на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-196">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="4e9cb-197">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4e9cb-198">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="4e9cb-198">homeScreenPages</span></span>|<span data-ttu-id="4e9cb-199">Коллекция [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="4e9cb-199">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="4e9cb-200">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-200">A list of pages on the Home Screen.</span></span> <span data-ttu-id="4e9cb-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-201">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4e9cb-202">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="4e9cb-202">notificationSettings</span></span>|<span data-ttu-id="4e9cb-203">Коллекция [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="4e9cb-203">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="4e9cb-204">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="4e9cb-204">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="4e9cb-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-205">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4e9cb-206">синглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="4e9cb-206">singleSignOnSettings</span></span>|[<span data-ttu-id="4e9cb-207">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="4e9cb-207">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="4e9cb-208">Параметры входа в систему Kerberos, позволяющие приложениям на принимающих устройствах беспрепятственно выполнять проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-208">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="4e9cb-209">валлпапердисплайлокатион</span><span class="sxs-lookup"><span data-stu-id="4e9cb-209">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="4e9cb-210">иосваллпапердисплайлокатион</span><span class="sxs-lookup"><span data-stu-id="4e9cb-210">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="4e9cb-211">Описатель расположения для отображения фонового рисунка.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-211">A wallpaper display location specifier.</span></span> <span data-ttu-id="4e9cb-212">Возможные значения: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-212">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="4e9cb-213">валлпаперимаже</span><span class="sxs-lookup"><span data-stu-id="4e9cb-213">wallpaperImage</span></span>|<span data-ttu-id="4e9cb-214">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="4e9cb-214">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="4e9cb-215">Изображение фонового рисунка должно иметь формат PNG или JPEG.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-215">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="4e9cb-216">Для этого требуется контролируемое устройство с iOS 8 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-216">It requires a supervised device with iOS 8 or later version.</span></span>|
|<span data-ttu-id="4e9cb-217">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="4e9cb-217">singleSignOnExtension</span></span>|[<span data-ttu-id="4e9cb-218">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="4e9cb-218">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="4e9cb-219">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-219">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="4e9cb-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e9cb-220">Response</span></span>
<span data-ttu-id="4e9cb-221">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-221">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e9cb-222">Пример</span><span class="sxs-lookup"><span data-stu-id="4e9cb-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e9cb-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e9cb-223">Request</span></span>
<span data-ttu-id="4e9cb-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5571

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
  }
}
```

### <a name="response"></a><span data-ttu-id="4e9cb-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e9cb-225">Response</span></span>
<span data-ttu-id="4e9cb-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e9cb-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5743

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
  }
}
```





