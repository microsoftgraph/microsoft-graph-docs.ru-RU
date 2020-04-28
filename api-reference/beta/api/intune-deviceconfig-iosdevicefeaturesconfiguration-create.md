---
title: Создание объекта iosDeviceFeaturesConfiguration
description: Создание объекта iosDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a14a2355044ecc59fa84bafb73ae126c58d8e0b3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432795"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="3de18-103">Создание объекта iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="3de18-103">Create iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="3de18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3de18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3de18-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3de18-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3de18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3de18-107">Создание объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-107">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3de18-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3de18-108">Prerequisites</span></span>
<span data-ttu-id="3de18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3de18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3de18-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3de18-111">Permission type</span></span>|<span data-ttu-id="3de18-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3de18-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3de18-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3de18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3de18-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3de18-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3de18-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3de18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3de18-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de18-116">Not supported.</span></span>|
|<span data-ttu-id="3de18-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3de18-117">Application</span></span>|<span data-ttu-id="3de18-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3de18-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3de18-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3de18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3de18-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3de18-120">Request headers</span></span>
|<span data-ttu-id="3de18-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3de18-121">Header</span></span>|<span data-ttu-id="3de18-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3de18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3de18-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3de18-123">Authorization</span></span>|<span data-ttu-id="3de18-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3de18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3de18-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3de18-125">Accept</span></span>|<span data-ttu-id="3de18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3de18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3de18-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3de18-127">Request body</span></span>
<span data-ttu-id="3de18-128">В теле запроса добавьте представление объекта iosDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3de18-128">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="3de18-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3de18-129">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="3de18-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3de18-130">Property</span></span>|<span data-ttu-id="3de18-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3de18-131">Type</span></span>|<span data-ttu-id="3de18-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3de18-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3de18-133">id</span><span class="sxs-lookup"><span data-stu-id="3de18-133">id</span></span>|<span data-ttu-id="3de18-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3de18-134">String</span></span>|<span data-ttu-id="3de18-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3de18-135">Key of the entity.</span></span> <span data-ttu-id="3de18-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de18-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3de18-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3de18-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de18-138">DateTimeOffset</span></span>|<span data-ttu-id="3de18-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3de18-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3de18-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de18-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3de18-141">roleScopeTagIds</span></span>|<span data-ttu-id="3de18-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="3de18-142">String collection</span></span>|<span data-ttu-id="3de18-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3de18-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3de18-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de18-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="3de18-145">supportsScopeTags</span></span>|<span data-ttu-id="3de18-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3de18-146">Boolean</span></span>|<span data-ttu-id="3de18-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3de18-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3de18-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="3de18-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3de18-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3de18-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3de18-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3de18-150">This property is read-only.</span></span> <span data-ttu-id="3de18-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de18-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3de18-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3de18-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3de18-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3de18-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3de18-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3de18-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de18-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3de18-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3de18-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3de18-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3de18-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3de18-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3de18-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de18-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3de18-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3de18-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3de18-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3de18-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3de18-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3de18-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de18-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3de18-164">createdDateTime</span></span>|<span data-ttu-id="3de18-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de18-165">DateTimeOffset</span></span>|<span data-ttu-id="3de18-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3de18-166">DateTime the object was created.</span></span> <span data-ttu-id="3de18-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de18-168">description</span><span class="sxs-lookup"><span data-stu-id="3de18-168">description</span></span>|<span data-ttu-id="3de18-169">String</span><span class="sxs-lookup"><span data-stu-id="3de18-169">String</span></span>|<span data-ttu-id="3de18-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3de18-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3de18-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de18-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3de18-172">displayName</span></span>|<span data-ttu-id="3de18-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3de18-173">String</span></span>|<span data-ttu-id="3de18-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3de18-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3de18-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de18-176">version</span><span class="sxs-lookup"><span data-stu-id="3de18-176">version</span></span>|<span data-ttu-id="3de18-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3de18-177">Int32</span></span>|<span data-ttu-id="3de18-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3de18-178">Version of the device configuration.</span></span> <span data-ttu-id="3de18-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de18-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de18-180">аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="3de18-180">airPrintDestinations</span></span>|<span data-ttu-id="3de18-181">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="3de18-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="3de18-182">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="3de18-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="3de18-183">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3de18-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3de18-184">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="3de18-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="3de18-185">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="3de18-185">assetTagTemplate</span></span>|<span data-ttu-id="3de18-186">String</span><span class="sxs-lookup"><span data-stu-id="3de18-186">String</span></span>|<span data-ttu-id="3de18-187">Сведения о теге ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="3de18-187">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="3de18-188">Contentfiltersettings к объекту</span><span class="sxs-lookup"><span data-stu-id="3de18-188">contentFilterSettings</span></span>|<span data-ttu-id="3de18-189">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md);</span><span class="sxs-lookup"><span data-stu-id="3de18-189">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>|<span data-ttu-id="3de18-190">Получает или задает параметры фильтра веб-содержимого iOS, режим с контролируемым режимом</span><span class="sxs-lookup"><span data-stu-id="3de18-190">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="3de18-191">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="3de18-191">lockScreenFootnote</span></span>|<span data-ttu-id="3de18-192">String</span><span class="sxs-lookup"><span data-stu-id="3de18-192">String</span></span>|<span data-ttu-id="3de18-193">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="3de18-193">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="3de18-194">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="3de18-194">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="3de18-195">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="3de18-195">homeScreenDockIcons</span></span>|<span data-ttu-id="3de18-196">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="3de18-196">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="3de18-197">Список приложений и папок, которые должны отображаться на панели Dock на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="3de18-197">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="3de18-198">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3de18-198">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3de18-199">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="3de18-199">homeScreenPages</span></span>|<span data-ttu-id="3de18-200">Коллекция [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="3de18-200">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="3de18-201">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="3de18-201">A list of pages on the Home Screen.</span></span> <span data-ttu-id="3de18-202">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3de18-202">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3de18-203">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="3de18-203">notificationSettings</span></span>|<span data-ttu-id="3de18-204">Коллекция [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="3de18-204">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="3de18-205">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="3de18-205">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="3de18-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3de18-206">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3de18-207">синглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="3de18-207">singleSignOnSettings</span></span>|[<span data-ttu-id="3de18-208">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="3de18-208">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="3de18-209">Параметры входа в систему Kerberos, позволяющие приложениям на принимающих устройствах беспрепятственно выполнять проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="3de18-209">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="3de18-210">валлпапердисплайлокатион</span><span class="sxs-lookup"><span data-stu-id="3de18-210">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="3de18-211">иосваллпапердисплайлокатион</span><span class="sxs-lookup"><span data-stu-id="3de18-211">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="3de18-212">Описатель расположения для отображения фонового рисунка.</span><span class="sxs-lookup"><span data-stu-id="3de18-212">A wallpaper display location specifier.</span></span> <span data-ttu-id="3de18-213">Возможные значения: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span><span class="sxs-lookup"><span data-stu-id="3de18-213">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="3de18-214">валлпаперимаже</span><span class="sxs-lookup"><span data-stu-id="3de18-214">wallpaperImage</span></span>|<span data-ttu-id="3de18-215">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="3de18-215">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="3de18-216">Изображение фонового рисунка должно иметь формат PNG или JPEG.</span><span class="sxs-lookup"><span data-stu-id="3de18-216">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="3de18-217">Для этого требуется контролируемое устройство с iOS 8 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="3de18-217">It requires a supervised device with iOS 8 or later version.</span></span>|
|<span data-ttu-id="3de18-218">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="3de18-218">singleSignOnExtension</span></span>|[<span data-ttu-id="3de18-219">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="3de18-219">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="3de18-220">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="3de18-220">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="3de18-221">Устарело: вместо этого используйте Иоссинглесигнонекстенсион.</span><span class="sxs-lookup"><span data-stu-id="3de18-221">Deprecated: use IOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="3de18-222">iosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="3de18-222">iosSingleSignOnExtension</span></span>|[<span data-ttu-id="3de18-223">iosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="3de18-223">iosSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-iossinglesignonextension.md)|<span data-ttu-id="3de18-224">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="3de18-224">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="3de18-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="3de18-225">Response</span></span>
<span data-ttu-id="3de18-226">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3de18-226">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3de18-227">Пример</span><span class="sxs-lookup"><span data-stu-id="3de18-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="3de18-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="3de18-228">Request</span></span>
<span data-ttu-id="3de18-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3de18-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3de18-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="3de18-230">Response</span></span>
<span data-ttu-id="3de18-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3de18-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



