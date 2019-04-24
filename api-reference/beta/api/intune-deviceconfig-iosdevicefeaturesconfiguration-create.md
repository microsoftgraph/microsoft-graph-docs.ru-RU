---
title: Создание объекта iosDeviceFeaturesConfiguration
description: Создание объекта iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f10bc7b7027b534a24f4a8f52ddbdd0499579f28
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467570"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="04649-103">Создание объекта iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="04649-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="04649-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04649-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04649-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04649-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04649-106">Создание объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04649-106">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04649-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="04649-107">Prerequisites</span></span>
<span data-ttu-id="04649-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04649-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04649-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04649-110">Permission type</span></span>|<span data-ttu-id="04649-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04649-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04649-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04649-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04649-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04649-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04649-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04649-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04649-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04649-115">Not supported.</span></span>|
|<span data-ttu-id="04649-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04649-116">Application</span></span>|<span data-ttu-id="04649-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04649-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04649-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04649-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="04649-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04649-119">Request headers</span></span>
|<span data-ttu-id="04649-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04649-120">Header</span></span>|<span data-ttu-id="04649-121">Значение</span><span class="sxs-lookup"><span data-stu-id="04649-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04649-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04649-122">Authorization</span></span>|<span data-ttu-id="04649-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04649-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04649-124">Accept</span><span class="sxs-lookup"><span data-stu-id="04649-124">Accept</span></span>|<span data-ttu-id="04649-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04649-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04649-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04649-126">Request body</span></span>
<span data-ttu-id="04649-127">В теле запроса добавьте представление объекта iosDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04649-127">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="04649-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="04649-128">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="04649-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="04649-129">Property</span></span>|<span data-ttu-id="04649-130">Тип</span><span class="sxs-lookup"><span data-stu-id="04649-130">Type</span></span>|<span data-ttu-id="04649-131">Описание</span><span class="sxs-lookup"><span data-stu-id="04649-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04649-132">id</span><span class="sxs-lookup"><span data-stu-id="04649-132">id</span></span>|<span data-ttu-id="04649-133">Строка</span><span class="sxs-lookup"><span data-stu-id="04649-133">String</span></span>|<span data-ttu-id="04649-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="04649-134">Key of the entity.</span></span> <span data-ttu-id="04649-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04649-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04649-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04649-136">lastModifiedDateTime</span></span>|<span data-ttu-id="04649-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04649-137">DateTimeOffset</span></span>|<span data-ttu-id="04649-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="04649-138">DateTime the object was last modified.</span></span> <span data-ttu-id="04649-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04649-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04649-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="04649-140">roleScopeTagIds</span></span>|<span data-ttu-id="04649-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="04649-141">String collection</span></span>|<span data-ttu-id="04649-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="04649-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="04649-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04649-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04649-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="04649-144">supportsScopeTags</span></span>|<span data-ttu-id="04649-145">Логический</span><span class="sxs-lookup"><span data-stu-id="04649-145">Boolean</span></span>|<span data-ttu-id="04649-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="04649-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="04649-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="04649-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="04649-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="04649-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="04649-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04649-149">This property is read-only.</span></span> <span data-ttu-id="04649-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04649-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04649-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04649-151">createdDateTime</span></span>|<span data-ttu-id="04649-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04649-152">DateTimeOffset</span></span>|<span data-ttu-id="04649-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="04649-153">DateTime the object was created.</span></span> <span data-ttu-id="04649-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04649-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04649-155">description</span><span class="sxs-lookup"><span data-stu-id="04649-155">description</span></span>|<span data-ttu-id="04649-156">String</span><span class="sxs-lookup"><span data-stu-id="04649-156">String</span></span>|<span data-ttu-id="04649-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="04649-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="04649-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04649-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04649-159">displayName</span><span class="sxs-lookup"><span data-stu-id="04649-159">displayName</span></span>|<span data-ttu-id="04649-160">Строка</span><span class="sxs-lookup"><span data-stu-id="04649-160">String</span></span>|<span data-ttu-id="04649-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="04649-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="04649-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04649-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04649-163">version</span><span class="sxs-lookup"><span data-stu-id="04649-163">version</span></span>|<span data-ttu-id="04649-164">Int32</span><span class="sxs-lookup"><span data-stu-id="04649-164">Int32</span></span>|<span data-ttu-id="04649-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="04649-165">Version of the device configuration.</span></span> <span data-ttu-id="04649-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="04649-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04649-167">Аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="04649-167">airPrintDestinations</span></span>|<span data-ttu-id="04649-168">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="04649-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="04649-169">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="04649-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="04649-170">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="04649-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="04649-171">НаСледуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="04649-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="04649-172">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="04649-172">assetTagTemplate</span></span>|<span data-ttu-id="04649-173">String</span><span class="sxs-lookup"><span data-stu-id="04649-173">String</span></span>|<span data-ttu-id="04649-174">Сведения о теге ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="04649-174">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="04649-175">Contentfiltersettings к объекту</span><span class="sxs-lookup"><span data-stu-id="04649-175">contentFilterSettings</span></span>|<span data-ttu-id="04649-176">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md);</span><span class="sxs-lookup"><span data-stu-id="04649-176">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>|<span data-ttu-id="04649-177">Получает или задает параметры фильтра веб-содержимого iOS, режим с контролируемым режимом</span><span class="sxs-lookup"><span data-stu-id="04649-177">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="04649-178">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="04649-178">lockScreenFootnote</span></span>|<span data-ttu-id="04649-179">String</span><span class="sxs-lookup"><span data-stu-id="04649-179">String</span></span>|<span data-ttu-id="04649-180">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="04649-180">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="04649-181">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="04649-181">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="04649-182">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="04649-182">homeScreenDockIcons</span></span>|<span data-ttu-id="04649-183">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="04649-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="04649-184">Список приложений и папок, которые должны отображаться на панели Dock на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="04649-184">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="04649-185">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="04649-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="04649-186">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="04649-186">homeScreenPages</span></span>|<span data-ttu-id="04649-187">Коллекция [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="04649-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="04649-188">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="04649-188">A list of pages on the Home Screen.</span></span> <span data-ttu-id="04649-189">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="04649-189">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="04649-190">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="04649-190">notificationSettings</span></span>|<span data-ttu-id="04649-191">Коллекция [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="04649-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="04649-192">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="04649-192">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="04649-193">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="04649-193">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="04649-194">Синглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="04649-194">singleSignOnSettings</span></span>|[<span data-ttu-id="04649-195">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="04649-195">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="04649-196">Параметры входа в систему Kerberos, позволяющие приложениям на принимающих устройствах беспрепятственно выполнять проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="04649-196">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|
|<span data-ttu-id="04649-197">Валлпапердисплайлокатион</span><span class="sxs-lookup"><span data-stu-id="04649-197">wallpaperDisplayLocation</span></span>|[<span data-ttu-id="04649-198">Иосваллпапердисплайлокатион</span><span class="sxs-lookup"><span data-stu-id="04649-198">iosWallpaperDisplayLocation</span></span>](../resources/intune-deviceconfig-ioswallpaperdisplaylocation.md)|<span data-ttu-id="04649-199">Описатель расположения для отображения фонового рисунка.</span><span class="sxs-lookup"><span data-stu-id="04649-199">A wallpaper display location specifier.</span></span> <span data-ttu-id="04649-200">Возможные значения: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span><span class="sxs-lookup"><span data-stu-id="04649-200">Possible values are: `notConfigured`, `lockScreen`, `homeScreen`, `lockAndHomeScreens`.</span></span>|
|<span data-ttu-id="04649-201">Валлпаперимаже</span><span class="sxs-lookup"><span data-stu-id="04649-201">wallpaperImage</span></span>|<span data-ttu-id="04649-202">[mimeContent](../resources/intune-shared-mimecontent.md);</span><span class="sxs-lookup"><span data-stu-id="04649-202">[mimeContent](../resources/intune-shared-mimecontent.md)</span></span>|<span data-ttu-id="04649-203">Изображение фонового рисунка должно иметь формат PNG или JPEG.</span><span class="sxs-lookup"><span data-stu-id="04649-203">A wallpaper image must be in either PNG or JPEG format.</span></span> <span data-ttu-id="04649-204">Для этого требуется контролируемое устройство с iOS 8 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="04649-204">It requires a supervised device with iOS 8 or later version.</span></span>|



## <a name="response"></a><span data-ttu-id="04649-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="04649-205">Response</span></span>
<span data-ttu-id="04649-206">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="04649-206">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04649-207">Пример</span><span class="sxs-lookup"><span data-stu-id="04649-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="04649-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="04649-208">Request</span></span>
<span data-ttu-id="04649-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04649-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="04649-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="04649-210">Response</span></span>
<span data-ttu-id="04649-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04649-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





