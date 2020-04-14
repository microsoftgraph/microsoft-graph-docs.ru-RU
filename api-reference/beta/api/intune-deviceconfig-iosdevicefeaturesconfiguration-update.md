---
title: Update iosDeviceFeaturesConfiguration
description: Обновление свойств объекта iosDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d5d1ec3d55ce23e2783b828188a8a4f1fe577e3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432751"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="cdcef-103">Update iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="cdcef-103">Update iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="cdcef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdcef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdcef-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdcef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdcef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdcef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdcef-107">Обновление свойств объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-107">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdcef-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cdcef-108">Prerequisites</span></span>
<span data-ttu-id="cdcef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdcef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdcef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdcef-111">Permission type</span></span>|<span data-ttu-id="cdcef-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdcef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdcef-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdcef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdcef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdcef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cdcef-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdcef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdcef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdcef-116">Not supported.</span></span>|
|<span data-ttu-id="cdcef-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cdcef-117">Application</span></span>|<span data-ttu-id="cdcef-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdcef-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdcef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdcef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cdcef-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cdcef-120">Request headers</span></span>
|<span data-ttu-id="cdcef-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdcef-121">Header</span></span>|<span data-ttu-id="cdcef-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cdcef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdcef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdcef-123">Authorization</span></span>|<span data-ttu-id="cdcef-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdcef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdcef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cdcef-125">Accept</span></span>|<span data-ttu-id="cdcef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdcef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdcef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdcef-127">Request body</span></span>
<span data-ttu-id="cdcef-128">В тексте запроса добавьте представление объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdcef-128">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="cdcef-129">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-129">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="cdcef-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdcef-130">Property</span></span>|<span data-ttu-id="cdcef-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cdcef-131">Type</span></span>|<span data-ttu-id="cdcef-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cdcef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdcef-133">id</span><span class="sxs-lookup"><span data-stu-id="cdcef-133">id</span></span>|<span data-ttu-id="cdcef-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cdcef-134">String</span></span>|<span data-ttu-id="cdcef-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cdcef-135">Key of the entity.</span></span> <span data-ttu-id="cdcef-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdcef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cdcef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cdcef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdcef-138">DateTimeOffset</span></span>|<span data-ttu-id="cdcef-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cdcef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="cdcef-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdcef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cdcef-141">roleScopeTagIds</span></span>|<span data-ttu-id="cdcef-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cdcef-142">String collection</span></span>|<span data-ttu-id="cdcef-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cdcef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cdcef-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdcef-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="cdcef-145">supportsScopeTags</span></span>|<span data-ttu-id="cdcef-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="cdcef-146">Boolean</span></span>|<span data-ttu-id="cdcef-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="cdcef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cdcef-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="cdcef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cdcef-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="cdcef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cdcef-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdcef-150">This property is read-only.</span></span> <span data-ttu-id="cdcef-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdcef-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cdcef-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="cdcef-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cdcef-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="cdcef-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cdcef-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="cdcef-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdcef-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cdcef-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="cdcef-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cdcef-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="cdcef-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cdcef-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="cdcef-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdcef-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cdcef-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="cdcef-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cdcef-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="cdcef-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cdcef-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="cdcef-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdcef-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cdcef-164">createdDateTime</span></span>|<span data-ttu-id="cdcef-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdcef-165">DateTimeOffset</span></span>|<span data-ttu-id="cdcef-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cdcef-166">DateTime the object was created.</span></span> <span data-ttu-id="cdcef-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdcef-168">description</span><span class="sxs-lookup"><span data-stu-id="cdcef-168">description</span></span>|<span data-ttu-id="cdcef-169">String</span><span class="sxs-lookup"><span data-stu-id="cdcef-169">String</span></span>|<span data-ttu-id="cdcef-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cdcef-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cdcef-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdcef-172">displayName</span><span class="sxs-lookup"><span data-stu-id="cdcef-172">displayName</span></span>|<span data-ttu-id="cdcef-173">Строка</span><span class="sxs-lookup"><span data-stu-id="cdcef-173">String</span></span>|<span data-ttu-id="cdcef-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cdcef-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cdcef-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdcef-176">version</span><span class="sxs-lookup"><span data-stu-id="cdcef-176">version</span></span>|<span data-ttu-id="cdcef-177">Int32</span><span class="sxs-lookup"><span data-stu-id="cdcef-177">Int32</span></span>|<span data-ttu-id="cdcef-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cdcef-178">Version of the device configuration.</span></span> <span data-ttu-id="cdcef-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cdcef-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdcef-180">аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="cdcef-180">airPrintDestinations</span></span>|<span data-ttu-id="cdcef-181">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="cdcef-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="cdcef-182">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="cdcef-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="cdcef-183">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="cdcef-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="cdcef-184">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="cdcef-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="cdcef-185">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="cdcef-185">assetTagTemplate</span></span>|<span data-ttu-id="cdcef-186">String</span><span class="sxs-lookup"><span data-stu-id="cdcef-186">String</span></span>|<span data-ttu-id="cdcef-187">Сведения о теге ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="cdcef-187">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="cdcef-188">Contentfiltersettings к объекту</span><span class="sxs-lookup"><span data-stu-id="cdcef-188">contentFilterSettings</span></span>|<span data-ttu-id="cdcef-189">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md);</span><span class="sxs-lookup"><span data-stu-id="cdcef-189">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>|<span data-ttu-id="cdcef-190">Получает или задает параметры фильтра веб-содержимого iOS, режим с контролируемым режимом</span><span class="sxs-lookup"><span data-stu-id="cdcef-190">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="cdcef-191">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="cdcef-191">lockScreenFootnote</span></span>|<span data-ttu-id="cdcef-192">String</span><span class="sxs-lookup"><span data-stu-id="cdcef-192">String</span></span>|<span data-ttu-id="cdcef-193">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="cdcef-193">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="cdcef-194">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="cdcef-194">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="cdcef-195">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="cdcef-195">homeScreenDockIcons</span></span>|<span data-ttu-id="cdcef-196">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="cdcef-196">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="cdcef-197">Список приложений и папок, которые должны отображаться на панели Dock на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="cdcef-197">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="cdcef-198">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="cdcef-198">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cdcef-199">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="cdcef-199">homeScreenPages</span></span>|<span data-ttu-id="cdcef-200">Коллекция [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="cdcef-200">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="cdcef-201">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="cdcef-201">A list of pages on the Home Screen.</span></span> <span data-ttu-id="cdcef-202">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="cdcef-202">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cdcef-203">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="cdcef-203">notificationSettings</span></span>|<span data-ttu-id="cdcef-204">Коллекция [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="cdcef-204">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="cdcef-205">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="cdcef-205">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="cdcef-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="cdcef-206">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cdcef-207">синглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="cdcef-207">singleSignOnSettings</span></span>|[<span data-ttu-id="cdcef-208">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="cdcef-208">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="cdcef-209">Параметры входа в систему Kerberos, позволяющие приложениям на принимающих устройствах беспрепятственно выполнять проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="cdcef-209">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="cdcef-210">валлпапердисплайлокатион</span><span class="sxs-lookup"><span data-stu-id="cdcef-210">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="cdcef-211">иосваллпапердисплайлокатион</span><span class="sxs-lookup"><span data-stu-id="cdcef-211">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="cdcef-212">Описатель расположения для отображения фонового рисунка.</span><span class="sxs-lookup"><span data-stu-id="cdcef-212">A wallpaper display location specifier.</span></span> <span data-ttu-id="cdcef-213">Возможные значения: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span><span class="sxs-lookup"><span data-stu-id="cdcef-213">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="cdcef-214">валлпаперимаже</span><span class="sxs-lookup"><span data-stu-id="cdcef-214">wallpaperImage</span></span>|<span data-ttu-id="cdcef-215">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="cdcef-215">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="cdcef-216">Изображение фонового рисунка должно иметь формат PNG или JPEG.</span><span class="sxs-lookup"><span data-stu-id="cdcef-216">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="cdcef-217">Для этого требуется контролируемое устройство с iOS 8 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="cdcef-217">It requires a supervised device with iOS 8 or later version.</span></span>|
|<span data-ttu-id="cdcef-218">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="cdcef-218">singleSignOnExtension</span></span>|[<span data-ttu-id="cdcef-219">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="cdcef-219">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="cdcef-220">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="cdcef-220">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="cdcef-221">Устарело: вместо этого используйте Иоссинглесигнонекстенсион.</span><span class="sxs-lookup"><span data-stu-id="cdcef-221">Deprecated: use IOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="cdcef-222">iosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="cdcef-222">iosSingleSignOnExtension</span></span>|[<span data-ttu-id="cdcef-223">iosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="cdcef-223">iosSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-iossinglesignonextension.md)|<span data-ttu-id="cdcef-224">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="cdcef-224">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="cdcef-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdcef-225">Response</span></span>
<span data-ttu-id="cdcef-226">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cdcef-226">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdcef-227">Пример</span><span class="sxs-lookup"><span data-stu-id="cdcef-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdcef-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdcef-228">Request</span></span>
<span data-ttu-id="cdcef-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdcef-229">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cdcef-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdcef-230">Response</span></span>
<span data-ttu-id="cdcef-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdcef-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



