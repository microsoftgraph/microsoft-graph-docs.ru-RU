---
title: Update iosDeviceFeaturesConfiguration
description: Обновление свойств объекта iosDeviceFeaturesConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d7f8fe33f495bfe7dd01987d4c2db3ad8765f437
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424947"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="6d02d-103">Update iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d02d-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="6d02d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6d02d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6d02d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d02d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d02d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d02d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d02d-107">Обновление свойств объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d02d-107">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d02d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6d02d-108">Prerequisites</span></span>
<span data-ttu-id="6d02d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6d02d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6d02d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d02d-111">Permission type</span></span>|<span data-ttu-id="6d02d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d02d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d02d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d02d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d02d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d02d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d02d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d02d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d02d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d02d-116">Not supported.</span></span>|
|<span data-ttu-id="6d02d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d02d-117">Application</span></span>|<span data-ttu-id="6d02d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d02d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d02d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d02d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6d02d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d02d-120">Request headers</span></span>
|<span data-ttu-id="6d02d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d02d-121">Header</span></span>|<span data-ttu-id="6d02d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6d02d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d02d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d02d-123">Authorization</span></span>|<span data-ttu-id="6d02d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6d02d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d02d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6d02d-125">Accept</span></span>|<span data-ttu-id="6d02d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d02d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d02d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d02d-127">Request body</span></span>
<span data-ttu-id="6d02d-128">В тексте запроса добавьте представление объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d02d-128">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="6d02d-129">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d02d-129">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="6d02d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d02d-130">Property</span></span>|<span data-ttu-id="6d02d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6d02d-131">Type</span></span>|<span data-ttu-id="6d02d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6d02d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d02d-133">id</span><span class="sxs-lookup"><span data-stu-id="6d02d-133">id</span></span>|<span data-ttu-id="6d02d-134">String</span><span class="sxs-lookup"><span data-stu-id="6d02d-134">String</span></span>|<span data-ttu-id="6d02d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6d02d-135">Key of the entity.</span></span> <span data-ttu-id="6d02d-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d02d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d02d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d02d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6d02d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d02d-138">DateTimeOffset</span></span>|<span data-ttu-id="6d02d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6d02d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6d02d-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d02d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d02d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6d02d-141">roleScopeTagIds</span></span>|<span data-ttu-id="6d02d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6d02d-142">String collection</span></span>|<span data-ttu-id="6d02d-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6d02d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6d02d-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d02d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d02d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6d02d-145">supportsScopeTags</span></span>|<span data-ttu-id="6d02d-146">Логический</span><span class="sxs-lookup"><span data-stu-id="6d02d-146">Boolean</span></span>|<span data-ttu-id="6d02d-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="6d02d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6d02d-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="6d02d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6d02d-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6d02d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6d02d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6d02d-150">This property is read-only.</span></span> <span data-ttu-id="6d02d-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d02d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d02d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d02d-152">createdDateTime</span></span>|<span data-ttu-id="6d02d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d02d-153">DateTimeOffset</span></span>|<span data-ttu-id="6d02d-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6d02d-154">DateTime the object was created.</span></span> <span data-ttu-id="6d02d-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d02d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d02d-156">description</span><span class="sxs-lookup"><span data-stu-id="6d02d-156">description</span></span>|<span data-ttu-id="6d02d-157">String</span><span class="sxs-lookup"><span data-stu-id="6d02d-157">String</span></span>|<span data-ttu-id="6d02d-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d02d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6d02d-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d02d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d02d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6d02d-160">displayName</span></span>|<span data-ttu-id="6d02d-161">String</span><span class="sxs-lookup"><span data-stu-id="6d02d-161">String</span></span>|<span data-ttu-id="6d02d-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d02d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6d02d-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d02d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d02d-164">version</span><span class="sxs-lookup"><span data-stu-id="6d02d-164">version</span></span>|<span data-ttu-id="6d02d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6d02d-165">Int32</span></span>|<span data-ttu-id="6d02d-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d02d-166">Version of the device configuration.</span></span> <span data-ttu-id="6d02d-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d02d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d02d-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="6d02d-168">airPrintDestinations</span></span>|<span data-ttu-id="6d02d-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6d02d-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="6d02d-170">Массив AirPrint принтеров, которые всегда должны быть отображены.</span><span class="sxs-lookup"><span data-stu-id="6d02d-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="6d02d-171">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6d02d-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6d02d-172">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="6d02d-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="6d02d-173">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="6d02d-173">assetTagTemplate</span></span>|<span data-ttu-id="6d02d-174">String</span><span class="sxs-lookup"><span data-stu-id="6d02d-174">String</span></span>|<span data-ttu-id="6d02d-175">Сведения о теге ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="6d02d-175">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="6d02d-176">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="6d02d-176">contentFilterSettings</span></span>|<span data-ttu-id="6d02d-177">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md);</span><span class="sxs-lookup"><span data-stu-id="6d02d-177">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>|<span data-ttu-id="6d02d-178">Получает или задает параметры фильтра веб-содержимого, контролируемом режим только операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="6d02d-178">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="6d02d-179">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="6d02d-179">lockScreenFootnote</span></span>|<span data-ttu-id="6d02d-180">String</span><span class="sxs-lookup"><span data-stu-id="6d02d-180">String</span></span>|<span data-ttu-id="6d02d-181">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="6d02d-181">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="6d02d-182">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="6d02d-182">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="6d02d-183">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="6d02d-183">homeScreenDockIcons</span></span>|<span data-ttu-id="6d02d-184">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="6d02d-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="6d02d-185">Список приложений и папок, которые должны отображаться на панели Dock на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="6d02d-185">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="6d02d-186">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6d02d-186">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6d02d-187">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="6d02d-187">homeScreenPages</span></span>|<span data-ttu-id="6d02d-188">Коллекция [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="6d02d-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="6d02d-189">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="6d02d-189">A list of pages on the Home Screen.</span></span> <span data-ttu-id="6d02d-190">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6d02d-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6d02d-191">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="6d02d-191">notificationSettings</span></span>|<span data-ttu-id="6d02d-192">Коллекция [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6d02d-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="6d02d-193">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d02d-193">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="6d02d-194">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6d02d-194">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6d02d-195">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="6d02d-195">singleSignOnSettings</span></span>|[<span data-ttu-id="6d02d-196">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="6d02d-196">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="6d02d-197">Параметры входа в систему Kerberos, которые позволяют приложения на получение устройства для проверки подлинности беспрепятственно.</span><span class="sxs-lookup"><span data-stu-id="6d02d-197">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="6d02d-198">wallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="6d02d-198">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="6d02d-199">iosWallpaperDisplayLocation</span><span class="sxs-lookup"><span data-stu-id="6d02d-199">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="6d02d-200">Расположение описателя отображения фонового рисунка.</span><span class="sxs-lookup"><span data-stu-id="6d02d-200">A wallpaper display location specifier.</span></span> <span data-ttu-id="6d02d-201">Возможные значения: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span><span class="sxs-lookup"><span data-stu-id="6d02d-201">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="6d02d-202">wallpaperImage</span><span class="sxs-lookup"><span data-stu-id="6d02d-202">wallpaperImage</span></span>|<span data-ttu-id="6d02d-203">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="6d02d-203">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="6d02d-204">Рисунок должен быть в формате PNG или JPEG.</span><span class="sxs-lookup"><span data-stu-id="6d02d-204">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="6d02d-205">Требуется контролируемом устройство с iOS 8 или более поздняя версия.</span><span class="sxs-lookup"><span data-stu-id="6d02d-205">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="6d02d-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d02d-206">Response</span></span>
<span data-ttu-id="6d02d-207">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6d02d-207">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d02d-208">Пример</span><span class="sxs-lookup"><span data-stu-id="6d02d-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d02d-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d02d-209">Request</span></span>
<span data-ttu-id="6d02d-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d02d-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3656

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  }
}
```

### <a name="response"></a><span data-ttu-id="6d02d-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d02d-211">Response</span></span>
<span data-ttu-id="6d02d-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6d02d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3828

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  }
}
```




