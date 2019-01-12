---
title: Update iosDeviceFeaturesConfiguration
description: Обновление свойств объекта iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 730b44d05582c48ace0e3ab399a6669a97d42c7e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950188"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="a70db-103">Update iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="a70db-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="a70db-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a70db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a70db-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a70db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a70db-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a70db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a70db-107">Обновление свойств объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70db-107">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a70db-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a70db-108">Prerequisites</span></span>
<span data-ttu-id="a70db-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a70db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a70db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a70db-111">Permission type</span></span>|<span data-ttu-id="a70db-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a70db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a70db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a70db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a70db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a70db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a70db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a70db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a70db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a70db-116">Not supported.</span></span>|
|<span data-ttu-id="a70db-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a70db-117">Application</span></span>|<span data-ttu-id="a70db-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a70db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a70db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a70db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a70db-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a70db-120">Request headers</span></span>
|<span data-ttu-id="a70db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a70db-121">Header</span></span>|<span data-ttu-id="a70db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a70db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a70db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a70db-123">Authorization</span></span>|<span data-ttu-id="a70db-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a70db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a70db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a70db-125">Accept</span></span>|<span data-ttu-id="a70db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a70db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a70db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a70db-127">Request body</span></span>
<span data-ttu-id="a70db-128">В тексте запроса добавьте представление объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a70db-128">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="a70db-129">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70db-129">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="a70db-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a70db-130">Property</span></span>|<span data-ttu-id="a70db-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a70db-131">Type</span></span>|<span data-ttu-id="a70db-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a70db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a70db-133">id</span><span class="sxs-lookup"><span data-stu-id="a70db-133">id</span></span>|<span data-ttu-id="a70db-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a70db-134">String</span></span>|<span data-ttu-id="a70db-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a70db-135">Key of the entity.</span></span> <span data-ttu-id="a70db-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70db-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70db-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a70db-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a70db-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a70db-138">DateTimeOffset</span></span>|<span data-ttu-id="a70db-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a70db-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a70db-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70db-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70db-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a70db-141">roleScopeTagIds</span></span>|<span data-ttu-id="a70db-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a70db-142">String collection</span></span>|<span data-ttu-id="a70db-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a70db-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a70db-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70db-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70db-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a70db-145">supportsScopeTags</span></span>|<span data-ttu-id="a70db-146">Логический</span><span class="sxs-lookup"><span data-stu-id="a70db-146">Boolean</span></span>|<span data-ttu-id="a70db-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="a70db-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a70db-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="a70db-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a70db-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a70db-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a70db-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a70db-150">This property is read-only.</span></span> <span data-ttu-id="a70db-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70db-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70db-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a70db-152">createdDateTime</span></span>|<span data-ttu-id="a70db-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a70db-153">DateTimeOffset</span></span>|<span data-ttu-id="a70db-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a70db-154">DateTime the object was created.</span></span> <span data-ttu-id="a70db-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70db-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70db-156">описание</span><span class="sxs-lookup"><span data-stu-id="a70db-156">description</span></span>|<span data-ttu-id="a70db-157">Строка</span><span class="sxs-lookup"><span data-stu-id="a70db-157">String</span></span>|<span data-ttu-id="a70db-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a70db-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a70db-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70db-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70db-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a70db-160">displayName</span></span>|<span data-ttu-id="a70db-161">Строка</span><span class="sxs-lookup"><span data-stu-id="a70db-161">String</span></span>|<span data-ttu-id="a70db-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a70db-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a70db-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70db-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70db-164">version</span><span class="sxs-lookup"><span data-stu-id="a70db-164">version</span></span>|<span data-ttu-id="a70db-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a70db-165">Int32</span></span>|<span data-ttu-id="a70db-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a70db-166">Version of the device configuration.</span></span> <span data-ttu-id="a70db-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70db-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70db-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="a70db-168">airPrintDestinations</span></span>|<span data-ttu-id="a70db-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a70db-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="a70db-170">Массив AirPrint принтеров, которые всегда должны быть отображены.</span><span class="sxs-lookup"><span data-stu-id="a70db-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="a70db-171">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a70db-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a70db-172">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="a70db-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="a70db-173">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="a70db-173">assetTagTemplate</span></span>|<span data-ttu-id="a70db-174">String</span><span class="sxs-lookup"><span data-stu-id="a70db-174">String</span></span>|<span data-ttu-id="a70db-175">Сведения о теге ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="a70db-175">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="a70db-176">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="a70db-176">contentFilterSettings</span></span>|<span data-ttu-id="a70db-177">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md);</span><span class="sxs-lookup"><span data-stu-id="a70db-177">[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>|<span data-ttu-id="a70db-178">Получает или задает параметры фильтра веб-содержимого, контролируемом режим только операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="a70db-178">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="a70db-179">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="a70db-179">lockScreenFootnote</span></span>|<span data-ttu-id="a70db-180">String</span><span class="sxs-lookup"><span data-stu-id="a70db-180">String</span></span>|<span data-ttu-id="a70db-181">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="a70db-181">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="a70db-182">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="a70db-182">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="a70db-183">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="a70db-183">homeScreenDockIcons</span></span>|<span data-ttu-id="a70db-184">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a70db-184">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="a70db-185">Список приложений и папок, которые должны отображаться на панели Dock на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="a70db-185">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="a70db-186">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a70db-186">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a70db-187">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="a70db-187">homeScreenPages</span></span>|<span data-ttu-id="a70db-188">Коллекция [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="a70db-188">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="a70db-189">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="a70db-189">A list of pages on the Home Screen.</span></span> <span data-ttu-id="a70db-190">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a70db-190">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a70db-191">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="a70db-191">notificationSettings</span></span>|<span data-ttu-id="a70db-192">Коллекция [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a70db-192">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="a70db-193">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a70db-193">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="a70db-194">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a70db-194">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a70db-195">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="a70db-195">singleSignOnSettings</span></span>|[<span data-ttu-id="a70db-196">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="a70db-196">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="a70db-197">Параметры входа в систему Kerberos, которые позволяют приложения на получение устройства для проверки подлинности беспрепятственно.</span><span class="sxs-lookup"><span data-stu-id="a70db-197">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|



## <a name="response"></a><span data-ttu-id="a70db-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="a70db-198">Response</span></span>
<span data-ttu-id="a70db-199">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a70db-199">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a70db-200">Пример</span><span class="sxs-lookup"><span data-stu-id="a70db-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="a70db-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="a70db-201">Request</span></span>
<span data-ttu-id="a70db-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a70db-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3474

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="a70db-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="a70db-203">Response</span></span>
<span data-ttu-id="a70db-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a70db-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3651

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
  }
}
```





