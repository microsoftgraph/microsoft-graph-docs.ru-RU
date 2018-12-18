---
title: Update androidGeneralDeviceConfiguration
description: Обновление свойств объекта androidGeneralDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: a495a071577798597685d1ff15e1705968c32d31
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326882"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="80097-103">Update androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="80097-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="80097-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="80097-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80097-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80097-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80097-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="80097-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80097-107">Обновление свойств объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80097-107">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80097-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="80097-108">Prerequisites</span></span>
<span data-ttu-id="80097-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80097-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80097-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80097-111">Permission type</span></span>|<span data-ttu-id="80097-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="80097-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80097-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80097-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80097-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80097-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80097-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80097-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80097-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80097-116">Not supported.</span></span>|
|<span data-ttu-id="80097-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80097-117">Application</span></span>|<span data-ttu-id="80097-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80097-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80097-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80097-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="80097-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80097-120">Request headers</span></span>
|<span data-ttu-id="80097-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80097-121">Header</span></span>|<span data-ttu-id="80097-122">Значение</span><span class="sxs-lookup"><span data-stu-id="80097-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80097-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80097-123">Authorization</span></span>|<span data-ttu-id="80097-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="80097-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80097-125">Accept</span><span class="sxs-lookup"><span data-stu-id="80097-125">Accept</span></span>|<span data-ttu-id="80097-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80097-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80097-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80097-127">Request body</span></span>
<span data-ttu-id="80097-128">В тексте запроса добавьте представление объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80097-128">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="80097-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80097-129">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="80097-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="80097-130">Property</span></span>|<span data-ttu-id="80097-131">Тип</span><span class="sxs-lookup"><span data-stu-id="80097-131">Type</span></span>|<span data-ttu-id="80097-132">Описание</span><span class="sxs-lookup"><span data-stu-id="80097-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80097-133">id</span><span class="sxs-lookup"><span data-stu-id="80097-133">id</span></span>|<span data-ttu-id="80097-134">Строка</span><span class="sxs-lookup"><span data-stu-id="80097-134">String</span></span>|<span data-ttu-id="80097-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="80097-135">Key of the entity.</span></span> <span data-ttu-id="80097-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80097-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80097-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80097-137">lastModifiedDateTime</span></span>|<span data-ttu-id="80097-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80097-138">DateTimeOffset</span></span>|<span data-ttu-id="80097-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="80097-139">DateTime the object was last modified.</span></span> <span data-ttu-id="80097-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80097-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80097-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80097-141">roleScopeTagIds</span></span>|<span data-ttu-id="80097-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="80097-142">String collection</span></span>|<span data-ttu-id="80097-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="80097-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="80097-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80097-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80097-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="80097-145">supportsScopeTags</span></span>|<span data-ttu-id="80097-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="80097-146">Boolean</span></span>|<span data-ttu-id="80097-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="80097-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="80097-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="80097-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="80097-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="80097-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="80097-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80097-150">This property is read-only.</span></span> <span data-ttu-id="80097-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80097-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80097-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80097-152">createdDateTime</span></span>|<span data-ttu-id="80097-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80097-153">DateTimeOffset</span></span>|<span data-ttu-id="80097-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="80097-154">DateTime the object was created.</span></span> <span data-ttu-id="80097-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80097-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80097-156">описание</span><span class="sxs-lookup"><span data-stu-id="80097-156">description</span></span>|<span data-ttu-id="80097-157">Строка</span><span class="sxs-lookup"><span data-stu-id="80097-157">String</span></span>|<span data-ttu-id="80097-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="80097-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="80097-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80097-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80097-160">displayName</span><span class="sxs-lookup"><span data-stu-id="80097-160">displayName</span></span>|<span data-ttu-id="80097-161">Строка</span><span class="sxs-lookup"><span data-stu-id="80097-161">String</span></span>|<span data-ttu-id="80097-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="80097-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="80097-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80097-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80097-164">version</span><span class="sxs-lookup"><span data-stu-id="80097-164">version</span></span>|<span data-ttu-id="80097-165">Int32</span><span class="sxs-lookup"><span data-stu-id="80097-165">Int32</span></span>|<span data-ttu-id="80097-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="80097-166">Version of the device configuration.</span></span> <span data-ttu-id="80097-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80097-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80097-168">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="80097-168">appsBlockClipboardSharing</span></span>|<span data-ttu-id="80097-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-169">Boolean</span></span>|<span data-ttu-id="80097-170">Указывает, следует ли запретить совместное использование буфера обмена для копирования данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="80097-170">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="80097-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="80097-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="80097-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-172">Boolean</span></span>|<span data-ttu-id="80097-173">Указывает, следует ли запретить копирование данных между приложениями.</span><span class="sxs-lookup"><span data-stu-id="80097-173">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="80097-174">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="80097-174">appsBlockYouTube</span></span>|<span data-ttu-id="80097-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-175">Boolean</span></span>|<span data-ttu-id="80097-176">Указывает, следует ли заблокировать приложение YouTube.</span><span class="sxs-lookup"><span data-stu-id="80097-176">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="80097-177">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-177">bluetoothBlocked</span></span>|<span data-ttu-id="80097-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-178">Boolean</span></span>|<span data-ttu-id="80097-179">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="80097-179">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="80097-180">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-180">cameraBlocked</span></span>|<span data-ttu-id="80097-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-181">Boolean</span></span>|<span data-ttu-id="80097-182">Указывает, следует ли запретить использовать камеру.</span><span class="sxs-lookup"><span data-stu-id="80097-182">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="80097-183">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="80097-183">cellularBlockDataRoaming</span></span>|<span data-ttu-id="80097-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-184">Boolean</span></span>|<span data-ttu-id="80097-185">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="80097-185">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="80097-186">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="80097-186">cellularBlockMessaging</span></span>|<span data-ttu-id="80097-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-187">Boolean</span></span>|<span data-ttu-id="80097-188">Указывает, следует ли запретить обмениваться SMS и MMS.</span><span class="sxs-lookup"><span data-stu-id="80097-188">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="80097-189">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="80097-189">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="80097-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-190">Boolean</span></span>|<span data-ttu-id="80097-191">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="80097-191">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="80097-192">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="80097-192">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="80097-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-193">Boolean</span></span>|<span data-ttu-id="80097-194">Указывает, следует ли блокировать синхронизацию модема Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="80097-194">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="80097-195">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="80097-195">compliantAppsList</span></span>|<span data-ttu-id="80097-196">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="80097-196">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="80097-197">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="80097-197">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="80097-198">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="80097-198">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="80097-199">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="80097-199">compliantAppListType</span></span>|[<span data-ttu-id="80097-200">appListType</span><span class="sxs-lookup"><span data-stu-id="80097-200">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="80097-201">Тип списка, определенного свойством CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="80097-201">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="80097-202">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="80097-202">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="80097-203">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="80097-203">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="80097-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-204">Boolean</span></span>|<span data-ttu-id="80097-205">Указывает, следует ли блокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="80097-205">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="80097-206">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-206">locationServicesBlocked</span></span>|<span data-ttu-id="80097-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-207">Boolean</span></span>|<span data-ttu-id="80097-208">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="80097-208">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="80097-209">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="80097-209">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="80097-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-210">Boolean</span></span>|<span data-ttu-id="80097-211">Указывает, следует ли блокировать автоматическую синхронизацию учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="80097-211">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="80097-212">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-212">googlePlayStoreBlocked</span></span>|<span data-ttu-id="80097-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-213">Boolean</span></span>|<span data-ttu-id="80097-214">Указывает, следует ли блокировать Google Play Маркет.</span><span class="sxs-lookup"><span data-stu-id="80097-214">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="80097-215">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="80097-215">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="80097-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-216">Boolean</span></span>|<span data-ttu-id="80097-217">Указывает, следует ли блокировать кнопку спящего режима экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="80097-217">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="80097-218">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="80097-218">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="80097-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-219">Boolean</span></span>|<span data-ttu-id="80097-220">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="80097-220">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="80097-221">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="80097-221">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="80097-222">Boolean.</span><span class="sxs-lookup"><span data-stu-id="80097-222">Boolean</span></span>|<span data-ttu-id="80097-223">Указывает, следует ли блокировать изменение даты и времени в режиме НОКСА.</span><span class="sxs-lookup"><span data-stu-id="80097-223">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="80097-224">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="80097-224">kioskModeApps</span></span>|<span data-ttu-id="80097-225">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="80097-225">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="80097-226">Список разрешенных приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="80097-226">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="80097-227">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="80097-227">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="80097-228">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-228">nfcBlocked</span></span>|<span data-ttu-id="80097-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-229">Boolean</span></span>|<span data-ttu-id="80097-230">Указывает, следует ли блокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="80097-230">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="80097-231">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="80097-231">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="80097-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-232">Boolean</span></span>|<span data-ttu-id="80097-233">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="80097-233">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="80097-234">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="80097-234">passwordBlockTrustAgents</span></span>|<span data-ttu-id="80097-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-235">Boolean</span></span>|<span data-ttu-id="80097-236">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="80097-236">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="80097-237">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="80097-237">passwordExpirationDays</span></span>|<span data-ttu-id="80097-238">Int32</span><span class="sxs-lookup"><span data-stu-id="80097-238">Int32</span></span>|<span data-ttu-id="80097-239">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="80097-239">Number of days before the password expires.</span></span> <span data-ttu-id="80097-240">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="80097-240">Valid values 1 to 365</span></span>|
|<span data-ttu-id="80097-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="80097-241">passwordMinimumLength</span></span>|<span data-ttu-id="80097-242">Int32</span><span class="sxs-lookup"><span data-stu-id="80097-242">Int32</span></span>|<span data-ttu-id="80097-243">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="80097-243">Minimum length of passwords.</span></span> <span data-ttu-id="80097-244">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="80097-244">Valid values 4 to 16</span></span>|
|<span data-ttu-id="80097-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="80097-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="80097-246">Int32</span><span class="sxs-lookup"><span data-stu-id="80097-246">Int32</span></span>|<span data-ttu-id="80097-247">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="80097-247">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="80097-248">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="80097-248">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="80097-249">Int32</span><span class="sxs-lookup"><span data-stu-id="80097-249">Int32</span></span>|<span data-ttu-id="80097-250">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="80097-250">Number of previous passwords to block.</span></span> <span data-ttu-id="80097-251">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="80097-251">Valid values 0 to 24</span></span>|
|<span data-ttu-id="80097-252">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="80097-252">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="80097-253">Int32</span><span class="sxs-lookup"><span data-stu-id="80097-253">Int32</span></span>|<span data-ttu-id="80097-254">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="80097-254">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="80097-255">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="80097-255">Valid values 4 to 11</span></span>|
|<span data-ttu-id="80097-256">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="80097-256">passwordRequiredType</span></span>|[<span data-ttu-id="80097-257">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="80097-257">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="80097-258">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="80097-258">Type of password that is required.</span></span> <span data-ttu-id="80097-259">Возможные значения: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="80097-259">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="80097-260">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="80097-260">passwordRequired</span></span>|<span data-ttu-id="80097-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-261">Boolean</span></span>|<span data-ttu-id="80097-262">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="80097-262">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="80097-263">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-263">powerOffBlocked</span></span>|<span data-ttu-id="80097-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-264">Boolean</span></span>|<span data-ttu-id="80097-265">Указывает, следует ли блокировать отключение устройства.</span><span class="sxs-lookup"><span data-stu-id="80097-265">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="80097-266">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-266">factoryResetBlocked</span></span>|<span data-ttu-id="80097-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-267">Boolean</span></span>|<span data-ttu-id="80097-268">Указывает, следует ли запретить пользователю восстанавливать заводские настройки.</span><span class="sxs-lookup"><span data-stu-id="80097-268">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="80097-269">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-269">screenCaptureBlocked</span></span>|<span data-ttu-id="80097-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-270">Boolean</span></span>|<span data-ttu-id="80097-271">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="80097-271">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="80097-272">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="80097-272">deviceSharingAllowed</span></span>|<span data-ttu-id="80097-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-273">Boolean</span></span>|<span data-ttu-id="80097-274">Указывает, следует ли разрешить режим совместного доступа к устройству.</span><span class="sxs-lookup"><span data-stu-id="80097-274">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="80097-275">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="80097-275">storageBlockGoogleBackup</span></span>|<span data-ttu-id="80097-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-276">Boolean</span></span>|<span data-ttu-id="80097-277">Указывает, следует ли блокировать резервное копирование Google.</span><span class="sxs-lookup"><span data-stu-id="80097-277">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="80097-278">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="80097-278">storageBlockRemovableStorage</span></span>|<span data-ttu-id="80097-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-279">Boolean</span></span>|<span data-ttu-id="80097-280">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="80097-280">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="80097-281">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="80097-281">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="80097-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-282">Boolean</span></span>|<span data-ttu-id="80097-283">Указывает, обязательно ли шифрование устройства.</span><span class="sxs-lookup"><span data-stu-id="80097-283">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="80097-284">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="80097-284">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="80097-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-285">Boolean</span></span>|<span data-ttu-id="80097-286">Указывает, обязательно ли шифрование съемных носителей.</span><span class="sxs-lookup"><span data-stu-id="80097-286">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="80097-287">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-287">voiceAssistantBlocked</span></span>|<span data-ttu-id="80097-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-288">Boolean</span></span>|<span data-ttu-id="80097-289">Указывает, следует ли блокировать использование голосового помощника.</span><span class="sxs-lookup"><span data-stu-id="80097-289">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="80097-290">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-290">voiceDialingBlocked</span></span>|<span data-ttu-id="80097-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-291">Boolean</span></span>|<span data-ttu-id="80097-292">Указывает, следует ли блокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="80097-292">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="80097-293">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="80097-293">webBrowserBlockPopups</span></span>|<span data-ttu-id="80097-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-294">Boolean</span></span>|<span data-ttu-id="80097-295">Указывает, следует ли блокировать всплывающие окна в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="80097-295">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="80097-296">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="80097-296">webBrowserBlockAutofill</span></span>|<span data-ttu-id="80097-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-297">Boolean</span></span>|<span data-ttu-id="80097-298">Указывает, следует ли заблокировать функцию автозаполнения в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="80097-298">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="80097-299">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="80097-299">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="80097-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-300">Boolean</span></span>|<span data-ttu-id="80097-301">Указывает, следует ли заблокировать JavaScript в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="80097-301">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="80097-302">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-302">webBrowserBlocked</span></span>|<span data-ttu-id="80097-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-303">Boolean</span></span>|<span data-ttu-id="80097-304">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="80097-304">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="80097-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="80097-305">webBrowserCookieSettings</span></span>|[<span data-ttu-id="80097-306">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="80097-306">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="80097-307">Настройки файлов cookie в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="80097-307">Cookie settings within the web browser.</span></span> <span data-ttu-id="80097-308">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="80097-308">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="80097-309">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="80097-309">wiFiBlocked</span></span>|<span data-ttu-id="80097-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-310">Boolean</span></span>|<span data-ttu-id="80097-311">Указывает, следует ли заблокировать синхронизацию Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="80097-311">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="80097-312">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="80097-312">appsInstallAllowList</span></span>|<span data-ttu-id="80097-313">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="80097-313">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="80097-314">Список приложений, которые можно установить на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="80097-314">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="80097-315">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="80097-315">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="80097-316">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="80097-316">appsLaunchBlockList</span></span>|<span data-ttu-id="80097-317">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="80097-317">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="80097-318">Список приложений, которые запрещено запускать на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="80097-318">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="80097-319">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="80097-319">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="80097-320">appsHideList</span><span class="sxs-lookup"><span data-stu-id="80097-320">appsHideList</span></span>|<span data-ttu-id="80097-321">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="80097-321">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="80097-322">Список приложений, которые следует скрыть на устройстве KNOX.</span><span class="sxs-lookup"><span data-stu-id="80097-322">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="80097-323">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="80097-323">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="80097-324">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="80097-324">securityRequireVerifyApps</span></span>|<span data-ttu-id="80097-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="80097-325">Boolean</span></span>|<span data-ttu-id="80097-326">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="80097-326">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="80097-327">Ответ</span><span class="sxs-lookup"><span data-stu-id="80097-327">Response</span></span>
<span data-ttu-id="80097-328">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="80097-328">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80097-329">Пример</span><span class="sxs-lookup"><span data-stu-id="80097-329">Example</span></span>
### <a name="request"></a><span data-ttu-id="80097-330">Запрос</span><span class="sxs-lookup"><span data-stu-id="80097-330">Request</span></span>
<span data-ttu-id="80097-331">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80097-331">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3153

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="80097-332">Ответ</span><span class="sxs-lookup"><span data-stu-id="80097-332">Response</span></span>
<span data-ttu-id="80097-p123">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="80097-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3333

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```





