---
title: Обновление объекта iosGeneralDeviceConfiguration
description: Обновление свойств объекта iosGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f72ae25934e08c228375dbfefc6a243e87792b82
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974365"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="861f7-103">Обновление объекта iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="861f7-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="861f7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="861f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="861f7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="861f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="861f7-106">Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="861f7-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="861f7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="861f7-107">Prerequisites</span></span>
<span data-ttu-id="861f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="861f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="861f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="861f7-110">Permission type</span></span>|<span data-ttu-id="861f7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="861f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="861f7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="861f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="861f7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861f7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="861f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="861f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="861f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="861f7-115">Not supported.</span></span>|
|<span data-ttu-id="861f7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="861f7-116">Application</span></span>|<span data-ttu-id="861f7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="861f7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="861f7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="861f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="861f7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="861f7-119">Request headers</span></span>
|<span data-ttu-id="861f7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="861f7-120">Header</span></span>|<span data-ttu-id="861f7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="861f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="861f7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="861f7-122">Authorization</span></span>|<span data-ttu-id="861f7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="861f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="861f7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="861f7-124">Accept</span></span>|<span data-ttu-id="861f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="861f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="861f7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="861f7-126">Request body</span></span>
<span data-ttu-id="861f7-127">В тексте запроса добавьте представление объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="861f7-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="861f7-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="861f7-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="861f7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="861f7-129">Property</span></span>|<span data-ttu-id="861f7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="861f7-130">Type</span></span>|<span data-ttu-id="861f7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="861f7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="861f7-132">id</span><span class="sxs-lookup"><span data-stu-id="861f7-132">id</span></span>|<span data-ttu-id="861f7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="861f7-133">String</span></span>|<span data-ttu-id="861f7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="861f7-134">Key of the entity.</span></span> <span data-ttu-id="861f7-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="861f7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="861f7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="861f7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="861f7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="861f7-137">DateTimeOffset</span></span>|<span data-ttu-id="861f7-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="861f7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="861f7-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="861f7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="861f7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="861f7-140">roleScopeTagIds</span></span>|<span data-ttu-id="861f7-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="861f7-141">String collection</span></span>|<span data-ttu-id="861f7-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="861f7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="861f7-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="861f7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="861f7-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="861f7-144">supportsScopeTags</span></span>|<span data-ttu-id="861f7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-145">Boolean</span></span>|<span data-ttu-id="861f7-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="861f7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="861f7-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="861f7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="861f7-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="861f7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="861f7-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="861f7-149">This property is read-only.</span></span> <span data-ttu-id="861f7-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="861f7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="861f7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="861f7-151">createdDateTime</span></span>|<span data-ttu-id="861f7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="861f7-152">DateTimeOffset</span></span>|<span data-ttu-id="861f7-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="861f7-153">DateTime the object was created.</span></span> <span data-ttu-id="861f7-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="861f7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="861f7-155">description</span><span class="sxs-lookup"><span data-stu-id="861f7-155">description</span></span>|<span data-ttu-id="861f7-156">String</span><span class="sxs-lookup"><span data-stu-id="861f7-156">String</span></span>|<span data-ttu-id="861f7-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="861f7-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="861f7-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="861f7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="861f7-159">displayName</span><span class="sxs-lookup"><span data-stu-id="861f7-159">displayName</span></span>|<span data-ttu-id="861f7-160">String</span><span class="sxs-lookup"><span data-stu-id="861f7-160">String</span></span>|<span data-ttu-id="861f7-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="861f7-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="861f7-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="861f7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="861f7-163">version</span><span class="sxs-lookup"><span data-stu-id="861f7-163">version</span></span>|<span data-ttu-id="861f7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="861f7-164">Int32</span></span>|<span data-ttu-id="861f7-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="861f7-165">Version of the device configuration.</span></span> <span data-ttu-id="861f7-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="861f7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="861f7-167">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="861f7-167">accountBlockModification</span></span>|<span data-ttu-id="861f7-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-168">Boolean</span></span>|<span data-ttu-id="861f7-169">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-169">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-170">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="861f7-170">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="861f7-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-171">Boolean</span></span>|<span data-ttu-id="861f7-172">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-172">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="861f7-173">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-173">airDropBlocked</span></span>|<span data-ttu-id="861f7-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-174">Boolean</span></span>|<span data-ttu-id="861f7-175">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-175">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-176">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="861f7-176">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="861f7-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-177">Boolean</span></span>|<span data-ttu-id="861f7-178">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-178">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="861f7-179">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="861f7-179">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="861f7-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-180">Boolean</span></span>|<span data-ttu-id="861f7-181">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="861f7-181">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="861f7-182">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="861f7-182">appleWatchBlockPairing</span></span>|<span data-ttu-id="861f7-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-183">Boolean</span></span>|<span data-ttu-id="861f7-184">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-184">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="861f7-185">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="861f7-185">appleWatchForceWristDetection</span></span>|<span data-ttu-id="861f7-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-186">Boolean</span></span>|<span data-ttu-id="861f7-187">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-187">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="861f7-188">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-188">appleNewsBlocked</span></span>|<span data-ttu-id="861f7-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-189">Boolean</span></span>|<span data-ttu-id="861f7-190">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-190">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="861f7-191">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="861f7-191">appsSingleAppModeList</span></span>|<span data-ttu-id="861f7-192">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="861f7-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="861f7-193">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="861f7-193">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="861f7-194">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-194">Supervised only.</span></span> <span data-ttu-id="861f7-195">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="861f7-195">iOS 7.0 and later.</span></span> <span data-ttu-id="861f7-196">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="861f7-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="861f7-197">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="861f7-197">appsVisibilityList</span></span>|<span data-ttu-id="861f7-198">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="861f7-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="861f7-199">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-199">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="861f7-200">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="861f7-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="861f7-201">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="861f7-201">appsVisibilityListType</span></span>|[<span data-ttu-id="861f7-202">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="861f7-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="861f7-203">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="861f7-203">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="861f7-204">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="861f7-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="861f7-205">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="861f7-205">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="861f7-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-206">Boolean</span></span>|<span data-ttu-id="861f7-207">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-207">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="861f7-208">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-208">appStoreBlocked</span></span>|<span data-ttu-id="861f7-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-209">Boolean</span></span>|<span data-ttu-id="861f7-210">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="861f7-210">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="861f7-211">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="861f7-211">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="861f7-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-212">Boolean</span></span>|<span data-ttu-id="861f7-213">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="861f7-213">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="861f7-214">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="861f7-214">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="861f7-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-215">Boolean</span></span>|<span data-ttu-id="861f7-216">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="861f7-216">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="861f7-217">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-217">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="861f7-218">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="861f7-218">appStoreRequirePassword</span></span>|<span data-ttu-id="861f7-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-219">Boolean</span></span>|<span data-ttu-id="861f7-220">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="861f7-220">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="861f7-221">Аутофиллфорцеаусентикатион</span><span class="sxs-lookup"><span data-stu-id="861f7-221">autoFillForceAuthentication</span></span>|<span data-ttu-id="861f7-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-222">Boolean</span></span>|<span data-ttu-id="861f7-223">Указывает, следует ли принудительно выполнять проверку подлинности пользователей перед автозаполнением паролей и сведений о кредитных картах в Safari и других приложениях на контролируемых устройствах.</span><span class="sxs-lookup"><span data-stu-id="861f7-223">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="861f7-224">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="861f7-224">bluetoothBlockModification</span></span>|<span data-ttu-id="861f7-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-225">Boolean</span></span>|<span data-ttu-id="861f7-226">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-226">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="861f7-227">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-227">cameraBlocked</span></span>|<span data-ttu-id="861f7-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-228">Boolean</span></span>|<span data-ttu-id="861f7-229">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="861f7-229">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="861f7-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="861f7-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="861f7-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-231">Boolean</span></span>|<span data-ttu-id="861f7-232">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="861f7-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="861f7-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="861f7-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="861f7-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-234">Boolean</span></span>|<span data-ttu-id="861f7-235">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="861f7-235">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="861f7-236">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="861f7-236">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="861f7-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-237">Boolean</span></span>|<span data-ttu-id="861f7-238">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-238">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-239">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="861f7-239">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="861f7-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-240">Boolean</span></span>|<span data-ttu-id="861f7-241">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="861f7-241">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="861f7-242">Целлуларблоккпланмодификатион</span><span class="sxs-lookup"><span data-stu-id="861f7-242">cellularBlockPlanModification</span></span>|<span data-ttu-id="861f7-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-243">Boolean</span></span>|<span data-ttu-id="861f7-244">Указывает, следует ли запретить пользователям изменять параметры плана сотовой связи на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="861f7-244">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="861f7-245">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="861f7-245">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="861f7-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-246">Boolean</span></span>|<span data-ttu-id="861f7-247">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="861f7-247">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="861f7-248">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="861f7-248">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="861f7-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-249">Boolean</span></span>|<span data-ttu-id="861f7-250">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="861f7-250">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="861f7-251">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="861f7-251">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="861f7-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-252">Boolean</span></span>|<span data-ttu-id="861f7-253">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-253">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="861f7-254">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="861f7-254">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="861f7-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-255">Boolean</span></span>|<span data-ttu-id="861f7-256">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-256">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-257">Классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="861f7-257">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="861f7-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-258">Boolean</span></span>|<span data-ttu-id="861f7-259">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-259">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-260">Классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="861f7-260">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="861f7-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-261">Boolean</span></span>|<span data-ttu-id="861f7-262">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="861f7-262">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="861f7-263">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-263">Supervised only.</span></span>|
|<span data-ttu-id="861f7-264">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="861f7-264">compliantAppsList</span></span>|<span data-ttu-id="861f7-265">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="861f7-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="861f7-266">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="861f7-266">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="861f7-267">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="861f7-267">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="861f7-268">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="861f7-268">compliantAppListType</span></span>|[<span data-ttu-id="861f7-269">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="861f7-269">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="861f7-270">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="861f7-270">List that is in the AppComplianceList.</span></span> <span data-ttu-id="861f7-271">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="861f7-271">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="861f7-272">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="861f7-272">configurationProfileBlockChanges</span></span>|<span data-ttu-id="861f7-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-273">Boolean</span></span>|<span data-ttu-id="861f7-274">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-274">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-275">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-275">definitionLookupBlocked</span></span>|<span data-ttu-id="861f7-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-276">Boolean</span></span>|<span data-ttu-id="861f7-277">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-277">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="861f7-278">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="861f7-278">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="861f7-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-279">Boolean</span></span>|<span data-ttu-id="861f7-280">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-280">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-281">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="861f7-281">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="861f7-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-282">Boolean</span></span>|<span data-ttu-id="861f7-283">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-283">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-284">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="861f7-284">deviceBlockNameModification</span></span>|<span data-ttu-id="861f7-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-285">Boolean</span></span>|<span data-ttu-id="861f7-286">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-286">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="861f7-287">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="861f7-287">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="861f7-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-288">Boolean</span></span>|<span data-ttu-id="861f7-289">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="861f7-289">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="861f7-290">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="861f7-290">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="861f7-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-291">Boolean</span></span>|<span data-ttu-id="861f7-292">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-292">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="861f7-293">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="861f7-293">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="861f7-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-294">Boolean</span></span>|<span data-ttu-id="861f7-295">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="861f7-295">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="861f7-296">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="861f7-296">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="861f7-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-297">Boolean</span></span>|<span data-ttu-id="861f7-298">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="861f7-298">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="861f7-299">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="861f7-299">emailInDomainSuffixes</span></span>|<span data-ttu-id="861f7-300">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="861f7-300">String collection</span></span>|<span data-ttu-id="861f7-301">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="861f7-301">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="861f7-302">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="861f7-302">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="861f7-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-303">Boolean</span></span>|<span data-ttu-id="861f7-304">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="861f7-304">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="861f7-305">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="861f7-305">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="861f7-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-306">Boolean</span></span>|<span data-ttu-id="861f7-307">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="861f7-307">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="861f7-308">Есимблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="861f7-308">esimBlockModification</span></span>|<span data-ttu-id="861f7-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-309">Boolean</span></span>|<span data-ttu-id="861f7-310">Указывает, следует ли разрешить добавление или удаление планов сотовой связи на eSIM контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="861f7-310">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="861f7-311">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-311">faceTimeBlocked</span></span>|<span data-ttu-id="861f7-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-312">Boolean</span></span>|<span data-ttu-id="861f7-313">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="861f7-313">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="861f7-314">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-314">findMyFriendsBlocked</span></span>|<span data-ttu-id="861f7-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-315">Boolean</span></span>|<span data-ttu-id="861f7-316">Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-316">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-317">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="861f7-317">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="861f7-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-318">Boolean</span></span>|<span data-ttu-id="861f7-319">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="861f7-319">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="861f7-320">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="861f7-320">gamingBlockMultiplayer</span></span>|<span data-ttu-id="861f7-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-321">Boolean</span></span>|<span data-ttu-id="861f7-322">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="861f7-322">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="861f7-323">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-323">gameCenterBlocked</span></span>|<span data-ttu-id="861f7-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-324">Boolean</span></span>|<span data-ttu-id="861f7-325">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-325">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-326">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-326">hostPairingBlocked</span></span>|<span data-ttu-id="861f7-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-327">Boolean</span></span>|<span data-ttu-id="861f7-328">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-328">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-329">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-329">iBooksStoreBlocked</span></span>|<span data-ttu-id="861f7-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-330">Boolean</span></span>|<span data-ttu-id="861f7-331">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-331">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-332">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="861f7-332">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="861f7-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-333">Boolean</span></span>|<span data-ttu-id="861f7-334">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="861f7-334">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="861f7-335">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="861f7-335">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="861f7-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-336">Boolean</span></span>|<span data-ttu-id="861f7-337">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="861f7-337">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="861f7-338">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="861f7-338">iCloudBlockBackup</span></span>|<span data-ttu-id="861f7-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-339">Boolean</span></span>|<span data-ttu-id="861f7-340">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="861f7-340">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="861f7-341">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="861f7-341">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="861f7-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-342">Boolean</span></span>|<span data-ttu-id="861f7-343">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="861f7-343">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="861f7-344">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="861f7-344">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="861f7-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-345">Boolean</span></span>|<span data-ttu-id="861f7-346">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="861f7-346">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="861f7-347">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="861f7-347">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="861f7-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-348">Boolean</span></span>|<span data-ttu-id="861f7-349">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="861f7-349">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="861f7-350">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="861f7-350">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="861f7-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-351">Boolean</span></span>|<span data-ttu-id="861f7-352">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="861f7-352">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="861f7-353">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="861f7-353">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="861f7-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-354">Boolean</span></span>|<span data-ttu-id="861f7-355">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="861f7-355">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="861f7-356">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="861f7-356">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="861f7-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-357">Boolean</span></span>|<span data-ttu-id="861f7-358">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="861f7-358">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="861f7-359">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="861f7-359">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="861f7-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-360">Boolean</span></span>|<span data-ttu-id="861f7-361">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="861f7-361">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="861f7-362">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="861f7-362">iTunesBlockMusicService</span></span>|<span data-ttu-id="861f7-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-363">Boolean</span></span>|<span data-ttu-id="861f7-364">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-364">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="861f7-365">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="861f7-365">iTunesBlockRadio</span></span>|<span data-ttu-id="861f7-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-366">Boolean</span></span>|<span data-ttu-id="861f7-367">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-367">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="861f7-368">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="861f7-368">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="861f7-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-369">Boolean</span></span>|<span data-ttu-id="861f7-370">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-370">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="861f7-371">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="861f7-371">keyboardBlockDictation</span></span>|<span data-ttu-id="861f7-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-372">Boolean</span></span>|<span data-ttu-id="861f7-373">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-373">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-374">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="861f7-374">keyboardBlockPredictive</span></span>|<span data-ttu-id="861f7-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-375">Boolean</span></span>|<span data-ttu-id="861f7-376">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-376">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="861f7-377">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="861f7-377">keyboardBlockShortcuts</span></span>|<span data-ttu-id="861f7-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-378">Boolean</span></span>|<span data-ttu-id="861f7-379">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-379">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="861f7-380">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="861f7-380">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="861f7-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-381">Boolean</span></span>|<span data-ttu-id="861f7-382">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-382">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="861f7-383">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="861f7-383">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="861f7-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-384">Boolean</span></span>|<span data-ttu-id="861f7-385">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-385">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-386">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="861f7-386">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="861f7-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-387">Boolean</span></span>|<span data-ttu-id="861f7-388">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-388">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-389">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="861f7-389">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="861f7-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-390">Boolean</span></span>|<span data-ttu-id="861f7-391">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-391">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-392">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="861f7-392">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="861f7-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-393">Boolean</span></span>|<span data-ttu-id="861f7-394">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-394">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-395">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="861f7-395">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="861f7-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-396">Boolean</span></span>|<span data-ttu-id="861f7-397">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-397">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-398">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="861f7-398">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="861f7-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-399">Boolean</span></span>|<span data-ttu-id="861f7-400">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-400">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-401">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="861f7-401">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="861f7-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-402">Boolean</span></span>|<span data-ttu-id="861f7-403">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-403">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-404">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="861f7-404">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="861f7-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-405">Boolean</span></span>|<span data-ttu-id="861f7-406">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-406">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-407">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="861f7-407">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="861f7-408">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-408">Boolean</span></span>|<span data-ttu-id="861f7-409">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-409">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-410">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="861f7-410">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="861f7-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-411">Boolean</span></span>|<span data-ttu-id="861f7-412">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-412">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-413">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="861f7-413">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="861f7-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-414">Boolean</span></span>|<span data-ttu-id="861f7-415">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="861f7-415">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="861f7-416">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="861f7-416">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="861f7-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-417">Boolean</span></span>|<span data-ttu-id="861f7-418">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-418">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-419">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="861f7-419">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="861f7-420">String</span><span class="sxs-lookup"><span data-stu-id="861f7-420">String</span></span>|<span data-ttu-id="861f7-421">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-421">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="861f7-422">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="861f7-422">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="861f7-423">Киоскмодебуилтинаппид</span><span class="sxs-lookup"><span data-stu-id="861f7-423">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="861f7-424">String</span><span class="sxs-lookup"><span data-stu-id="861f7-424">String</span></span>|<span data-ttu-id="861f7-425">Идентификатор встроенных приложений для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-425">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="861f7-426">Используется, когда KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.</span><span class="sxs-lookup"><span data-stu-id="861f7-426">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="861f7-427">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="861f7-427">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="861f7-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-428">Boolean</span></span>|<span data-ttu-id="861f7-429">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-429">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-430">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="861f7-430">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="861f7-431">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-431">Boolean</span></span>|<span data-ttu-id="861f7-432">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-432">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-433">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="861f7-433">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="861f7-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-434">Boolean</span></span>|<span data-ttu-id="861f7-435">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-435">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-436">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="861f7-436">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="861f7-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-437">Boolean</span></span>|<span data-ttu-id="861f7-438">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-438">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-439">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="861f7-439">kioskModeRequireZoom</span></span>|<span data-ttu-id="861f7-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-440">Boolean</span></span>|<span data-ttu-id="861f7-441">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-441">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="861f7-442">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="861f7-442">kioskModeManagedAppId</span></span>|<span data-ttu-id="861f7-443">String</span><span class="sxs-lookup"><span data-stu-id="861f7-443">String</span></span>|<span data-ttu-id="861f7-444">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="861f7-444">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="861f7-445">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="861f7-445">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="861f7-446">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="861f7-446">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="861f7-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-447">Boolean</span></span>|<span data-ttu-id="861f7-448">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="861f7-448">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="861f7-449">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="861f7-449">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="861f7-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-450">Boolean</span></span>|<span data-ttu-id="861f7-451">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="861f7-451">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="861f7-452">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="861f7-452">lockScreenBlockPassbook</span></span>|<span data-ttu-id="861f7-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-453">Boolean</span></span>|<span data-ttu-id="861f7-454">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="861f7-454">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="861f7-455">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="861f7-455">lockScreenBlockTodayView</span></span>|<span data-ttu-id="861f7-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-456">Boolean</span></span>|<span data-ttu-id="861f7-457">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="861f7-457">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="861f7-458">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="861f7-458">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="861f7-459">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="861f7-459">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="861f7-460">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="861f7-460">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="861f7-461">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="861f7-461">mediaContentRatingCanada</span></span>|[<span data-ttu-id="861f7-462">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="861f7-462">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="861f7-463">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="861f7-463">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="861f7-464">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="861f7-464">mediaContentRatingFrance</span></span>|[<span data-ttu-id="861f7-465">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="861f7-465">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="861f7-466">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="861f7-466">Media content rating settings for France</span></span>|
|<span data-ttu-id="861f7-467">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="861f7-467">mediaContentRatingGermany</span></span>|[<span data-ttu-id="861f7-468">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="861f7-468">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="861f7-469">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="861f7-469">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="861f7-470">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="861f7-470">mediaContentRatingIreland</span></span>|[<span data-ttu-id="861f7-471">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="861f7-471">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="861f7-472">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="861f7-472">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="861f7-473">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="861f7-473">mediaContentRatingJapan</span></span>|[<span data-ttu-id="861f7-474">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="861f7-474">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="861f7-475">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="861f7-475">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="861f7-476">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="861f7-476">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="861f7-477">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="861f7-477">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="861f7-478">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="861f7-478">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="861f7-479">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="861f7-479">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="861f7-480">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="861f7-480">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="861f7-481">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="861f7-481">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="861f7-482">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="861f7-482">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="861f7-483">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="861f7-483">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="861f7-484">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="861f7-484">Media content rating settings for United States</span></span>|
|<span data-ttu-id="861f7-485">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="861f7-485">networkUsageRules</span></span>|<span data-ttu-id="861f7-486">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="861f7-486">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="861f7-487">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="861f7-487">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="861f7-488">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="861f7-488">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="861f7-489">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="861f7-489">mediaContentRatingApps</span></span>|[<span data-ttu-id="861f7-490">Ратингаппстипе</span><span class="sxs-lookup"><span data-stu-id="861f7-490">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="861f7-491">Параметры оценки контента мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="861f7-491">Media content rating settings for Apps.</span></span> <span data-ttu-id="861f7-492">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="861f7-492">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="861f7-493">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-493">messagesBlocked</span></span>|<span data-ttu-id="861f7-494">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-494">Boolean</span></span>|<span data-ttu-id="861f7-495">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="861f7-495">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="861f7-496">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="861f7-496">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="861f7-497">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-497">Boolean</span></span>|<span data-ttu-id="861f7-498">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-498">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="861f7-499">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="861f7-499">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="861f7-500">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-500">Boolean</span></span>|<span data-ttu-id="861f7-501">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="861f7-501">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="861f7-502">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="861f7-502">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="861f7-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-503">Boolean</span></span>|<span data-ttu-id="861f7-504">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-504">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="861f7-505">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="861f7-505">passcodeBlockModification</span></span>|<span data-ttu-id="861f7-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-506">Boolean</span></span>|<span data-ttu-id="861f7-507">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-507">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="861f7-508">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="861f7-508">passcodeBlockSimple</span></span>|<span data-ttu-id="861f7-509">Логический</span><span class="sxs-lookup"><span data-stu-id="861f7-509">Boolean</span></span>|<span data-ttu-id="861f7-510">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="861f7-510">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="861f7-511">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="861f7-511">passcodeExpirationDays</span></span>|<span data-ttu-id="861f7-512">Int32</span><span class="sxs-lookup"><span data-stu-id="861f7-512">Int32</span></span>|<span data-ttu-id="861f7-513">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="861f7-513">Number of days before the passcode expires.</span></span> <span data-ttu-id="861f7-514">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="861f7-514">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="861f7-515">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="861f7-515">passcodeMinimumLength</span></span>|<span data-ttu-id="861f7-516">Int32</span><span class="sxs-lookup"><span data-stu-id="861f7-516">Int32</span></span>|<span data-ttu-id="861f7-517">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="861f7-517">Minimum length of passcode.</span></span> <span data-ttu-id="861f7-518">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="861f7-518">Valid values 4 to 14</span></span>|
|<span data-ttu-id="861f7-519">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="861f7-519">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="861f7-520">Int32</span><span class="sxs-lookup"><span data-stu-id="861f7-520">Int32</span></span>|<span data-ttu-id="861f7-521">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="861f7-521">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="861f7-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="861f7-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="861f7-523">Int32</span><span class="sxs-lookup"><span data-stu-id="861f7-523">Int32</span></span>|<span data-ttu-id="861f7-524">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="861f7-524">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="861f7-525">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="861f7-525">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="861f7-526">Int32</span><span class="sxs-lookup"><span data-stu-id="861f7-526">Int32</span></span>|<span data-ttu-id="861f7-527">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="861f7-527">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="861f7-528">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="861f7-528">Valid values 0 to 4</span></span>|
|<span data-ttu-id="861f7-529">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="861f7-529">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="861f7-530">Int32</span><span class="sxs-lookup"><span data-stu-id="861f7-530">Int32</span></span>|<span data-ttu-id="861f7-531">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="861f7-531">Number of previous passcodes to block.</span></span> <span data-ttu-id="861f7-532">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="861f7-532">Valid values 1 to 24</span></span>|
|<span data-ttu-id="861f7-533">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="861f7-533">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="861f7-534">Int32</span><span class="sxs-lookup"><span data-stu-id="861f7-534">Int32</span></span>|<span data-ttu-id="861f7-535">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="861f7-535">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="861f7-536">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="861f7-536">Valid values 4 to 11</span></span>|
|<span data-ttu-id="861f7-537">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="861f7-537">passcodeRequiredType</span></span>|[<span data-ttu-id="861f7-538">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="861f7-538">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="861f7-539">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="861f7-539">Type of passcode that is required.</span></span> <span data-ttu-id="861f7-540">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="861f7-540">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="861f7-541">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="861f7-541">passcodeRequired</span></span>|<span data-ttu-id="861f7-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-542">Boolean</span></span>|<span data-ttu-id="861f7-543">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="861f7-543">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="861f7-544">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-544">podcastsBlocked</span></span>|<span data-ttu-id="861f7-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-545">Boolean</span></span>|<span data-ttu-id="861f7-546">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-546">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="861f7-547">Проксимитиблокксетуптоневдевице</span><span class="sxs-lookup"><span data-stu-id="861f7-547">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="861f7-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-548">Boolean</span></span>|<span data-ttu-id="861f7-549">Указывает, следует ли включить запрос на установку находящихся рядом устройств с защищенным устройством.</span><span class="sxs-lookup"><span data-stu-id="861f7-549">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="861f7-550">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="861f7-550">safariBlockAutofill</span></span>|<span data-ttu-id="861f7-551">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-551">Boolean</span></span>|<span data-ttu-id="861f7-552">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="861f7-552">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="861f7-553">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="861f7-553">safariBlockJavaScript</span></span>|<span data-ttu-id="861f7-554">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-554">Boolean</span></span>|<span data-ttu-id="861f7-555">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="861f7-555">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="861f7-556">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="861f7-556">safariBlockPopups</span></span>|<span data-ttu-id="861f7-557">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-557">Boolean</span></span>|<span data-ttu-id="861f7-558">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="861f7-558">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="861f7-559">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-559">safariBlocked</span></span>|<span data-ttu-id="861f7-560">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-560">Boolean</span></span>|<span data-ttu-id="861f7-561">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="861f7-561">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="861f7-562">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="861f7-562">safariCookieSettings</span></span>|[<span data-ttu-id="861f7-563">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="861f7-563">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="861f7-564">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="861f7-564">Cookie settings for Safari.</span></span> <span data-ttu-id="861f7-565">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="861f7-565">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="861f7-566">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="861f7-566">safariManagedDomains</span></span>|<span data-ttu-id="861f7-567">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="861f7-567">String collection</span></span>|<span data-ttu-id="861f7-568">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="861f7-568">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="861f7-569">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="861f7-569">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="861f7-570">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="861f7-570">String collection</span></span>|<span data-ttu-id="861f7-571">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="861f7-571">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="861f7-572">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-572">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="861f7-573">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="861f7-573">safariRequireFraudWarning</span></span>|<span data-ttu-id="861f7-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-574">Boolean</span></span>|<span data-ttu-id="861f7-575">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="861f7-575">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="861f7-576">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-576">screenCaptureBlocked</span></span>|<span data-ttu-id="861f7-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-577">Boolean</span></span>|<span data-ttu-id="861f7-578">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="861f7-578">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="861f7-579">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-579">siriBlocked</span></span>|<span data-ttu-id="861f7-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-580">Boolean</span></span>|<span data-ttu-id="861f7-581">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="861f7-581">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="861f7-582">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="861f7-582">siriBlockedWhenLocked</span></span>|<span data-ttu-id="861f7-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-583">Boolean</span></span>|<span data-ttu-id="861f7-584">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="861f7-584">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="861f7-585">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="861f7-585">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="861f7-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-586">Boolean</span></span>|<span data-ttu-id="861f7-587">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="861f7-587">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="861f7-588">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="861f7-588">siriRequireProfanityFilter</span></span>|<span data-ttu-id="861f7-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-589">Boolean</span></span>|<span data-ttu-id="861f7-590">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="861f7-590">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="861f7-591">Софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="861f7-591">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="861f7-592">Int32</span><span class="sxs-lookup"><span data-stu-id="861f7-592">Int32</span></span>|<span data-ttu-id="861f7-593">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="861f7-593">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="861f7-594">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="861f7-594">Valid values 0 to 90</span></span>|
|<span data-ttu-id="861f7-595">Софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="861f7-595">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="861f7-596">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-596">Boolean</span></span>|<span data-ttu-id="861f7-597">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-597">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-598">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="861f7-598">spotlightBlockInternetResults</span></span>|<span data-ttu-id="861f7-599">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-599">Boolean</span></span>|<span data-ttu-id="861f7-600">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="861f7-600">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="861f7-601">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-601">voiceDialingBlocked</span></span>|<span data-ttu-id="861f7-602">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-602">Boolean</span></span>|<span data-ttu-id="861f7-603">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="861f7-603">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="861f7-604">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="861f7-604">wallpaperBlockModification</span></span>|<span data-ttu-id="861f7-605">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-605">Boolean</span></span>|<span data-ttu-id="861f7-606">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-606">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="861f7-607">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="861f7-607">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="861f7-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-608">Boolean</span></span>|<span data-ttu-id="861f7-609">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="861f7-609">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="861f7-610">Классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="861f7-610">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="861f7-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-611">Boolean</span></span>|<span data-ttu-id="861f7-612">Указывает, является ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса (iOS 11,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-612">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="861f7-613">Кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="861f7-613">keychainBlockCloudSync</span></span>|<span data-ttu-id="861f7-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-614">Boolean</span></span>|<span data-ttu-id="861f7-615">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud.</span><span class="sxs-lookup"><span data-stu-id="861f7-615">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="861f7-616">Пкиблоккотаупдатес</span><span class="sxs-lookup"><span data-stu-id="861f7-616">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="861f7-617">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-617">Boolean</span></span>|<span data-ttu-id="861f7-618">Указывает, блокируются ли обновления PKI беспроводной сети.</span><span class="sxs-lookup"><span data-stu-id="861f7-618">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="861f7-619">Если задать для этого ограничения значение false, проверки CRL и OCSP (iOS 7,0 и более поздних версий) не отключаются.</span><span class="sxs-lookup"><span data-stu-id="861f7-619">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="861f7-620">Привацифорцелимитадтраккинг</span><span class="sxs-lookup"><span data-stu-id="861f7-620">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="861f7-621">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-621">Boolean</span></span>|<span data-ttu-id="861f7-622">Указывает, ограничено ли отслеживание AD. (iOS 7,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-622">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="861f7-623">Ентерприсебукблоккбаккуп</span><span class="sxs-lookup"><span data-stu-id="861f7-623">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="861f7-624">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-624">Boolean</span></span>|<span data-ttu-id="861f7-625">Указывает, блокируется ли резервное копирование корпоративной книги.</span><span class="sxs-lookup"><span data-stu-id="861f7-625">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="861f7-626">Ентерприсебукблоккметадатасинк</span><span class="sxs-lookup"><span data-stu-id="861f7-626">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="861f7-627">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-627">Boolean</span></span>|<span data-ttu-id="861f7-628">Указывает, блокируется ли синхронизация заметок и выделений корпоративных книг.</span><span class="sxs-lookup"><span data-stu-id="861f7-628">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="861f7-629">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="861f7-629">airPrintBlocked</span></span>|<span data-ttu-id="861f7-630">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-630">Boolean</span></span>|<span data-ttu-id="861f7-631">Указывает, заблокировано ли Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-631">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="861f7-632">Аирпринтблокккредентиалсстораже</span><span class="sxs-lookup"><span data-stu-id="861f7-632">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="861f7-633">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-633">Boolean</span></span>|<span data-ttu-id="861f7-634">Указывает, заблокировано ли хранение цепочки ключей имени пользователя и пароля для Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-634">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="861f7-635">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="861f7-635">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="861f7-636">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-636">Boolean</span></span>|<span data-ttu-id="861f7-637">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-637">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="861f7-638">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="861f7-638">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="861f7-639">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-639">Boolean</span></span>|<span data-ttu-id="861f7-640">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="861f7-640">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="861f7-641">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-641">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="861f7-642">Блокксистемаппремовал</span><span class="sxs-lookup"><span data-stu-id="861f7-642">blockSystemAppRemoval</span></span>|<span data-ttu-id="861f7-643">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-643">Boolean</span></span>|<span data-ttu-id="861f7-644">Указывает, заблокировано ли удаление системных приложений с устройства на контролируемом устройстве (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-644">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="861f7-645">Впнблокккреатион</span><span class="sxs-lookup"><span data-stu-id="861f7-645">vpnBlockCreation</span></span>|<span data-ttu-id="861f7-646">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-646">Boolean</span></span>|<span data-ttu-id="861f7-647">Указывает, блокируется ли создание конфигураций VPN (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-647">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="861f7-648">Аппремовалблоккед</span><span class="sxs-lookup"><span data-stu-id="861f7-648">appRemovalBlocked</span></span>|<span data-ttu-id="861f7-649">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-649">Boolean</span></span>|<span data-ttu-id="861f7-650">Указывает, разрешено ли удаление приложений.</span><span class="sxs-lookup"><span data-stu-id="861f7-650">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="861f7-651">Усбрестриктедмодеблоккед</span><span class="sxs-lookup"><span data-stu-id="861f7-651">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="861f7-652">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-652">Boolean</span></span>|<span data-ttu-id="861f7-653">Указывает, разрешена ли подключаться к стандарту USB, пока устройство заблокировано (iOS 11.4.1 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-653">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="861f7-654">Пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="861f7-654">passwordBlockAutoFill</span></span>|<span data-ttu-id="861f7-655">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-655">Boolean</span></span>|<span data-ttu-id="861f7-656">Указывает, разрешена ли функция автоЗаполнения паролей (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-656">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="861f7-657">Пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="861f7-657">passwordBlockProximityRequests</span></span>|<span data-ttu-id="861f7-658">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-658">Boolean</span></span>|<span data-ttu-id="861f7-659">Указывает, следует ли запретить запрашивать пароли с близлежащих устройств (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-659">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="861f7-660">Пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="861f7-660">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="861f7-661">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-661">Boolean</span></span>|<span data-ttu-id="861f7-662">Указывает, следует ли заблокировать общий доступ к паролям с помощью AirDrop паролей iOS 12,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="861f7-662">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="861f7-663">Датеандтимефорцесетаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="861f7-663">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="861f7-664">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-664">Boolean</span></span>|<span data-ttu-id="861f7-665">Указывает, включена ли функция даты и времени "автоматически задано" и не может быть отключена пользователем (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-665">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="861f7-666">Контактсалловманажедтаунманажедврите</span><span class="sxs-lookup"><span data-stu-id="861f7-666">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="861f7-667">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-667">Boolean</span></span>|<span data-ttu-id="861f7-668">Указывает, могут ли управляемые приложения записывать контакты в неуправляемые учетные записи контактов (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="861f7-668">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="861f7-669">Контактсалловунманажедтоманажедреад</span><span class="sxs-lookup"><span data-stu-id="861f7-669">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="861f7-670">Boolean</span><span class="sxs-lookup"><span data-stu-id="861f7-670">Boolean</span></span>|<span data-ttu-id="861f7-671">Указывает, могут ли неуправляемые приложения читать из управляемых учетных записей контактов (iOS 12,0 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="861f7-671">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="861f7-672">Отклик</span><span class="sxs-lookup"><span data-stu-id="861f7-672">Response</span></span>
<span data-ttu-id="861f7-673">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="861f7-673">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="861f7-674">Пример</span><span class="sxs-lookup"><span data-stu-id="861f7-674">Example</span></span>

### <a name="request"></a><span data-ttu-id="861f7-675">Запрос</span><span class="sxs-lookup"><span data-stu-id="861f7-675">Request</span></span>
<span data-ttu-id="861f7-676">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="861f7-676">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 9105

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true
}
```

### <a name="response"></a><span data-ttu-id="861f7-677">Отклик</span><span class="sxs-lookup"><span data-stu-id="861f7-677">Response</span></span>
<span data-ttu-id="861f7-p133">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="861f7-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9277

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true
}
```




